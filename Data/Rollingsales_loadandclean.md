



<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-89838813501af0ab77e1b954a224433f83e8f31af4b3a4570c8343b6a972ba1c.css" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-308233841d8e7af078ce5873e18f8a07f391a38ce8d12120a384edf406f51c38.css" media="all" rel="stylesheet" />
    
    
    
    

    <link as="script" href="https://assets-cdn.github.com/assets/frameworks-b801b4f0918b70f4a3a4105efbf8e5c567b4b12e41a263b4805397c93aebf317.js" rel="preload" />
    
    <link as="script" href="https://assets-cdn.github.com/assets/github-9e11266e9840a1629501dc03630329cc0bd58efc0dcfcc89a16868ba1d5c1465.js" rel="preload" />

    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=device-width">
    
    
    <title>Livesession3Assignment/Rollingsales_loadandclean.md at master · payolitec/Livesession3Assignment</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" href="/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-touch-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-touch-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-touch-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-touch-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180x180.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="https://avatars1.githubusercontent.com/u/19627294?v=3&amp;s=400" name="twitter:image:src" /><meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="payolitec/Livesession3Assignment" name="twitter:title" /><meta content="Livesession3Assignment - MSDS 6306 DOING DATA SCIENCE - 401" name="twitter:description" />
      <meta content="https://avatars1.githubusercontent.com/u/19627294?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="payolitec/Livesession3Assignment" property="og:title" /><meta content="https://github.com/payolitec/Livesession3Assignment" property="og:url" /><meta content="Livesession3Assignment - MSDS 6306 DOING DATA SCIENCE - 401" property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="web-socket" href="wss://live.github.com/_sockets/MTk2MjcyOTQ6MTI1YjA3OWY1MzJhZTliOThmZDg3ZjMyYjYxYmE1Y2I6ODI5YWFjMzM5NDBkZTVhZmJlNjJhNThjZWUxMGQ1NDBmOGVmNWU4NDNkNmQ5MDIzYjEzMzIzNGFiYjM1ODNjZg==--c4086b37b4d979534066b6a1462e25dcfd8833d6">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="4A339F71:8524:10054A7C:57504FE6" name="octolytics-dimension-request_id" /><meta content="19627294" name="octolytics-actor-id" /><meta content="payolitec" name="octolytics-actor-login" /><meta content="4a4b6028ce06c2d68b6ffdd62c4ecf8c233650a1b6b50024d0cdd420b50b0894" name="octolytics-actor-hash" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />



  <meta class="js-ga-set" name="dimension1" content="Logged In">



        <meta name="hostname" content="github.com">
    <meta name="user-login" content="payolitec">

        <meta name="expected-hostname" content="github.com">
      <meta name="js-proxy-site-detection-payload" content="YWE0MGUwZmI4MTM1NTc3ZDI1MjY4MzgzNGU4MTk2YmUzOGViNTlmNjU3NDJiZWM2MjQwMDJkYTViNzhiY2JhOXx7InJlbW90ZV9hZGRyZXNzIjoiNzQuNTEuMTU5LjExMyIsInJlcXVlc3RfaWQiOiI0QTMzOUY3MTo4NTI0OjEwMDU0QTdDOjU3NTA0RkU2IiwidGltZXN0YW1wIjoxNDY0ODgxMTI3fQ==">


      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta name="html-safe-nonce" content="b839dadf510bea084835c236cd125282d7c119c6">
    <meta content="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" name="form-nonce" />

    <meta http-equiv="x-pjax-version" content="f0691b9f15824111b7853857b85a7fd5">
    

      
  <meta name="description" content="Livesession3Assignment - MSDS 6306 DOING DATA SCIENCE - 401">
  <meta name="go-import" content="github.com/payolitec/Livesession3Assignment git https://github.com/payolitec/Livesession3Assignment.git">

  <meta content="19627294" name="octolytics-dimension-user_id" /><meta content="payolitec" name="octolytics-dimension-user_login" /><meta content="59912216" name="octolytics-dimension-repository_id" /><meta content="payolitec/Livesession3Assignment" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="59912216" name="octolytics-dimension-repository_network_root_id" /><meta content="payolitec/Livesession3Assignment" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/payolitec/Livesession3Assignment/commits/master.atom" rel="alternate" title="Recent Commits to Livesession3Assignment:master" type="application/atom+xml">


      <link rel="canonical" href="https://github.com/payolitec/Livesession3Assignment/blob/master/Paper/Rollingsales_loadandclean.md" data-pjax-transient>
  </head>


  <body class="logged-in   env-production  vis-public page-blob">
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"></div>
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



        <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <svg aria-hidden="true" class="octicon octicon-mark-github" height="28" version="1.1" viewBox="0 0 16 16" width="28"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59 0.4 0.07 0.55-0.17 0.55-0.38 0-0.19-0.01-0.82-0.01-1.49-2.01 0.37-2.53-0.49-2.69-0.94-0.09-0.23-0.48-0.94-0.82-1.13-0.28-0.15-0.68-0.52-0.01-0.53 0.63-0.01 1.08 0.58 1.23 0.82 0.72 1.21 1.87 0.87 2.33 0.66 0.07-0.52 0.28-0.87 0.51-1.07-1.78-0.2-3.64-0.89-3.64-3.95 0-0.87 0.31-1.59 0.82-2.15-0.08-0.2-0.36-1.02 0.08-2.12 0 0 0.67-0.21 2.2 0.82 0.64-0.18 1.32-0.27 2-0.27 0.68 0 1.36 0.09 2 0.27 1.53-1.04 2.2-0.82 2.2-0.82 0.44 1.1 0.16 1.92 0.08 2.12 0.51 0.56 0.82 1.27 0.82 2.15 0 3.07-1.87 3.75-3.65 3.95 0.29 0.25 0.54 0.73 0.54 1.48 0 1.07-0.01 1.93-0.01 2.2 0 0.21 0.15 0.46 0.55 0.38C13.71 14.53 16 11.53 16 8 16 3.58 12.42 0 8 0z"></path></svg>
