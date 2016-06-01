# RollingSales
Andrew Abbott, Ken Avery, Paola Leon, Earl Shaw  
May 30, 2016  


```r
setwd("/Users/Abbott/test-repo/RollingSales")
```

# Save the file as a csv and use read.csv

```r
queens <- read.csv("rollingsales_queens.csv",skip=4,header=TRUE)
```

## Check the data

```r
head(queens)
```

```
##   BOROUGH              NEIGHBORHOOD
## 1       4 AIRPORT JFK              
## 2       4 AIRPORT LA GUARDIA       
## 3       4 AIRPORT LA GUARDIA       
## 4       4 AIRPORT LA GUARDIA       
## 5       4 AIRPORT LA GUARDIA       
## 6       4 AIRPORT LA GUARDIA       
##                        BUILDING.CLASS.CATEGORY TAX.CLASS.AT.PRESENT BLOCK
## 1 31  COMMERCIAL VACANT LAND                                      4 14260
## 2 01  ONE FAMILY DWELLINGS                                        1   976
## 3 03  THREE FAMILY DWELLINGS                                      1   949
## 4 03  THREE FAMILY DWELLINGS                                      1   949
## 5 03  THREE FAMILY DWELLINGS                                      1   976
## 6 39  TRANSPORTATION FACILITIES                                   4   926
##   LOT EASE.MENT BUILDING.CLASS.AT.PRESENT
## 1  70        NA                        V1
## 2  13        NA                        A5
## 3  51        NA                        C0
## 4  52        NA                        C0
## 5  38        NA                        C0
## 6   1        NA                        T1
##                                     ADDRESS APARTMENT.NUMBER ZIP.CODE
## 1 181-25 EASTERN ROAD                                           11430
## 2 21-16 81ST   STREET                                           11370
## 3 19-79 80TH STREET                                             11370
## 4 19-77 80TH STREET                                             11370
## 5 21-66 81ST STREET                                             11370
## 6 83-00 23RD   AVENUE                                           11370
##   RESIDENTIAL.UNITS COMMERCIAL.UNITS TOTAL.UNITS LAND.SQUARE.FEET
## 1                 0                0           0           223027
## 2                 1                0           1             1800
## 3                 3                0           3             2000
## 4                 3                0           3             2000
## 5                 3                0           3             2100
## 6                 0                4           4         29305534
##   GROSS.SQUARE.FEET YEAR.BUILT TAX.CLASS.AT.TIME.OF.SALE
## 1                 0          0                         4
## 2              1224       1950                         1
## 3              2635       1945                         1
## 4              2835       1945                         1
## 5              2016       1950                         1
## 6           2949024       1933                         4
##   BUILDING.CLASS.AT.TIME.OF.SALE   SALE.PRICE  SALE.DATE
## 1                             V1  $7,800,000   1/14/2016
## 2                             A5    $620,000   10/6/2015
## 3                             C0        $-     6/26/2015
## 4                             C0        $-     8/13/2015
## 5                             C0        $-    12/15/2015
## 6                             T1        $-     7/22/2015
```

```r
summary(queens)
```

