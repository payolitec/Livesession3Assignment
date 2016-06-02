# RollingSales
Andrew Abbott, Ken Avery, Paola Leon, Earl Shaw  
May 30, 2016  


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