</a>


        <div class="header-search scoped-search site-scoped-search js-site-search" role="search">
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/payolitec/Livesession3Assignment/search" class="js-site-search-form" data-scoped-search-url="/payolitec/Livesession3Assignment/search" data-unscoped-search-url="/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <label class="form-control header-search-wrapper js-chromeless-input-container">
      <div class="header-search-scope">This repository</div>
      <input type="text"
        class="form-control header-search-input js-site-search-focus js-site-search-field is-clearable"
        data-hotkey="s"
        name="q"
        placeholder="Search"
        aria-label="Search this repository"
        data-unscoped-placeholder="Search GitHub"
        data-scoped-placeholder="Search"
        tabindex="1"
        autocapitalize="off">
    </label>
</form></div>


      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item">
          <a href="/pulls" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:pulls context:user" data-hotkey="g p" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls">
            Pull requests
</a>        </li>
        <li class="header-nav-item">
          <a href="/issues" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:issues context:user" data-hotkey="g i" data-selected-links="/issues /issues/assigned /issues/mentioned /issues">
            Issues
</a>        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com/" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item">
    

  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link tooltipped tooltipped-s js-menu-target" href="/new"
       aria-label="Create new…"
       data-ga-click="Header, create new, icon:add">
      <svg aria-hidden="true" class="octicon octicon-plus left" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 9H7v5H5V9H0V7h5V2h2v5h5v2z"></path></svg>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <ul class="dropdown-menu dropdown-menu-sw">
        
<a class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>

  <a class="dropdown-item" href="/new/import" data-ga-click="Header, import a repository">
    Import repository
  </a>


  <a class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="payolitec/Livesession3Assignment">This repository</span>
  </div>
    <a class="dropdown-item" href="/payolitec/Livesession3Assignment/issues/new" data-ga-click="Header, create new issue">
      New issue
    </a>
    <a class="dropdown-item" href="/payolitec/Livesession3Assignment/settings/collaboration" data-ga-click="Header, create new collaborator">
      New collaborator
    </a>

      </ul>
    </div>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name tooltipped tooltipped-sw js-menu-target" href="/payolitec"
       aria-label="View profile and more"
       data-ga-click="Header, show menu, icon:avatar">
      <img alt="@payolitec" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/19627294?v=3&amp;s=40" width="20" />
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <div class="dropdown-menu  dropdown-menu-sw">
        <div class=" dropdown-header header-nav-current-user css-truncate">
            Signed in as <strong class="css-truncate-target">payolitec</strong>

        </div>


        <div class="dropdown-divider"></div>

          <a class="dropdown-item" href="/payolitec" data-ga-click="Header, go to profile, text:your profile">
            Your profile
          </a>
        <a class="dropdown-item" href="/stars" data-ga-click="Header, go to starred repos, text:your stars">
          Your stars
        </a>
          <a class="dropdown-item" href="/explore" data-ga-click="Header, go to explore, text:explore">
            Explore
          </a>
          <a class="dropdown-item" href="/integrations" data-ga-click="Header, go to integrations, text:integrations">
            Integrations
          </a>
        <a class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">
          Help
        </a>


          <div class="dropdown-divider"></div>

          <a class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">
            Settings
          </a>

          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/logout" class="logout-form" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="X6x+SVeVp/nymLAXrh4aFDIIF3TfX8+nkjyQ77vkk1S3lHBp3A30jARlCAn3InE2tXgylYLh/c2D5Xb73BgItw==" /></div>
            <button class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
              Sign out
            </button>
</form>
      </div>
    </div>
  </li>
</ul>


    
  </div>
</div>


      


    <div id="start-of-content" class="accessibility-aid"></div>

      <div id="js-flash-container">