```
##     BOROUGH                     NEIGHBORHOOD  
##  Min.   :4   FLUSHING-NORTH           : 2572  
##  1st Qu.:4   FOREST HILLS             : 1185  
##  Median :4   BAYSIDE                  : 1068  
##  Mean   :4   ASTORIA                  : 1042  
##  3rd Qu.:4   JACKSON HEIGHTS          : 1037  
##  Max.   :4   FLUSHING-SOUTH           :  822  
##              (Other)                  :17398  
##                                  BUILDING.CLASS.CATEGORY
##  01  ONE FAMILY DWELLINGS                    :7860      
##  02  TWO FAMILY DWELLINGS                    :5247      
##  10  COOPS - ELEVATOR APARTMENTS             :3763      
##  13  CONDOS - ELEVATOR APARTMENTS            :1868      
##  09  COOPS - WALKUP APARTMENTS               :1279      
##  03  THREE FAMILY DWELLINGS                  :1217      
##  (Other)                                     :3890      
##  TAX.CLASS.AT.PRESENT     BLOCK            LOT         EASE.MENT     
##  1      :14389        Min.   :   13   Min.   :   1.0   Mode:logical  
##  2      : 7387        1st Qu.: 2702   1st Qu.:  16.0   NA's:25124    
##  4      : 1760        Median : 5843   Median :  39.0                 
##  2A     :  612        Mean   : 6554   Mean   : 208.7                 
##  1A     :  384        3rd Qu.: 9968   3rd Qu.:  82.0                 
##  1B     :  365        Max.   :16322   Max.   :7097.0                 
##  (Other):  227                                                       
##  BUILDING.CLASS.AT.PRESENT
##  D4     : 3763            
##  A1     : 3606            
##  A5     : 1954            
##  R4     : 1864            
##  B3     : 1773            
##  B2     : 1747            
##  (Other):10417            
##                                       ADDRESS          APARTMENT.NUMBER
##  41-23 CRESCENT STREET                    :  152               :22029  
##  120 BEACH 26 STREET                      :  127   3A          :   56  
##  142-28 38TH   AVENUE                     :   74   2A          :   54  
##  65-20 BOOTH STREET                       :   67   3B          :   47  
##  108-20 71ST    AVENUE                    :   55   2B          :   45  
##  106-20 70TH   AVENUE                     :   45   4B          :   42  
##  (Other)                                  :24604   (Other)     : 2851  
##     ZIP.CODE     RESIDENTIAL.UNITS COMMERCIAL.UNITS  TOTAL.UNITS    
##  Min.   :    0   Min.   :  0.000   Min.   :  0.00   Min.   :  0.00  
##  1st Qu.:11361   1st Qu.:  0.000   1st Qu.:  0.00   1st Qu.:  1.00  
##  Median :11375   Median :  1.000   Median :  0.00   Median :  1.00  
##  Mean   :11367   Mean   :  1.493   Mean   :  0.11   Mean   :  1.63  
##  3rd Qu.:11419   3rd Qu.:  2.000   3rd Qu.:  0.00   3rd Qu.:  2.00  
##  Max.   :11694   Max.   :442.000   Max.   :123.00   Max.   :442.00  
##                                                                     
##  LAND.SQUARE.FEET   GROSS.SQUARE.FEET   YEAR.BUILT  
##  Min.   :       0   Min.   :      0   Min.   :   0  
##  1st Qu.:       0   1st Qu.:      0   1st Qu.:1925  
##  Median :    2064   Median :   1268   Median :1945  
##  Mean   :    3712   Mean   :   1944   Mean   :1859  
##  3rd Qu.:    3310   3rd Qu.:   1994   3rd Qu.:1960  
##  Max.   :29305534   Max.   :2949024   Max.   :2016  
##                                                     
##  TAX.CLASS.AT.TIME.OF.SALE BUILDING.CLASS.AT.TIME.OF.SALE
##  Min.   :1.000             D4     : 3763                 
##  1st Qu.:1.000             A1     : 3607                 
##  Median :1.000             A5     : 1956                 
##  Mean   :1.537             R4     : 1868                 
##  3rd Qu.:2.000             B3     : 1752                 
##  Max.   :4.000             B2     : 1740                 
##                            (Other):10438                 
##       SALE.PRICE         SALE.DATE    
##   $-       : 7488   1/20/2016 :  250  
##   $10      :  206   4/5/2016  :  183  
##   $450,000 :  161   8/13/2015 :  181  
##   $400,000 :  143   6/18/2015 :  169  
##   $300,000 :  142   2/29/2016 :  160  
##   $600,000 :  132   10/29/2015:  153  
##  (Other)   :16852   (Other)   :24028
```

```r
str(queens)
```

```
## 'data.frame':	25124 obs. of  21 variables:
##  $ BOROUGH                       : int  4 4 4 4 4 4 4 4 4 4 ...
##  $ NEIGHBORHOOD                  : Factor w/ 61 levels "AIRPORT JFK              ",..: 1 2 2 2 2 2 3 3 3 3 ...
##  $ BUILDING.CLASS.CATEGORY       : Factor w/ 42 levels "01  ONE FAMILY DWELLINGS                    ",..: 27 1 3 3 3 35 1 1 1 1 ...
##  $ TAX.CLASS.AT.PRESENT          : Factor w/ 9 levels "1","1A","1B",..: 9 1 1 1 1 9 1 1 1 1 ...
##  $ BLOCK                         : int  14260 976 949 949 976 926 15828 15830 15837 15837 ...
##  $ LOT                           : int  70 13 51 52 38 1 53 42 17 17 ...
##  $ EASE.MENT                     : logi  NA NA NA NA NA NA ...
##  $ BUILDING.CLASS.AT.PRESENT     : Factor w/ 114 levels "A0","A1","A2",..: 106 6 14 14 14 104 2 3 7 7 ...
##  $ ADDRESS                       : Factor w/ 22157 levels "1-06 SAMOS LN                            ",..: 7642 8648 7959 7957 8752 19081 11505 12371 12174 12174 ...
##  $ APARTMENT.NUMBER              : Factor w/ 1135 levels "            ",..: 1 1 1 1 1 1 1 1 1 1 ...
##  $ ZIP.CODE                      : int  11430 11370 11370 11370 11370 11370 11691 11691 11691 11691 ...
##  $ RESIDENTIAL.UNITS             : int  0 1 3 3 3 0 1 1 1 1 ...
##  $ COMMERCIAL.UNITS              : int  0 0 0 0 0 4 0 0 0 0 ...
##  $ TOTAL.UNITS                   : int  0 1 3 3 3 4 1 1 1 1 ...
##  $ LAND.SQUARE.FEET              : int  223027 1800 2000 2000 2100 29305534 3810 1766 3804 3804 ...
##  $ GROSS.SQUARE.FEET             : int  0 1224 2635 2835 2016 2949024 1200 1521 745 745 ...
##  $ YEAR.BUILT                    : int  0 1950 1945 1945 1950 1933 2002 1920 1925 1925 ...
##  $ TAX.CLASS.AT.TIME.OF.SALE     : int  4 1 1 1 1 4 1 1 1 1 ...
##  $ BUILDING.CLASS.AT.TIME.OF.SALE: Factor w/ 116 levels "A0","A1","A2",..: 108 6 14 14 14 106 2 3 7 7 ...
##  $ SALE.PRICE                    : Factor w/ 3220 levels " $-   "," $1 ",..: 2707 2509 1 1 1 1 1158 1 1242 2673 ...
##  $ SALE.DATE                     : Factor w/ 347 levels "1/1/2016","1/10/2016",..: 6 58 251 295 97 277 141 147 11 218 ...
```

# We create a new variable that is a "clean" version of sale.price.
# sale.price.n is numeric, not a factor.

```r
library(plyr)
queens$SALE.PRICE.N <- as.numeric(gsub("[^[:digit:]]","", queens$SALE.PRICE))
count(is.na(queens$SALE.PRICE.N))
```

```
##       x  freq
## 1 FALSE 17636
## 2  TRUE  7488
```
There are 7,488 without values.

# Make all variable names lower case

```r
names(queens) <- tolower(names(queens)) 
names(queens)
```

```
##  [1] "borough"                        "neighborhood"                  
##  [3] "building.class.category"        "tax.class.at.present"          
##  [5] "block"                          "lot"                           
##  [7] "ease.ment"                      "building.class.at.present"     
##  [9] "address"                        "apartment.number"              
## [11] "zip.code"                       "residential.units"             
## [13] "commercial.units"               "total.units"                   
## [15] "land.square.feet"               "gross.square.feet"             
## [17] "year.built"                     "tax.class.at.time.of.sale"     
## [19] "building.class.at.time.of.sale" "sale.price"                    
## [21] "sale.date"                      "sale.price.n"
```

## Get rid of leading digits and make sure numeric


```r
queens$gross.sqft <- as.numeric(gsub("[^[:digit:]]","", queens$gross.square.feet))
queens$land.sqft <- as.numeric(gsub("[^[:digit:]]","", queens$land.square.feet))
class(queens$gross.sqft)
```

```
## [1] "numeric"
```