</div>


    <div role="main" class="main-content">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
        <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="Z1BD1sSOIuQBxALsVKieNCqIz1ZMofW7ETRUHvAeLTBR8SVtaIXI/Z8HO4Mp5aJAdBQr02SOLajLg9jCU2Uwdg==" /></div>      <input class="form-control" id="repository_id" name="repository_id" type="hidden" value="59912216" />

        <div class="select-menu js-menu-container js-select-menu">
          <a href="/payolitec/Livesession3Assignment/subscription"
            class="btn btn-sm btn-with-count select-menu-button js-menu-target" role="button" tabindex="0" aria-haspopup="true"
            data-ga-click="Repository, click Watch settings, action:blob#show">
            <span class="js-select-button">
              <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6c4.94 0 7.94-6 7.94-6S13 2 8.06 2z m-0.06 10c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4z m2-4c0 1.11-0.89 2-2 2s-2-0.89-2-2 0.89-2 2-2 2 0.89 2 2z"></path></svg>
              Unwatch
            </span>
          </a>
          <a class="social-count js-social-count" href="/payolitec/Livesession3Assignment/watchers">
            1
          </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header js-navigation-enable" tabindex="-1">
              <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
              <span class="select-menu-title">Notifications</span>
            </div>

              <div class="select-menu-list js-navigation-container" role="menu">

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_included" name="do" type="radio" value="included" />
                    <span class="select-menu-item-heading">Not watching</span>
                    <span class="description">Be notified when participating or @mentioned.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6c4.94 0 7.94-6 7.94-6S13 2 8.06 2z m-0.06 10c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4z m2-4c0 1.11-0.89 2-2 2s-2-0.89-2-2 0.89-2 2-2 2 0.89 2 2z"></path></svg>
                      Watch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input checked="checked" id="do_subscribed" name="do" type="radio" value="subscribed" />
                    <span class="select-menu-item-heading">Watching</span>
                    <span class="description">Be notified of all conversations.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6c4.94 0 7.94-6 7.94-6S13 2 8.06 2z m-0.06 10c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4z m2-4c0 1.11-0.89 2-2 2s-2-0.89-2-2 0.89-2 2-2 2 0.89 2 2z"></path></svg>
                      Unwatch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_ignore" name="do" type="radio" value="ignore" />
                    <span class="select-menu-item-heading">Ignoring</span>
                    <span class="description">Never be notified.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-mute" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8 2.81v10.38c0 0.67-0.81 1-1.28 0.53L3 10H1c-0.55 0-1-0.45-1-1V7c0-0.55 0.45-1 1-1h2l3.72-3.72c0.47-0.47 1.28-0.14 1.28 0.53z m7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06 1.97 1.97-1.97 1.97 1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06-1.97-1.97 1.97-1.97z"></path></svg>
                      Stop ignoring
                    </span>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/payolitec/Livesession3Assignment/unstar" class="starred" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="Z/vebjO+D47qolo/1DxcycKAovH+7SYW011YJYqneTUJuDlAYBtlLWYLbUZ21L5Bda1blAN1kf/g0rSd32tETg==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar payolitec/Livesession3Assignment"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-0.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14l4.33-2.33 4.33 2.33L10.4 9.26 14 6z"></path></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/payolitec/Livesession3Assignment/stargazers">
          0
        </a>
</form>
    <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/payolitec/Livesession3Assignment/star" class="unstarred" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="BiUA14KbcL+QgUxnRJmaA7iAveEzT/5IAW/TJL9cPb7hQpqhr9V5hE7VSZ7pi7A7kYDT88yi//F4hcd8Vf5PTw==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star payolitec/Livesession3Assignment"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-0.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14l4.33-2.33 4.33 2.33L10.4 9.26 14 6z"></path></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/payolitec/Livesession3Assignment/stargazers">
          0
        </a>
</form>  </div>

  </li>

  <li>
          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/payolitec/Livesession3Assignment/fork" class="btn-with-count" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="tQrgP8slP/QQ0i8nD23XGJfQImYNDhvNcI6aifuQN+lTg9sERxVnxDOqF2+RQTJGkxoraykuhhpr+F3LFjLbVQ==" /></div>
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of payolitec/Livesession3Assignment to your account"
                aria-label="Fork your own copy of payolitec/Livesession3Assignment to your account">
              <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path d="M8 1c-1.11 0-2 0.89-2 2 0 0.73 0.41 1.38 1 1.72v1.28L5 8 3 6v-1.28c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2S0 1.89 0 3c0 0.73 0.41 1.38 1 1.72v1.78l3 3v1.78c-0.59 0.34-1 0.98-1 1.72 0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.73-0.41-1.38-1-1.72V9.5l3-3V4.72c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2zM2 4.2c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m3 10c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m3-10c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z"></path></svg>
              Fork
            </button>
</form>
    <a href="/payolitec/Livesession3Assignment/network" class="social-count">
      1
    </a>
  </li>
</ul>

    <h1 class="entry-title public ">
  <svg aria-hidden="true" class="octicon octicon-repo" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M4 9h-1v-1h1v1z m0-3h-1v1h1v-1z m0-2h-1v1h1v-1z m0-2h-1v1h1v-1z m8-1v12c0 0.55-0.45 1-1 1H6v2l-1.5-1.5-1.5 1.5V14H1c-0.55 0-1-0.45-1-1V1C0 0.45 0.45 0 1 0h10c0.55 0 1 0.45 1 1z m-1 10H1v2h2v-1h3v1h5V11z m0-10H2v9h9V1z"></path></svg>
  <span class="author" itemprop="author"><a href="/payolitec" class="url fn" rel="author">payolitec</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/payolitec/Livesession3Assignment" data-pjax="#js-repo-pjax-container">Livesession3Assignment</a></strong>

</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/payolitec/Livesession3Assignment" aria-selected="true" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /payolitec/Livesession3Assignment" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M9.5 3l-1.5 1.5 3.5 3.5L8 11.5l1.5 1.5 4.5-5L9.5 3zM4.5 3L0 8l4.5 5 1.5-1.5L2.5 8l3.5-3.5L4.5 3z"></path></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a href="/payolitec/Livesession3Assignment/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /payolitec/Livesession3Assignment/issues" itemprop="url">
        <svg aria-hidden="true" class="octicon octicon-issue-opened" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7S10.14 13.7 7 13.7 1.3 11.14 1.3 8s2.56-5.7 5.7-5.7m0-1.3C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7S10.86 1 7 1z m1 3H6v5h2V4z m0 6H6v2h2V10z"></path></svg>
        <span itemprop="name">Issues</span>
        <span class="counter">0</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/payolitec/Livesession3Assignment/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /payolitec/Livesession3Assignment/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 11.28c0-1.73 0-6.28 0-6.28-0.03-0.78-0.34-1.47-0.94-2.06s-1.28-0.91-2.06-0.94c0 0-1.02 0-1 0V0L4 3l3 3V4h1c0.27 0.02 0.48 0.11 0.69 0.31s0.3 0.42 0.31 0.69v6.28c-0.59 0.34-1 0.98-1 1.72 0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.73-0.41-1.38-1-1.72z m-1 2.92c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2zM4 3c0-1.11-0.89-2-2-2S0 1.89 0 3c0 0.73 0.41 1.38 1 1.72 0 1.55 0 5.56 0 6.56-0.59 0.34-1 0.98-1 1.72 0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.73-0.41-1.38-1-1.72V4.72c0.59-0.34 1-0.98 1-1.72z m-0.8 10c0 0.66-0.55 1.2-1.2 1.2s-1.2-0.55-1.2-1.2 0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2z m-1.2-8.8c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z"></path></svg>
      <span itemprop="name">Pull requests</span>
      <span class="counter">0</span>
      <meta itemprop="position" content="3">
</a>  </span>

    <a href="/payolitec/Livesession3Assignment/wiki" class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /payolitec/Livesession3Assignment/wiki">
      <svg aria-hidden="true" class="octicon octicon-book" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M2 5h4v1H2v-1z m0 3h4v-1H2v1z m0 2h4v-1H2v1z m11-5H9v1h4v-1z m0 2H9v1h4v-1z m0 2H9v1h4v-1z m2-6v9c0 0.55-0.45 1-1 1H8.5l-1 1-1-1H1c-0.55 0-1-0.45-1-1V3c0-0.55 0.45-1 1-1h5.5l1 1 1-1h5.5c0.55 0 1 0.45 1 1z m-8 0.5l-0.5-0.5H1v9h6V3.5z m7-0.5H8.5l-0.5 0.5v8.5h6V3z"></path></svg>
      Wiki
</a>

  <a href="/payolitec/Livesession3Assignment/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /payolitec/Livesession3Assignment/pulse">
    <svg aria-hidden="true" class="octicon octicon-pulse" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0V10h3.6L4.5 8.2l0.9 5.4L9 8.5l1.6 1.5H14V8H11.5z"></path></svg>
    Pulse
</a>
  <a href="/payolitec/Livesession3Assignment/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /payolitec/Livesession3Assignment/graphs">
    <svg aria-hidden="true" class="octicon octicon-graph" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M16 14v1H0V0h1v14h15z m-11-1H3V8h2v5z m4 0H7V3h2v10z m4 0H11V6h2v7z"></path></svg>
    Graphs