```r
class(queens$land.sqft)
```

```
## [1] "numeric"
```

## Change sale.date to Date format in R, format must be specified.

```r
queens$sale.date <- as.Date(queens$sale.date, "%m/%d/%y")
queens$year.built <- as.numeric(as.character(queens$year.built))
class(queens$sale.date)
```

```
## [1] "Date"
```


## Do a bit of exploration to make sure there's not anything
## weird going on with sale prices

```r
attach(queens)
hist(sale.price.n) 
```

![](Rollingsales_files/figure-html/unnamed-chunk-8-1.png)<!-- -->

# Everything looks to be 0

```r
hist(sale.price.n[sale.price.n>0])
```

![](Rollingsales_files/figure-html/unnamed-chunk-9-1.png)<!-- -->

#That didn't help

```r
hist(sale.price.n[sale.price.n<1000000])
```

![](Rollingsales_files/figure-html/unnamed-chunk-10-1.png)<!-- -->

#that looks reasonable


```r
detach(queens)
```

##Now that the data is in correct formats and types we will write it to a new .csv file.

```r
write.csv(queens, file = "rollingsales_queens2.csv", )
```



## Lets keep only the actual sales and create a new data frame to hold them.
##First lets load the clean data.


```r
queens2 <- read.csv("rollingsales_queens2.csv",header=TRUE)
```

##Next lets filter out sales prices of $0.00


```r
queens.sale <-queens2[queens2$sale.price.n!=0,]
```

## We include only sales with prices greater than $0.


```r
plot(queens.sale$gross.sqft,queens.sale$sale.price.n)
```

![](Rollingsales_files/figure-html/unnamed-chunk-15-1.png)<!-- -->

```r
plot(log(queens.sale$gross.sqft),log(queens.sale$sale.price.n))
```

![](Rollingsales_files/figure-html/unnamed-chunk-16-1.png)<!-- -->

##Save this data step in a csv file.


```r
write.csv(queens.sale, file = "rollingsales_queenssale.csv")
```

## There are still some really large sales prices muddling the data.
## for now, let's look at 1-, 2-, and 3-family homes only
## and create a new data frame to hold them.


```r
queens3 <- read.csv("rollingsales_queenssale.csv",header=TRUE)
```



```r
queens.homes <- queens3[which(grepl("FAMILY",queens3$building.class.category)),]
dim(queens.homes)
```

```
## [1] 9711   26
```


```r
hist(queens.homes$sale.price.n)
```

![](Rollingsales_files/figure-html/unnamed-chunk-20-1.png)<!-- -->

```r
plot(log(queens.homes$gross.sqft),log(queens.homes$sale.price.n))
```

![](Rollingsales_files/figure-html/unnamed-chunk-21-1.png)<!-- -->

```r
summary(queens.homes[which(queens.homes$sale.price.n<100000),])
```

```
##       X.1            X            borough                     neighborhood
##  10     :  1   Min.   :   10   Min.   :4   SOUTH JAMAICA            : 22  
##  10852  :  1   1st Qu.: 6849   1st Qu.:4   FLUSHING-NORTH           : 21  
##  10888  :  1   Median :15050   Median :4   SOUTH OZONE PARK         : 19  
##  10897  :  1   Mean   :14203   Mean   :4   SPRINGFIELD GARDENS      : 18  
##  11     :  1   3rd Qu.:21546   3rd Qu.:4   HOLLIS                   : 16  
##  11410  :  1   Max.   :24812   Max.   :4   HOWARD BEACH             : 16  
##  (Other):368                               (Other)                  :262  
##                                  building.class.category
##  01  ONE FAMILY DWELLINGS                    :231       
##  02  TWO FAMILY DWELLINGS                    :128       
##  03  THREE FAMILY DWELLINGS                  : 15       
##  04  TAX CLASS 1 CONDOS                      :  0       
##  05  TAX CLASS 1 VACANT LAND                 :  0       
##  06  TAX CLASS 1 - OTHER                     :  0       
##  (Other)                                     :  0       
##  tax.class.at.present     block            lot          ease.ment     
##  1      :374          Min.   :  162   Min.   :   1.00   Mode:logical  
##  1A     :  0          1st Qu.: 6335   1st Qu.:  19.00   NA's:374      
##  1B     :  0          Median :10244   Median :  40.00                 
##  1C     :  0          Mean   : 9330   Mean   :  71.01                 
##  2      :  0          3rd Qu.:12513   3rd Qu.:  69.00                 
##  2A     :  0          Max.   :16268   Max.   :1523.00                 
##  (Other):  0                                                          
##  building.class.at.present                                      address   
##  A1     :104               70-37 175TH   STREET                     :  3  
##  B3     : 52               106-35 96TH   STREET                     :  2  
##  A5     : 50               31-14 70TH STREET                        :  2  
##  A2     : 42               317 BEACH 13 STREET                      :  2  
##  B2     : 36               10-36 116TH   STREET                     :  1  
##  B1     : 24               100-02 ROCKAWAY BEACH BLVD               :  1  
##  (Other): 66               (Other)                                  :363  
##      apartment.number    zip.code     residential.units commercial.units 
##              :374     Min.   :11001   Min.   :1.000     Min.   :0.00000  
##  1           :  0     1st Qu.:11370   1st Qu.:1.000     1st Qu.:0.00000  
##  1-A         :  0     Median :11416   Median :1.000     Median :0.00000  
##  1-C         :  0     Mean   :11419   Mean   :1.422     Mean   :0.02139  
##  1.00E+02    :  0     3rd Qu.:11429   3rd Qu.:2.000     3rd Qu.:0.00000  
##  10-A        :  0     Max.   :11694   Max.   :3.000     Max.   :1.00000  
##  (Other)     :  0                                                        
##   total.units    land.square.feet gross.square.feet   year.built  
##  Min.   :1.000   Min.   : 305     Min.   : 300      Min.   :1899  
##  1st Qu.:1.000   1st Qu.:2000     1st Qu.:1200      1st Qu.:1920  
##  Median :1.000   Median :2672     Median :1481      Median :1931  
##  Mean   :1.444   Mean   :2986     Mean   :1609      Mean   :1938  
##  3rd Qu.:2.000   3rd Qu.:4000     3rd Qu.:2000      3rd Qu.:1950  
##  Max.   :3.000   Max.   :7764     Max.   :4467      Max.   :2014  
##                                                                   
##  tax.class.at.time.of.sale building.class.at.time.of.sale     sale.price 
##  Min.   :1                 A1     :104                     $10     :167  
##  1st Qu.:1                 B3     : 52                     $1      : 25  
##  Median :1                 A5     : 50                     $20,000 : 15  
##  Mean   :1                 A2     : 42                     $1,000  : 13  
##  3rd Qu.:1                 B2     : 36                     $90,000 : 10  
##  Max.   :1                 B1     : 24                     $25,000 :  8  
##                            (Other): 66                    (Other)  :136  
##       sale.date    sale.price.n     gross.sqft     land.sqft   
##  2020-05-26:  6   Min.   :    1   Min.   : 300   Min.   : 305  
##  2020-02-22:  5   1st Qu.:   10   1st Qu.:1200   1st Qu.:2000  
##  2020-06-02:  5   Median :   10   Median :1481   Median :2672  
##  2020-09-25:  5   Mean   :17550   Mean   :1609   Mean   :2986  
##  2020-09-29:  5   3rd Qu.:25000   3rd Qu.:2000   3rd Qu.:4000  
##  2020-06-08:  4   Max.   :96000   Max.   :4467   Max.   :7764  
##  (Other)   :344
```

## Now to remove outliers that seem like they weren't actual sales

```r
queens.homes$outliers <- (log(queens.homes$sale.price.n) <=10) + 0
queens.homes <- queens.homes[which(queens.homes$outliers==0),]
plot(log(queens.homes$gross.sqft),log(queens.homes$sale.price.n))
```

![](Rollingsales_files/figure-html/unnamed-chunk-22-1.png)<!-- -->

## Finally save the dataframe as new csv files:


```r
write.csv(queens.homes, file = "rollingsales_queenshomes.csv")
```