</a>
    <a href="/payolitec/Livesession3Assignment/settings" class="js-selected-navigation-item reponav-item" data-selected-links="repo_settings repo_branch_settings hooks /payolitec/Livesession3Assignment/settings">
      <svg aria-hidden="true" class="octicon octicon-gear" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 8.77V7.17l-1.94-0.64-0.45-1.09 0.88-1.84-1.13-1.13-1.81 0.91-1.09-0.45-0.69-1.92H6.17l-0.63 1.94-1.11 0.45-1.84-0.88-1.13 1.13 0.91 1.81-0.45 1.09L0 7.23v1.59l1.94 0.64 0.45 1.09-0.88 1.84 1.13 1.13 1.81-0.91 1.09 0.45 0.69 1.92h1.59l0.63-1.94 1.11-0.45 1.84 0.88 1.13-1.13-0.92-1.81 0.47-1.09 1.92-0.69zM7 11c-1.66 0-3-1.34-3-3s1.34-3 3-3 3 1.34 3 3-1.34 3-3 3z"></path></svg>
      Settings
</a>
</nav>

  </div>
</div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/payolitec/Livesession3Assignment/blob/958d927268dac0018a3889affbc02ed2d8c9a903/Paper/Rollingsales_loadandclean.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:744ba64a586d906406ab7fede2a467e9 -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu branch-select-menu js-menu-container js-select-menu left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    title="master"
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Find or create a branch…" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Find or create a branch…">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Find or create a branch…" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/payolitec/Livesession3Assignment/blob/master/Paper/Rollingsales_loadandclean.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text" title="master">
                master
              </span>
            </a>
        </div>

          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/payolitec/Livesession3Assignment/branches" class="js-create-branch select-menu-item select-menu-new-item-form js-navigation-item js-new-item-form" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="SnTNhfsk74SYdJFfUuQuRuE0f+zwVB3uv0pexBbMcbshZQ//GXjgjGH85CR+HiGyJ4yi72RTP51V3XDniPPomg==" /></div>
          <svg aria-hidden="true" class="octicon octicon-git-branch select-menu-item-icon" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path d="M10 5c0-1.11-0.89-2-2-2s-2 0.89-2 2c0 0.73 0.41 1.38 1 1.72v0.3c-0.02 0.52-0.23 0.98-0.63 1.38s-0.86 0.61-1.38 0.63c-0.83 0.02-1.48 0.16-2 0.45V4.72c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2S0 1.89 0 3c0 0.73 0.41 1.38 1 1.72v6.56C0.41 11.63 0 12.27 0 13c0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.53-0.2-1-0.53-1.36 0.09-0.06 0.48-0.41 0.59-0.47 0.25-0.11 0.56-0.17 0.94-0.17 1.05-0.05 1.95-0.45 2.75-1.25s1.2-1.98 1.25-3.02h-0.02c0.61-0.36 1.02-1 1.02-1.73zM2 1.8c0.66 0 1.2 0.55 1.2 1.2s-0.55 1.2-1.2 1.2-1.2-0.55-1.2-1.2 0.55-1.2 1.2-1.2z m0 12.41c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m6-8c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z"></path></svg>
            <div class="select-menu-item-text">
              <span class="select-menu-item-heading">Create branch: <span class="js-new-item-name"></span></span>
              <span class="description">from ‘master’</span>
            </div>
            <input type="hidden" name="name" id="name" class="js-new-item-value">
            <input type="hidden" name="branch" id="branch" value="master">
            <input type="hidden" name="path" id="path" value="Paper/Rollingsales_loadandclean.md">
</form>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="btn-group right">
    <a href="/payolitec/Livesession3Assignment/find/master"
          class="js-pjax-capture-input btn btn-sm"
          data-pjax
          data-hotkey="t">
      Find file
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
  </div>
  <div class="breadcrumb js-zeroclipboard-target">
    <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/payolitec/Livesession3Assignment"><span>Livesession3Assignment</span></a></span></span><span class="separator">/</span><span class="js-path-segment"><a href="/payolitec/Livesession3Assignment/tree/master/Paper"><span>Paper</span></a></span><span class="separator">/</span><strong class="final-path">Rollingsales_loadandclean.md</strong>
  </div>
</div>


  <div class="commit-tease">
      <span class="right">
        <a class="commit-tease-sha" href="/payolitec/Livesession3Assignment/commit/4929b9c6516990e5ad2a908a64f8fab1016427f0" data-pjax>
          4929b9c
        </a>
        <relative-time datetime="2016-06-02T05:24:13Z">Jun 2, 2016</relative-time>
      </span>
      <div>
        <img alt="@eshaw1" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/19526170?v=3&amp;s=40" width="20" />
        <a href="/eshaw1" class="user-mention" rel="contributor">eshaw1</a>
          <a href="/payolitec/Livesession3Assignment/commit/4929b9c6516990e5ad2a908a64f8fab1016427f0" class="message" data-pjax="true" title="Update and rename Rollingsales.md to Rollingsales_loadandclean.md

All,

Here are changes to the &quot;Rollingsales.md&quot; file that should be included in the &quot;Data Directory&quot;. I&#39;ve also proposed a rename of the file to &quot;Rollingsales_loadandclean&quot;.">Update and rename Rollingsales.md to Rollingsales_loadandclean.md</a>
      </div>

    <div class="commit-tease-contributors">
      <button type="button" class="btn-link muted-link contributors-toggle" data-facebox="#blob_contributors_box">
        <strong>1</strong>
         contributor
      </button>
      
    </div>

    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@eshaw1" height="24" src="https://avatars2.githubusercontent.com/u/19526170?v=3&amp;s=48" width="24" />
            <a href="/eshaw1">eshaw1</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="btn-group">
      <a href="/payolitec/Livesession3Assignment/raw/master/Paper/Rollingsales_loadandclean.md" class="btn btn-sm " id="raw-url">Raw</a>
        <a href="/payolitec/Livesession3Assignment/blame/master/Paper/Rollingsales_loadandclean.md" class="btn btn-sm js-update-url-with-hash">Blame</a>
      <a href="/payolitec/Livesession3Assignment/commits/master/Paper/Rollingsales_loadandclean.md" class="btn btn-sm " rel="nofollow">History</a>
    </div>


        <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/payolitec/Livesession3Assignment/edit/master/Paper/Rollingsales_loadandclean.md" class="inline-form js-update-url-with-hash" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="XwtEW/74AlfEthG+nXZ5UAqlqxemv9r4iumdadS1C5PXN2w1E7sAQVb8Lbht6edX6lgCEyPKccr8q9VB40Hb1Q==" /></div>
          <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
            aria-label="Edit this file" data-hotkey="e" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-pencil" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path d="M0 12v3h3l8-8-3-3L0 12z m3 2H1V12h1v1h1v1z m10.3-9.3l-1.3 1.3-3-3 1.3-1.3c0.39-0.39 1.02-0.39 1.41 0l1.59 1.59c0.39 0.39 0.39 1.02 0 1.41z"></path></svg>
          </button>
</form>        <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/payolitec/Livesession3Assignment/delete/master/Paper/Rollingsales_loadandclean.md" class="inline-form" data-form-nonce="ced11c618cf7fa0d7b8252e0c34a61464cf699dd" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="6cyBuqo5SQAEE3rgiEMFs3Yqc/+rbYZBu4UhIBTT7z2KA/vgx/ZSYMJBL6rI8IWlD6UguJgrz9QL+k0885fvsQ==" /></div>
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Delete this file" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M10 2H8c0-0.55-0.45-1-1-1H4c-0.55 0-1 0.45-1 1H1c-0.55 0-1 0.45-1 1v1c0 0.55 0.45 1 1 1v9c0 0.55 0.45 1 1 1h7c0.55 0 1-0.45 1-1V5c0.55 0 1-0.45 1-1v-1c0-0.55-0.45-1-1-1z m-1 12H2V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9z m1-10H1v-1h9v1z"></path></svg>
          </button>
</form>  </div>

  <div class="file-info">
      297 lines (250 sloc)
      <span class="file-info-divider"></span>
    12.2 KB
  </div>
</div>

  
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-rollingsales" class="anchor" href="#rollingsales" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>RollingSales</h1>

<p>Andrew Abbott, Ken Avery, Paola Leon, Earl Shaw<br>
May 30, 2016  </p>

<div class="highlight highlight-source-r"><pre>setwd(<span class="pl-s"><span class="pl-pds">"</span>/Users/Abbott/test-repo/RollingSales<span class="pl-pds">"</span></span>)</pre></div>

<h1><a id="user-content-save-the-file-as-a-csv-and-use-readcsv" class="anchor" href="#save-the-file-as-a-csv-and-use-readcsv" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Save the file as a csv and use read.csv</h1>

<div class="highlight highlight-source-r"><pre><span class="pl-smi">queens</span> <span class="pl-k">&lt;-</span> read.csv(<span class="pl-s"><span class="pl-pds">"</span>rollingsales_queens.csv<span class="pl-pds">"</span></span>,<span class="pl-v">skip</span><span class="pl-k">=</span><span class="pl-c1">4</span>,<span class="pl-v">header</span><span class="pl-k">=</span><span class="pl-c1">TRUE</span>)</pre></div>

<h2><a id="user-content-check-the-data" class="anchor" href="#check-the-data" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Check the data</h2>

<div class="highlight highlight-source-r"><pre>head(<span class="pl-smi">queens</span>)</pre></div>

<pre><code>##   BOROUGH              NEIGHBORHOOD
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
</code></pre>

<div class="highlight highlight-source-r"><pre>summary(<span class="pl-smi">queens</span>)</pre></div>

<pre><code>##     BOROUGH                     NEIGHBORHOOD  
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
</code></pre>

<div class="highlight highlight-source-r"><pre>str(<span class="pl-smi">queens</span>)</pre></div>

<pre><code>## 'data.frame':    25124 obs. of  21 variables:
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
</code></pre>

<h1><a id="user-content-we-create-a-new-variable-that-is-a-clean-version-of-saleprice" class="anchor" href="#we-create-a-new-variable-that-is-a-clean-version-of-saleprice" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>We create a new variable that is a "clean" version of sale.price.</h1>

<h1><a id="user-content-salepricen-is-numeric-not-a-factor" class="anchor" href="#salepricen-is-numeric-not-a-factor" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>sale.price.n is numeric, not a factor.</h1>

<div class="highlight highlight-source-r"><pre>library(<span class="pl-smi">plyr</span>)
<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">SALE.PRICE.N</span> <span class="pl-k">&lt;-</span> as.numeric(gsub(<span class="pl-s"><span class="pl-pds">"</span>[^[:digit:]]<span class="pl-pds">"</span></span>,<span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>, <span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">SALE.PRICE</span>))
count(is.na(<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">SALE.PRICE.N</span>))</pre></div>

<pre><code>##       x  freq
## 1 FALSE 17636
## 2  TRUE  7488
</code></pre>

<p>There are 7,488 without values.</p>

<h1><a id="user-content-make-all-variable-names-lower-case" class="anchor" href="#make-all-variable-names-lower-case" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Make all variable names lower case</h1>

<div class="highlight highlight-source-r"><pre>names(<span class="pl-smi">queens</span>) <span class="pl-k">&lt;-</span> tolower(names(<span class="pl-smi">queens</span>)) 
names(<span class="pl-smi">queens</span>)</pre></div>

<pre><code>##  [1] "borough"                        "neighborhood"                  
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
</code></pre>

<h2><a id="user-content-get-rid-of-leading-digits-and-make-sure-numeric" class="anchor" href="#get-rid-of-leading-digits-and-make-sure-numeric" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Get rid of leading digits and make sure numeric</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">gross.sqft</span> <span class="pl-k">&lt;-</span> as.numeric(gsub(<span class="pl-s"><span class="pl-pds">"</span>[^[:digit:]]<span class="pl-pds">"</span></span>,<span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>, <span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">gross.square.feet</span>))
<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">land.sqft</span> <span class="pl-k">&lt;-</span> as.numeric(gsub(<span class="pl-s"><span class="pl-pds">"</span>[^[:digit:]]<span class="pl-pds">"</span></span>,<span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>, <span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">land.square.feet</span>))
class(<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">gross.sqft</span>)</pre></div>

<pre><code>## [1] "numeric"
</code></pre>

<div class="highlight highlight-source-r"><pre>class(<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">land.sqft</span>)</pre></div>

<pre><code>## [1] "numeric"
</code></pre>

<h2><a id="user-content-change-saledate-to-date-format-in-r-format-must-be-specified" class="anchor" href="#change-saledate-to-date-format-in-r-format-must-be-specified" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Change sale.date to Date format in R, format must be specified.</h2>

<div class="highlight highlight-source-r"><pre><span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">sale.date</span> <span class="pl-k">&lt;-</span> as.Date(<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">sale.date</span>, <span class="pl-s"><span class="pl-pds">"</span>%m/%d/%y<span class="pl-pds">"</span></span>)
<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">year.built</span> <span class="pl-k">&lt;-</span> as.numeric(as.character(<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">year.built</span>))
class(<span class="pl-smi">queens</span><span class="pl-k">$</span><span class="pl-smi">sale.date</span>)</pre></div>

<pre><code>## [1] "Date"
</code></pre>

<h2><a id="user-content-do-a-bit-of-exploration-to-make-sure-theres-not-anything" class="anchor" href="#do-a-bit-of-exploration-to-make-sure-theres-not-anything" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Do a bit of exploration to make sure there's not anything</h2>

<h2><a id="user-content-weird-going-on-with-sale-prices" class="anchor" href="#weird-going-on-with-sale-prices" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>weird going on with sale prices</h2>

<div class="highlight highlight-source-r"><pre>attach(<span class="pl-smi">queens</span>)
hist(<span class="pl-smi">sale.price.n</span>) </pre></div>

<p><a href="/payolitec/Livesession3Assignment/blob/master/Paper/Rollingsales_files/figure-html/unnamed-chunk-8-1.png" target="_blank"><img src="/payolitec/Livesession3Assignment/raw/master/Paper/Rollingsales_files/figure-html/unnamed-chunk-8-1.png" alt="" style="max-width:100%;"></a>&lt;!-- --&gt;</p>

<h1><a id="user-content-everything-looks-to-be-0" class="anchor" href="#everything-looks-to-be-0" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Everything looks to be 0</h1>

<div class="highlight highlight-source-r"><pre>hist(<span class="pl-smi">sale.price.n</span>[<span class="pl-smi">sale.price.n</span><span class="pl-k">&gt;</span><span class="pl-c1">0</span>])</pre></div>

<p><a href="/payolitec/Livesession3Assignment/blob/master/Paper/Rollingsales_files/figure-html/unnamed-chunk-9-1.png" target="_blank"><img src="/payolitec/Livesession3Assignment/raw/master/Paper/Rollingsales_files/figure-html/unnamed-chunk-9-1.png" alt="" style="max-width:100%;"></a>&lt;!-- --&gt;</p>

<h1><a id="user-content-that-didnt-help" class="anchor" href="#that-didnt-help" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>That didn't help</h1>

<div class="highlight highlight-source-r"><pre>hist(<span class="pl-smi">sale.price.n</span>[<span class="pl-smi">sale.price.n</span><span class="pl-k">&lt;</span><span class="pl-c1">1000000</span>])</pre></div>

<p><a href="/payolitec/Livesession3Assignment/blob/master/Paper/Rollingsales_files/figure-html/unnamed-chunk-10-1.png" target="_blank"><img src="/payolitec/Livesession3Assignment/raw/master/Paper/Rollingsales_files/figure-html/unnamed-chunk-10-1.png" alt="" style="max-width:100%;"></a>&lt;!-- --&gt;</p>

<h1><a id="user-content-that-looks-reasonable" class="anchor" href="#that-looks-reasonable" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>that looks reasonable</h1>

<div class="highlight highlight-source-r"><pre>detach(<span class="pl-smi">queens</span>)</pre></div>

<h2><a id="user-content-now-that-the-data-is-in-correct-formats-and-types-we-will-write-it-to-a-new-csv-file" class="anchor" href="#now-that-the-data-is-in-correct-formats-and-types-we-will-write-it-to-a-new-csv-file" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Now that the data is in correct formats and types we will write it to a new .csv file.</h2>

<div class="highlight highlight-source-r"><pre>write.csv(<span class="pl-smi">queens</span>, <span class="pl-v">file</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>rollingsales_queens2.csv<span class="pl-pds">"</span></span>, )</pre></div>

<h2><a id="user-content-lets-keep-only-the-actual-sales-and-create-a-new-data-frame-to-hold-them" class="anchor" href="#lets-keep-only-the-actual-sales-and-create-a-new-data-frame-to-hold-them" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Lets keep only the actual sales and create a new data frame to hold them.</h2>
</article>
  </div>

</div>

<button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="hidden">Jump to Line</button>
<div id="jump-to-line" style="display:none">
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop"></div>
</div>


    </div>
  </div>

    </div>

        <div class="container site-footer-container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark" title="GitHub">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59 0.4 0.07 0.55-0.17 0.55-0.38 0-0.19-0.01-0.82-0.01-1.49-2.01 0.37-2.53-0.49-2.69-0.94-0.09-0.23-0.48-0.94-0.82-1.13-0.28-0.15-0.68-0.52-0.01-0.53 0.63-0.01 1.08 0.58 1.23 0.82 0.72 1.21 1.87 0.87 2.33 0.66 0.07-0.52 0.28-0.87 0.51-1.07-1.78-0.2-3.64-0.89-3.64-3.95 0-0.87 0.31-1.59 0.82-2.15-0.08-0.2-0.36-1.02 0.08-2.12 0 0 0.67-0.21 2.2 0.82 0.64-0.18 1.32-0.27 2-0.27 0.68 0 1.36 0.09 2 0.27 1.53-1.04 2.2-0.82 2.2-0.82 0.44 1.1 0.16 1.92 0.08 2.12 0.51 0.56 0.82 1.27 0.82 2.15 0 3.07-1.87 3.75-3.65 3.95 0.29 0.25 0.54 0.73 0.54 1.48 0 1.07-0.01 1.93-0.01 2.2 0 0.21 0.15 0.46 0.55 0.38C13.71 14.53 16 11.53 16 8 16 3.58 12.42 0 8 0z"></path></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2016 <span title="0.19502s from github-fe139-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    

    <div id="ajax-error-message" class="ajax-error-message flash flash-error">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15.72 12.5l-6.85-11.98C8.69 0.21 8.36 0.02 8 0.02s-0.69 0.19-0.87 0.5l-6.85 11.98c-0.18 0.31-0.18 0.69 0 1C0.47 13.81 0.8 14 1.15 14h13.7c0.36 0 0.69-0.19 0.86-0.5S15.89 12.81 15.72 12.5zM9 12H7V10h2V12zM9 9H7V5h2V9z"></path></svg>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
      </button>
      Something went wrong with that request. Please try again.
    </div>


      
      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-b801b4f0918b70f4a3a4105efbf8e5c567b4b12e41a263b4805397c93aebf317.js"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-9e11266e9840a1629501dc03630329cc0bd58efc0dcfcc89a16868ba1d5c1465.js"></script>
      
      
      
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner hidden">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15.72 12.5l-6.85-11.98C8.69 0.21 8.36 0.02 8 0.02s-0.69 0.19-0.87 0.5l-6.85 11.98c-0.18 0.31-0.18 0.69 0 1C0.47 13.81 0.8 14 1.15 14h13.7c0.36 0 0.69-0.19 0.86-0.5S15.89 12.81 15.72 12.5zM9 12H7V10h2V12zM9 9H7V5h2V9z"></path></svg>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
    <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
    </button>
  </div>
</div>

  </body>
</html>

