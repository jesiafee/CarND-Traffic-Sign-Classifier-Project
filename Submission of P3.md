





<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
  <link rel="dns-prefetch" href="https://assets-cdn.github.com">
  <link rel="dns-prefetch" href="https://avatars0.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars1.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars2.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars3.githubusercontent.com">
  <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
  <link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">



  <link crossorigin="anonymous" media="all" integrity="sha512-Z0JAar9+DkI1NjGVdZr3GivARUgJtA0o2eHlTv7Ou2gshR5awWVf8QGsq11Ns9ZxQLEs+G5/SuARmvpOLMzulw==" rel="stylesheet" href="https://assets-cdn.github.com/assets/frameworks-95aff0b550d3fe338b645a4deebdcb1b.css" />
  <link crossorigin="anonymous" media="all" integrity="sha512-DWgjUOaxSAtMfDQQNpAfTioFKvYEKjXyFv4r5vaYqWMS+NcDGjqOlOfA+qFRG+DjfeVHOLikwZMTYOzcx2R5Ww==" rel="stylesheet" href="https://assets-cdn.github.com/assets/github-5a68a4d0dfbff22a1f6f30a2beb6c6f0.css" />
  
  
  
  

  <meta name="viewport" content="width=device-width">
  
  <title>Udacity-CarND-P3-Traffic-Sign-Classifier/writeup for P3.md at master · Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier</title>
    <meta name="description" content="Contribute to Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier development by creating an account on GitHub.">
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    
    <meta property="og:image" content="https://avatars1.githubusercontent.com/u/41224105?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier" /><meta property="og:url" content="https://github.com/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier" /><meta property="og:description" content="Contribute to Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier development by creating an account on GitHub." />

  <link rel="assets" href="https://assets-cdn.github.com/">
  <link rel="web-socket" href="wss://live.github.com/_sockets/VjI6MzA4MDY3OTA5OjA2YmU5Njk4NDJmODMyMGE3ZmVmNTU5Mzg5MTZjYjhkN2Q3ZDA4ZjJiMjdkYzgyMjU2MjZjZThmYWU5NTA4MDY=--4000cfaf35f27407922a78bddfdd4c1e011b6e52">
  <meta name="pjax-timeout" content="1000">
  <link rel="sudo-modal" href="/sessions/sudo_modal">
  <meta name="request-id" content="C2EA:45D2:1FC34F3:2FE19A8:5B9DBAFF" data-pjax-transient>


  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

      <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
    <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">

  <meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-request_id" content="C2EA:45D2:1FC34F3:2FE19A8:5B9DBAFF" /><meta name="octolytics-dimension-region_edge" content="sea" /><meta name="octolytics-dimension-region_render" content="iad" /><meta name="octolytics-actor-id" content="41224032" /><meta name="octolytics-actor-login" content="jesiafee" /><meta name="octolytics-actor-hash" content="412d28fd54a08551d4843dcb2b08149c5501b284fbec6d54aaa49745fe3f9df1" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />



    <meta name="google-analytics" content="UA-3769691-2">

  <meta class="js-ga-set" name="userId" content="53e2f2fe080735cc683465446342203c" %>

<meta class="js-ga-set" name="dimension1" content="Logged In">



  

      <meta name="hostname" content="github.com">
    <meta name="user-login" content="jesiafee">

      <meta name="expected-hostname" content="github.com">
    <meta name="js-proxy-site-detection-payload" content="MGI2MWIxY2IxN2Y5M2EwY2NiMWMzM2NlMjQ1NjY1ODhiMzJiYTgzM2RiODNjZjVhZmUzMmFjZGVmOWNkMTZiN3x7InJlbW90ZV9hZGRyZXNzIjoiMTk4LjEzLjQ4LjYxIiwicmVxdWVzdF9pZCI6IkMyRUE6NDVEMjoxRkMzNEYzOjJGRTE5QTg6NUI5REJBRkYiLCJ0aW1lc3RhbXAiOjE1MzcwNjM2ODksImhvc3QiOiJnaXRodWIuY29tIn0=">

    <meta name="enabled-features" content="DASHBOARD_V2_LAYOUT_OPT_IN,EXPLORE_DISCOVER_REPOSITORIES,UNIVERSE_BANNER,FREE_TRIALS,MARKETPLACE_INSIGHTS,MARKETPLACE_DOCKERFILE_CI_CTA,MARKETPLACE_PLAN_RESTRICTION_EDITOR,MARKETPLACE_SEARCH,MARKETPLACE_INSIGHTS_CONVERSION_PERCENTAGES,MARKETPLACE_RETARGETING,QUOTE_MARKDOWN">

  <meta name="html-safe-nonce" content="d3fc4e9eeeeea8b01733adb4b253de0a18bcfd65">

  <meta http-equiv="x-pjax-version" content="fb5562753b4bee45cd182533218d988b">
  

      <link href="https://github.com/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/commits/master.atom" rel="alternate" title="Recent Commits to Udacity-CarND-P3-Traffic-Sign-Classifier:master" type="application/atom+xml">

  <meta name="go-import" content="github.com/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier git https://github.com/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier.git">

  <meta name="octolytics-dimension-user_id" content="41224105" /><meta name="octolytics-dimension-user_login" content="Sunshine-Sunset" /><meta name="octolytics-dimension-repository_id" content="147989224" /><meta name="octolytics-dimension-repository_nwo" content="Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="false" /><meta name="octolytics-dimension-repository_network_root_id" content="147989224" /><meta name="octolytics-dimension-repository_network_root_nwo" content="Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier" /><meta name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" content="true" />


    <link rel="canonical" href="https://github.com/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/blob/master/writeup%20for%20P3.md" data-pjax-transient>


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#000000">
  <link rel="icon" type="image/x-icon" class="js-site-favicon" href="https://assets-cdn.github.com/favicon.ico">

<meta name="theme-color" content="#1e2327">


  <meta name="u2f-support" content="true">

  <link rel="manifest" href="/manifest.json" crossOrigin="use-credentials">

  </head>

  <body class="logged-in env-production page-blob">
    

  <div class="position-relative js-header-wrapper ">
    <a href="#start-of-content" tabindex="1" class="p-3 bg-blue text-white show-on-focus js-skip-to-content">Skip to content</a>
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>

    
    
    



        
<header class="Header  f5" role="banner">
  <div class="d-flex flex-justify-between px-3 ">
    <div class="d-flex flex-justify-between ">
      <div class="">
        <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <svg height="32" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>

      </div>

    </div>

    <div class="HeaderMenu d-flex flex-justify-between flex-auto">
      <div class="d-flex">
            <div class="">
              <div class="header-search scoped-search site-scoped-search js-site-search position-relative js-jump-to"
  role="combobox"
  aria-owns="jump-to-results"
  aria-label="Search or jump to"
  aria-haspopup="listbox"
  aria-expanded="false"
>
  <div class="position-relative">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-site-search-form" data-scope-type="Repository" data-scope-id="147989224" data-scoped-search-url="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/search" data-unscoped-search-url="/search" action="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/search" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
      <label class="form-control header-search-wrapper header-search-wrapper-jump-to position-relative d-flex flex-justify-between flex-items-center js-chromeless-input-container">
        <input type="text"
          class="form-control header-search-input jump-to-field js-jump-to-field js-site-search-focus js-site-search-field is-clearable"
          data-hotkey="s,/"
          name="q"
          value=""
          placeholder="Search or jump to…"
          data-unscoped-placeholder="Search or jump to…"
          data-scoped-placeholder="Search or jump to…"
          autocapitalize="off"
          aria-autocomplete="list"
          aria-controls="jump-to-results"
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations#csrf-token=Wqz6Gf6NKLZdNkzU3zipa1mI3SHVwgptkMelZRdjLbqKeMZoa2/P+7onKULJCNs8dUwy9wgsQWgB58FdbExv9w=="
          spellcheck="false"
          autocomplete="off"
          >
          <input type="hidden" class="js-site-search-type-field" name="type" >
            <img src="https://assets-cdn.github.com/images/search-shortcut-hint.svg" alt="" class="mr-2 header-search-key-slash">

            <div class="Box position-absolute overflow-hidden d-none jump-to-suggestions js-jump-to-suggestions-container">
              <ul class="d-none js-jump-to-suggestions-template-container">
                <li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item" role="option">
                  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center p-2 jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open" href="">
                    <div class="jump-to-octicon js-jump-to-octicon mr-2 text-center d-none">
                      <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-octicon-repo d-none" title="Repository" aria-label="Repository" viewBox="0 0 12 16" version="1.1" role="img"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
                      <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-octicon-project d-none" title="Project" aria-label="Project" viewBox="0 0 15 16" version="1.1" role="img"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
                      <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-octicon-search d-none" title="Search" aria-label="Search" viewBox="0 0 16 16" version="1.1" role="img"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
                    </div>

                    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

                    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
                    </div>

                    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none js-jump-to-badge-search">
                      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
                        In this repository
                      </span>
                      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
                        All GitHub
                      </span>
                      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
                    </div>

                    <div aria-hidden="true" class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
                      Jump to
                      <span class="d-inline-block ml-1 v-align-middle">↵</span>
                    </div>
                  </a>
                </li>
              </ul>
              <ul class="d-none js-jump-to-no-results-template-container">
                <li class="d-flex flex-justify-center flex-items-center p-3 f5 d-none">
                  <span class="text-gray">No suggested jump to results</span>
                </li>
              </ul>

              <ul id="jump-to-results" role="listbox" class="js-navigation-container jump-to-suggestions-results-container js-jump-to-suggestions-results-container" >
                <li class="d-flex flex-justify-center flex-items-center p-0 f5">
                  <img src="https://assets-cdn.github.com/images/spinners/octocat-spinner-128.gif" alt="Octocat Spinner Icon" class="m-2" width="28">
                </li>
              </ul>
            </div>
      </label>
</form>  </div>
</div>

            </div>

          <ul class="d-flex pl-2 flex-items-center text-bold list-style-none" role="navigation">
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-hotkey="g p" data-ga-click="Header, click, Nav menu - item:pulls context:user" aria-label="Pull requests you created" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls" href="/pulls">
                Pull requests
</a>            </li>
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-hotkey="g i" data-ga-click="Header, click, Nav menu - item:issues context:user" aria-label="Issues you created" data-selected-links="/issues /issues/assigned /issues/mentioned /issues" href="/issues">
                Issues
</a>            </li>
              <li>
                <a class="js-selected-navigation-item HeaderNavlink px-2" data-ga-click="Header, click, Nav menu - item:marketplace context:user" data-octo-click="marketplace_click" data-octo-dimensions="location:nav_bar" data-selected-links=" /marketplace" href="/marketplace">
                   Marketplace
</a>              </li>
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-ga-click="Header, click, Nav menu - item:explore" data-selected-links="/explore /trending /trending/developers /integrations /integrations/feature/code /integrations/feature/collaborate /integrations/feature/ship showcases showcases_search showcases_landing /explore" href="/explore">
                Explore
</a>            </li>
          </ul>
      </div>

      <div class="d-flex">
        
<ul class="user-nav d-flex flex-items-center list-style-none" id="user-links">
  <li class="dropdown">
    <span class="d-inline-block  px-2">
      
    <a aria-label="You have no unread notifications" class="notification-indicator tooltipped tooltipped-s  js-socket-channel js-notification-indicator" data-hotkey="g n" data-ga-click="Header, go to notifications, icon:read" data-channel="notification-changed:41224032" href="/notifications">
        <span class="mail-status "></span>
        <svg class="octicon octicon-bell" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M13.99 11.991v1H0v-1l.73-.58c.769-.769.809-2.547 1.189-4.416.77-3.767 4.077-4.996 4.077-4.996 0-.55.45-1 .999-1 .55 0 1 .45 1 1 0 0 3.387 1.229 4.156 4.996.38 1.879.42 3.657 1.19 4.417l.659.58h-.01zM6.995 15.99c1.11 0 1.999-.89 1.999-1.999H4.996c0 1.11.89 1.999 1.999 1.999z"/></svg>
</a>
    </span>
  </li>

  <li class="dropdown">
    <details class="details-overlay details-reset d-flex px-2 flex-items-center">
      <summary class="HeaderNavlink"
         aria-label="Create new…"
         data-ga-click="Header, create new, icon:add">
        <svg class="octicon octicon-plus float-left mr-1 mt-1" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 9H7v5H5V9H0V7h5V2h2v5h5v2z"/></svg>
        <span class="dropdown-caret mt-1"></span>
      </summary>
      <details-menu class="dropdown-menu dropdown-menu-sw">
        
<a role="menuitem" class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>

  <a role="menuitem" class="dropdown-item" href="/new/import" data-ga-click="Header, import a repository">
    Import repository
  </a>

<a role="menuitem" class="dropdown-item" href="https://gist.github.com/" data-ga-click="Header, create new gist">
  New gist
</a>

  <a role="menuitem" class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>


  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier">This repository</span>
  </div>
    <a role="menuitem" class="dropdown-item" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/issues/new" data-ga-click="Header, create new issue">
      New issue
    </a>

      </details-menu>
    </details>
  </li>

  <li class="dropdown">

    <details class="details-overlay details-reset d-flex pl-2 flex-items-center">
      <summary class="HeaderNavlink name mt-1"
        aria-label="View profile and more"
        data-ga-click="Header, show menu, icon:avatar">
        <img alt="@jesiafee" class="avatar float-left mr-1" src="https://avatars1.githubusercontent.com/u/41224032?s=40&amp;v=4" height="20" width="20">
        <span class="dropdown-caret"></span>
      </summary>
      <details-menu class="dropdown-menu dropdown-menu-sw">
        <ul>
          <li class="header-nav-current-user css-truncate"><a role="menuitem" class="no-underline user-profile-link px-3 pt-2 pb-2 mb-n2 mt-n1 d-block" href="/jesiafee" data-ga-click="Header, go to profile, text:Signed in as">Signed in as <strong class="css-truncate-target">jesiafee</strong></a></li>
          <li class="dropdown-divider"></li>
          <li><a role="menuitem" class="dropdown-item" href="/jesiafee" data-ga-click="Header, go to profile, text:your profile">Your profile</a></li>
          <li><a role="menuitem" class="dropdown-item" href="/jesiafee?tab=repositories" data-ga-click="Header, go to repositories, text:your repositories">Your repositories</a></li>
          <li><a role="menuitem" class="dropdown-item" href="/jesiafee?tab=stars" data-ga-click="Header, go to starred repos, text:your stars">Your stars</a></li>
            <li><a role="menuitem" class="dropdown-item" href="https://gist.github.com/" data-ga-click="Header, your gists, text:your gists">Your gists</a></li>
          <li class="dropdown-divider"></li>
          <li><a role="menuitem" class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a></li>
          <li><a role="menuitem" class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">Settings</a></li>
          <li>
            <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="logout-form" action="/logout" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="gMfx0YNy7rMvgoEUTPRD4lj+psAQqWlEMRvjpafBjX/5jzrCAcXx2ZZ3uZ2Lt7b13qjIvwqdqqWvqzPjUK8UDw==" />
              <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout" role="menuitem">
                Sign out
              </button>
</form>          </li>
        </ul>
      </details-menu>
    </details>
  </li>
</ul>



        <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="sr-only right-0" action="/logout" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="h1kKaHYyVhau5UPhmNE4TvvPjPdNPMtFpI7chH/4aUz+EcF79IVJfBcQe2hfks1ZfZniiFcICKQ6PgzCiJbwPA==" />
          <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
            Sign out
          </button>
</form>      </div>
    </div>
  </div>
</header>

      

  </div>

  <div id="start-of-content" class="show-on-focus"></div>

    <div id="js-flash-container">


</div>



  <div role="main" class="application-main ">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode" class="">
    <div id="js-repo-pjax-container" data-pjax-container >
      





  



  <div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav  ">
    <div class="repohead-details-container clearfix container">

      <ul class="pagehead-actions">
  <li>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form data-autosubmit="true" data-remote="true" class="js-social-container" action="/notifications/subscribe" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="ImWYCpuaW10uhteJMU+1pIkZznWY218k3TbiP2cYMdKQAU3ggLiiNwl8mtwmodKSuI9TfKA9KGQmieZ+OBUKcg==" />      <input type="hidden" name="repository_id" id="repository_id" value="147989224" class="form-control" />

        <div class="select-menu js-menu-container js-select-menu">
          <a href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/subscription"
            class="btn btn-sm btn-with-count select-menu-button js-menu-target"
            role="button"
            aria-haspopup="true"
            aria-expanded="false"
            aria-label="Toggle repository notifications menu"
            data-ga-click="Repository, click Watch settings, action:blob#show">
            <span class="js-select-button">
                <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                Watch
            </span>
          </a>
          <a class="social-count js-social-count"
            href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/watchers"
            aria-label="0 users are watching this repository">
            0
          </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content">
            <div class="select-menu-header js-navigation-enable" tabindex="-1">
              <svg class="octicon octicon-x js-menu-close" role="img" aria-label="Close" viewBox="0 0 12 16" version="1.1" width="12" height="16"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
              <span class="select-menu-title">Notifications</span>
            </div>

              <div class="select-menu-list js-navigation-container" role="menu">

                <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                  <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
                  <div class="select-menu-item-text">
                    <input type="radio" name="do" id="do_included" value="included" checked="checked" />
                    <span class="select-menu-item-heading">Not watching</span>
                    <span class="description">Be notified when participating or @mentioned.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                      Watch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
                  <div class="select-menu-item-text">
                    <input type="radio" name="do" id="do_subscribed" value="subscribed" />
                    <span class="select-menu-item-heading">Watching</span>
                    <span class="description">Be notified of all conversations.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                        Unwatch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
                  <div class="select-menu-item-text">
                    <input type="radio" name="do" id="do_ignore" value="ignore" />
                    <span class="select-menu-item-heading">Ignoring</span>
                    <span class="description">Never be notified.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg class="octicon octicon-mute v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 2.81v10.38c0 .67-.81 1-1.28.53L3 10H1c-.55 0-1-.45-1-1V7c0-.55.45-1 1-1h2l3.72-3.72C7.19 1.81 8 2.14 8 2.81zm7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06L11.44 8 9.47 9.97l1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06L13.56 8l1.97-1.97z"/></svg>
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
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="starred js-social-form" action="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/unstar" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="nB4vUcUoVO2IWZ3ZOOOCUEDI+/2VIy7GaFrtpWuvxZTM4Vu/IQTK4ucsUS3ZnB5310P6NtoAX9HnCz4qg4xWLg==" />
      <input type="hidden" name="context" value="repository"></input>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg class="octicon octicon-star v-align-text-bottom" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/stargazers"
           aria-label="0 users starred this repository">
          0
        </a>
</form>
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="unstarred js-social-form" action="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/star" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="RAHDmoGi4XtpfHqOtdOWSICC5BzPFzvjAE5c2+L3ieXqxvojNO64TKZweMZjdZCy+cpc5Wi2xNiLb0eSDZ6AGw==" />
      <input type="hidden" name="context" value="repository"></input>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg class="octicon octicon-star v-align-text-bottom" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/stargazers"
           aria-label="0 users starred this repository">
          0
        </a>
</form>  </div>

  </li>

  <li>
          <details class="details-reset details-overlay details-overlay-dark d-inline-block float-left"
            data-deferred-details-content-url="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/fork?fragment=1">
            <summary class="btn btn-sm btn-with-count"
              title="Fork your own copy of Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier to your account"
              data-ga-click="Repository, show fork modal, action:blob#show; text:Fork">
              <svg class="octicon octicon-repo-forked v-align-text-bottom" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
              Fork
            </summary>
            <details-dialog class="anim-fade-in fast Box Box--overlay d-flex flex-column">
              <div class="Box-header">
                <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog>
                  <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
                </button>
                <h3 class="Box-title">Where should we fork this repository?</h3>
              </div>
              <div class="Box-body overflow-auto text-center">
                <include-fragment>
                  <div class="octocat-spinner my-3" aria-label="Loading..."></div>
                  <p class="f5 text-gray">If this dialog fails to load, you can visit <a href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/fork">the fork page</a> directly.</p>
                </include-fragment>
              </div>
            </details-dialog>
          </details>

    <a href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/network/members" class="social-count"
       aria-label="0 users forked this repository">
      0
    </a>
  </li>
</ul>

      <h1 class="public ">
  <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a class="url fn" rel="author" href="/Sunshine-Sunset">Sunshine-Sunset</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a data-pjax="#js-repo-pjax-container" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier">Udacity-CarND-P3-Traffic-Sign-Classifier</a></strong>

</h1>

    </div>
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax container"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a class="js-selected-navigation-item selected reponav-item" itemprop="url" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier">
      <svg class="octicon octicon-code" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a itemprop="url" data-hotkey="g i" class="js-selected-navigation-item reponav-item" data-selected-links="repo_issues repo_labels repo_milestones /Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/issues" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/issues">
        <svg class="octicon octicon-issue-opened" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg>
        <span itemprop="name">Issues</span>
        <span class="Counter">0</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a data-hotkey="g p" itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/pulls" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/pulls">
      <svg class="octicon octicon-git-pull-request" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="Counter">0</span>
      <meta itemprop="position" content="3">
</a>  </span>

    <a data-hotkey="g b" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/projects" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/projects">
      <svg class="octicon octicon-project" viewBox="0 0 15 16" version="1.1" width="15" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      Projects
      <span class="Counter" >0</span>
</a>

    <a class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/wiki" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/wiki">
      <svg class="octicon octicon-book" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M3 5h4v1H3V5zm0 3h4V7H3v1zm0 2h4V9H3v1zm11-5h-4v1h4V5zm0 2h-4v1h4V7zm0 2h-4v1h4V9zm2-6v9c0 .55-.45 1-1 1H9.5l-1 1-1-1H2c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h5.5l1 1 1-1H15c.55 0 1 .45 1 1zm-8 .5L7.5 3H2v9h6V3.5zm7-.5H9.5l-.5.5V12h6V3z"/></svg>
      Wiki
</a>
  <a class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors dependency_graph pulse /Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/pulse" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/pulse">
    <svg class="octicon octicon-graph" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
    Insights
</a>
    <a class="js-selected-navigation-item reponav-item" data-selected-links="repo_settings repo_branch_settings hooks integration_installations repo_keys_settings issue_template_editor /Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/settings" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/settings">
      <svg class="octicon octicon-gear" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 8.77v-1.6l-1.94-.64-.45-1.09.88-1.84-1.13-1.13-1.81.91-1.09-.45-.69-1.92h-1.6l-.63 1.94-1.11.45-1.84-.88-1.13 1.13.91 1.81-.45 1.09L0 7.23v1.59l1.94.64.45 1.09-.88 1.84 1.13 1.13 1.81-.91 1.09.45.69 1.92h1.59l.63-1.94 1.11-.45 1.84.88 1.13-1.13-.92-1.81.47-1.09L14 8.75v.02zM7 11c-1.66 0-3-1.34-3-3s1.34-3 3-3 3 1.34 3 3-1.34 3-3 3z"/></svg>
      Settings
</a>
</nav>


  </div>

<div class="container new-discussion-timeline experiment-repo-nav  ">
  <div class="repository-content ">

    
  <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/blob/93a333d40d323c6422a69cea132a550bc677b891/writeup%20for%20P3.md">Permalink</a>

  <!-- blob contrib key: blob_contributors:v21:7a02aaf0de7303f958e6a6f2f8a38806 -->

  

  <div class="file-navigation">
    
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class=" btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" aria-expanded="false" aria-haspopup="true">
      <i>Branch:</i>
      <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax>

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg class="octicon octicon-x js-menu-close" role="img" aria-label="Close" viewBox="0 0 12 16" version="1.1" width="12" height="16"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
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
               href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/blob/master/writeup%20for%20P3.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
        </div>

          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="select-menu-new-item-form js-new-item-form" action="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/branches" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="MMrI9IotovomXvxnf58H7s2YhbgaKXeeBllJnrtkZnGfBZQjhSUTcheCukKiG8sXY4qyK5BBZaNEsk5q7O7GlA==" />
            <input type="hidden" name="name" id="name" class="js-new-item-value">
            <input type="hidden" name="branch" id="branch" value="master">
            <input type="hidden" name="path" id="path" value="writeup%20for%20P3.md">

            <button type="submit" class="width-full select-menu-item js-navigation-open js-navigation-item">
              <svg class="octicon octicon-git-branch select-menu-item-icon" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M10 5c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v.3c-.02.52-.23.98-.63 1.38-.4.4-.86.61-1.38.63-.83.02-1.48.16-2 .45V4.72a1.993 1.993 0 0 0-1-3.72C.88 1 0 1.89 0 3a2 2 0 0 0 1 1.72v6.56c-.59.35-1 .99-1 1.72 0 1.11.89 2 2 2 1.11 0 2-.89 2-2 0-.53-.2-1-.53-1.36.09-.06.48-.41.59-.47.25-.11.56-.17.94-.17 1.05-.05 1.95-.45 2.75-1.25S8.95 7.77 9 6.73h-.02C9.59 6.37 10 5.73 10 5zM2 1.8c.66 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2C1.35 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2zm0 12.41c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm6-8c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
              <div class="select-menu-item-text">
                <span class="select-menu-item-heading">Create branch: <span class="js-new-item-name"></span></span>
                <span class="description">from ‘master’</span>
              </div>
            </button>
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

    <div class="BtnGroup float-right">
      <a href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/find/master"
            class="js-pjax-capture-input btn btn-sm BtnGroup-item"
            data-pjax
            data-hotkey="t">
        Find file
      </a>
      <clipboard-copy for="blob-path" class="btn btn-sm BtnGroup-item">
        Copy path
      </clipboard-copy>
    </div>
    <div id="blob-path" class="breadcrumb">
      <span class="repo-root js-repo-root"><span class="js-path-segment"><a data-pjax="true" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier"><span>Udacity-CarND-P3-Traffic-Sign-Classifier</span></a></span></span><span class="separator">/</span><strong class="final-path">writeup for P3.md</strong>
    </div>
  </div>


  
  <div class="commit-tease">
      <span class="float-right">
        <a class="commit-tease-sha" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/commit/93a333d40d323c6422a69cea132a550bc677b891" data-pjax>
          93a333d
        </a>
        <relative-time datetime="2018-09-16T02:07:51Z">Sep 16, 2018</relative-time>
      </span>
      <div>
        <a rel="contributor" data-skip-pjax="true" data-hovercard-user-id="41224032" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/jesiafee"><img class="avatar" src="https://avatars1.githubusercontent.com/u/41224032?s=40&amp;v=4" width="20" height="20" alt="@jesiafee" /></a>
        <a class="user-mention" rel="contributor" data-hovercard-user-id="41224032" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/jesiafee">jesiafee</a>
          <a data-pjax="true" title="Update writeup for P3.md" class="message" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/commit/93a333d40d323c6422a69cea132a550bc677b891">Update writeup for P3.md</a>
      </div>

    <div class="commit-tease-contributors">
      
<details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark float-left mr-2" id="blob_contributors_box">
  <summary class="btn-link" aria-haspopup="dialog"  >
    
    <span><strong>1</strong> contributor</span>
  </summary>
  <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast " aria-label="Users who have contributed to this file">
    <div class="Box-header">
      <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog>
        <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
      </button>
      <h3 class="Box-title">Users who have contributed to this file</h3>
    </div>
    
        <ul class="list-style-none overflow-auto">
            <li class="Box-row">
              <a class="link-gray-dark no-underline" href="/jesiafee">
                <img class="avatar mr-2" alt="" src="https://avatars1.githubusercontent.com/u/41224032?s=40&amp;v=4" width="20" height="20" />
                jesiafee
</a>            </li>
        </ul>

  </details-dialog>
</details>
      
    </div>
  </div>



  <div class="file">
    <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a id="raw-url" class="btn btn-sm BtnGroup-item" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/raw/master/writeup%20for%20P3.md">Raw</a>
        <a class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/blame/master/writeup%20for%20P3.md">Blame</a>
      <a rel="nofollow" class="btn btn-sm BtnGroup-item" href="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/commits/master/writeup%20for%20P3.md">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="x-github-client://openRepo/https://github.com/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier?branch=master&amp;filepath=writeup%20for%20P3.md"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:windows">
            <svg class="octicon octicon-device-desktop" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"/></svg>
        </a>

          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form js-update-url-with-hash" action="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/edit/master/writeup%20for%20P3.md" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="IDM7CUUsbkyYMCS+mphtvdTpU6NNAc5yCmCGjNYlPkC4gKtATGhH91sNRw2YEMlHAkVN7wTcOjloly80wUkEcw==" />
            <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
              aria-label="Edit this file" data-hotkey="e" data-disable-with>
              <svg class="octicon octicon-pencil" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
            </button>
</form>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form" action="/Sunshine-Sunset/Udacity-CarND-P3-Traffic-Sign-Classifier/delete/master/writeup%20for%20P3.md" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="e6UNsg5EED9GCY0a97S892ypK9r1xQ7xRuHEMiTIG8EImm2MdVHtvSlyvt3bR35t3foX2nhCT9gBHWuCtZWPsg==" />
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Delete this file" data-disable-with>
            <svg class="octicon octicon-trashcan" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
          </button>
</form>  </div>

  <div class="file-info">
      239 lines (150 sloc)
      <span class="file-info-divider"></span>
    8.39 KB
  </div>
</div>

    
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-self-driving-car-engineer-nanodegree" class="anchor" aria-hidden="true" href="#self-driving-car-engineer-nanodegree"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Self-Driving Car Engineer Nanodegree</h1>
<h2><a id="user-content-project-build-a-traffic-sign-recognition-classifier" class="anchor" aria-hidden="true" href="#project-build-a-traffic-sign-recognition-classifier"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Project: Build a Traffic Sign Recognition Classifier</h2>
<p>The goals / steps of this project are the following:</p>
<ul>
<li>Load the data set (see below for links to the project data set)</li>
<li>Explore, summarize and visualize the data set</li>
<li>Design, train and test a model architecture</li>
<li>Use the model to make predictions on new images</li>
<li>Analyze the softmax probabilities of the new images</li>
<li>Summarize the results with a written report</li>
</ul>
<p>The general steps are:</p>
<p>0.load the data;</p>
<p>1.dataset summary &amp; exploration</p>
<p>2.design and test a model architecture</p>
<p>3.test a model on new images</p>
<hr>
<h3><a id="user-content-step-0-load-the-data" class="anchor" aria-hidden="true" href="#step-0-load-the-data"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Step 0: Load the Data</h3>
<p>First, I change the directory of the workspace to the root, and find these three items named train.p, valid.p, test.p, respectively.
Then, I print them out and see what type and shape they are.</p>
<p>Current directory is:  /home/workspace/CarND-Traffic-Sign-Classifier-Project</p>
<p>Current directory is:  /home/workspace</p>
<p>X_train:  (34799, 32, 32, 3)  y_train:  (34799,)</p>
<p>X_valid:  (4410, 32, 32, 3)   y_valid:  (4410,)</p>
<p>X_test:   (12630, 32, 32, 3)  y_test:   (12630,)</p>
<h3><a id="user-content-step-1-dataset-summary--exploration" class="anchor" aria-hidden="true" href="#step-1-dataset-summary--exploration"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Step 1: Dataset Summary &amp; Exploration</h3>
<p>The pickled data is a dictionary with 4 key/value pairs:</p>
<ul>
<li><code>'features'</code> is a 4D array containing raw pixel data of the traffic sign images, (num examples, width, height, channels).</li>
<li><code>'labels'</code> is a 1D array containing the label/class id of the traffic sign. The file <code>signnames.csv</code> contains id -&gt; name mappings for each id.</li>
<li><code>'sizes'</code> is a list containing tuples, (width, height) representing the original width and height of the image.</li>
<li><code>'coords'</code> is a list containing tuples, (x1, y1, x2, y2) representing coordinates of a bounding box around the sign in the image. <strong>THESE COORDINATES ASSUME THE ORIGINAL IMAGE. THE PICKLED DATA CONTAINS RESIZED VERSIONS (32 by 32) OF THESE IMAGES</strong></li>
</ul>
<h4><a id="user-content-dataset-summary" class="anchor" aria-hidden="true" href="#dataset-summary"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Dataset Summary</h4>
<p>Number of training examples = 34799</p>
<p>Number of validation examples = 4410</p>
<p>Number of testing examples = 12630</p>
<p>Image data shape = (32, 32, 3)</p>
<p>Number of classes = 43</p>
<h4><a id="user-content-dataset-exploration" class="anchor" aria-hidden="true" href="#dataset-exploration"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Dataset Exploration</h4>
<p>type exploration:</p>
<p>type of train:  &lt;class 'dict'&gt;</p>
<p>dict_keys(['coords', 'labels', 'features', 'sizes'])</p>
<p>the shape of features:
(34799, 32, 32, 3)</p>
<p>the shape of labels:
(34799,)</p>
<p>the shape of sizes:
(34799, 2)</p>
<p>the shape of coords:
(34799, 4)</p>
<p>the csv file:</p>
<p>&lt;class '_csv.reader'&gt;</p>
<p>['ClassId', 'SignName']</p>
<p>['0', 'Speed limit (20km/h)']</p>
<p>['1', 'Speed limit (30km/h)']</p>
<p>['2', 'Speed limit (50km/h)']</p>
<p>['3', 'Speed limit (60km/h)']</p>
<p>...</p>
<p>['42', 'End of no passing by vehicles over 3.5 metric tons']</p>
<p>histogram(show the statistic data of the 3 dataset):</p>
<p>training dataset:
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591687-3cb73600-b98c-11e8-9066-b0f66843700c.png"><img src="https://user-images.githubusercontent.com/41224032/45591687-3cb73600-b98c-11e8-9066-b0f66843700c.png" alt="train" style="max-width:100%;"></a></p>
<p>validation dataset:
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591694-4f316f80-b98c-11e8-865a-e740cf258701.png"><img src="https://user-images.githubusercontent.com/41224032/45591694-4f316f80-b98c-11e8-865a-e740cf258701.png" alt="validation" style="max-width:100%;"></a></p>
<p>test dataset:
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591700-5789aa80-b98c-11e8-9906-647cf5e1789a.png"><img src="https://user-images.githubusercontent.com/41224032/45591700-5789aa80-b98c-11e8-9906-647cf5e1789a.png" alt="test" style="max-width:100%;"></a></p>
<h4><a id="user-content-dataset-visualization" class="anchor" aria-hidden="true" href="#dataset-visualization"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Dataset Visualization</h4>
<p>single image:</p>
<p>For one image of the data:</p>
<p>the original size of the data: [34 37]</p>
<p>the coordiantes: [ 5  6 28 31]</p>
<p>the shape of the iamge: (32, 32, 3)</p>
<p>the label of the image: 38</p>
<p><a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591719-bea75f00-b98c-11e8-9b1d-0fcc00e47dfc.png"><img src="https://user-images.githubusercontent.com/41224032/45591719-bea75f00-b98c-11e8-9b1d-0fcc00e47dfc.png" alt="single image" style="max-width:100%;"></a></p>
<p>the training dataset:</p>
<p><a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591730-01693700-b98d-11e8-8c49-98bb52694378.png"><img src="https://user-images.githubusercontent.com/41224032/45591730-01693700-b98d-11e8-8c49-98bb52694378.png" alt="training dataset" style="max-width:100%;"></a></p>
<h3><a id="user-content-pre-process-the-data-set-normalization-grayscale-etc" class="anchor" aria-hidden="true" href="#pre-process-the-data-set-normalization-grayscale-etc"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Pre-process the Data Set (normalization, grayscale, etc.)</h3>
<p>Here are the comparison of the original image, normalized image and grayscale image:</p>
<p><a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591758-a2f08880-b98d-11e8-9106-4b83b5df4a48.png"><img src="https://user-images.githubusercontent.com/41224032/45591758-a2f08880-b98d-11e8-9106-4b83b5df4a48.png" alt="comparison 1 2 3" style="max-width:100%;"></a></p>
<p>Here is the effect of normalized grayscale image:</p>
<p><a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591782-0e3a5a80-b98e-11e8-86be-5d67f44b315d.png"><img src="https://user-images.githubusercontent.com/41224032/45591782-0e3a5a80-b98e-11e8-86be-5d67f44b315d.png" alt="normalized grayscale image" style="max-width:100%;"></a></p>
<p>The adopted pre-process method is Normalizing the grayscale image.</p>
<p>After pre-processed, the shape of the datasets are:</p>
<p>(34799, 32, 32, 1);</p>
<p>(4410, 32, 32, 1);</p>
<p>(12630, 32, 32, 1).</p>
<h3><a id="user-content-step-2-design-and-test-a-model-architecture" class="anchor" aria-hidden="true" href="#step-2-design-and-test-a-model-architecture"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Step 2: Design and Test a Model Architecture</h3>
<p>In this section, I referred many lines of codes from those in the CNN quiz.</p>
<h3><a id="user-content-model-architecture" class="anchor" aria-hidden="true" href="#model-architecture"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Model Architecture</h3>
<p>My final model consisted of the following layers:</p>
<table>
<thead>
<tr>
<th align="center">Layer</th>
<th align="center">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Input</td>
<td align="center">32x32x1 grayscale image</td>
</tr>
<tr>
<td align="center">Convolution 5x5</td>
<td align="center">1x1 stride, valid padding, outputs 28x28x6</td>
</tr>
<tr>
<td align="center">RELU</td>
<td align="center"></td>
</tr>
<tr>
<td align="center">Max pooling</td>
<td align="center">2x2 stride,  outputs 14x14x6</td>
</tr>
<tr>
<td align="center">Convolution 5x5</td>
<td align="center">1x1 stride, valid padding, outputs 10x10x16</td>
</tr>
<tr>
<td align="center">RELU</td>
<td align="center"></td>
</tr>
<tr>
<td align="center">Max pooling</td>
<td align="center">2x2 stride,  outputs 5x5x16</td>
</tr>
<tr>
<td align="center">Flatten input</td>
<td align="center">outputs 400</td>
</tr>
<tr>
<td align="center">Fully connected</td>
<td align="center">outputs 120</td>
</tr>
<tr>
<td align="center">RELU</td>
<td align="center"></td>
</tr>
<tr>
<td align="center">Dropout</td>
<td align="center">keep_prob = 0.7</td>
</tr>
<tr>
<td align="center">Fully connected</td>
<td align="center">outputs 84</td>
</tr>
<tr>
<td align="center">RELU</td>
<td align="center"></td>
</tr>
<tr>
<td align="center">Dropout</td>
<td align="center">keep_prob = 0.7</td>
</tr>
<tr>
<td align="center">Fully connected</td>
<td align="center">outputs 43</td>
</tr>
<tr>
<td align="center">Softmax</td>
<td align="center">output for calculating cross-entropy</td>
</tr></tbody></table>
<p>First, I shuffle the training dataset.</p>
<p>Then, I set the epochs 80, the batch size 128 by default.</p>
<p>Tuning learning rate is important, because everytime I change it little, the result changes a lot. Finally, I set it 0.00035 here.</p>
<p>My final results are:</p>
<ul>
<li>validation set accuracy of 0.9503</li>
<li>test set accuracy of 0.9368</li>
</ul>
<h3><a id="user-content-step-3-test-a-model-on-new-images" class="anchor" aria-hidden="true" href="#step-3-test-a-model-on-new-images"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Step 3: Test a Model on New Images</h3>
<h4><a id="user-content-load-and-output-the-images" class="anchor" aria-hidden="true" href="#load-and-output-the-images"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Load and Output the Images</h4>
<p>Here are the 6 German traffic signs I found on the web:
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591934-134dd880-b993-11e8-8c35-9772709a18b2.jpg"><img src="https://user-images.githubusercontent.com/41224032/45591934-134dd880-b993-11e8-8c35-9772709a18b2.jpg" alt="image1 8" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591936-19dc5000-b993-11e8-81af-0e07636d8d8f.jpg"><img src="https://user-images.githubusercontent.com/41224032/45591936-19dc5000-b993-11e8-81af-0e07636d8d8f.jpg" alt="image2 33" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591938-1ea10400-b993-11e8-9cf4-cdd3c1aa0e82.jpg"><img src="https://user-images.githubusercontent.com/41224032/45591938-1ea10400-b993-11e8-9cf4-cdd3c1aa0e82.jpg" alt="image3 14" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591939-2365b800-b993-11e8-91d2-46e82fee229f.jpg"><img src="https://user-images.githubusercontent.com/41224032/45591939-2365b800-b993-11e8-91d2-46e82fee229f.jpg" alt="image4 11" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591941-2791d580-b993-11e8-9ba8-60d10daca606.jpg"><img src="https://user-images.githubusercontent.com/41224032/45591941-2791d580-b993-11e8-9ba8-60d10daca606.jpg" alt="image5 4" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591942-2c568980-b993-11e8-97fd-0b263cc3385d.jpg"><img src="https://user-images.githubusercontent.com/41224032/45591942-2c568980-b993-11e8-97fd-0b263cc3385d.jpg" alt="image6 27" style="max-width:100%;"></a></p>
<p>Before preprocessing them, I resize them by 32x32.
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591988-08477800-b994-11e8-9e3c-8dc7523c04bb.png"><img src="https://user-images.githubusercontent.com/41224032/45591988-08477800-b994-11e8-9e3c-8dc7523c04bb.png" alt="120" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591990-15646700-b994-11e8-85c3-9c39c2cd2ab0.png"><img src="https://user-images.githubusercontent.com/41224032/45591990-15646700-b994-11e8-85c3-9c39c2cd2ab0.png" alt="turn right" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591992-1d240b80-b994-11e8-83a2-16f6a9ee1fc6.png"><img src="https://user-images.githubusercontent.com/41224032/45591992-1d240b80-b994-11e8-83a2-16f6a9ee1fc6.png" alt="stop" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591994-28773700-b994-11e8-9d37-b02c0edcaa44.png"><img src="https://user-images.githubusercontent.com/41224032/45591994-28773700-b994-11e8-9d37-b02c0edcaa44.png" alt="priority" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591996-3036db80-b994-11e8-8eee-3cc08d932c30.png"><img src="https://user-images.githubusercontent.com/41224032/45591996-3036db80-b994-11e8-8eee-3cc08d932c30.png" alt="70" style="max-width:100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://user-images.githubusercontent.com/41224032/45591997-35942600-b994-11e8-9051-5b34466f86b0.png"><img src="https://user-images.githubusercontent.com/41224032/45591997-35942600-b994-11e8-9051-5b34466f86b0.png" alt="pedestrain" style="max-width:100%;"></a></p>
<h4><a id="user-content-predict-the-sign-type-for-each-image" class="anchor" aria-hidden="true" href="#predict-the-sign-type-for-each-image"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Predict the Sign Type for Each Image</h4>
<p>Then I put these signs together as the shape of a dataset(6, 32, 32, 1), pre-process and test it.</p>
<p>Here are the results of the prediction:</p>
<table>
<thead>
<tr>
<th align="center">Image</th>
<th align="center">Prediction</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Speed limit (120km/h)</td>
<td align="center">No passing for vehicles over 3.5 metric tons</td>
</tr>
<tr>
<td align="center">Turn right ahead</td>
<td align="center">Turn right ahead</td>
</tr>
<tr>
<td align="center">Stop Sign</td>
<td align="center">Stop sign</td>
</tr>
<tr>
<td align="center">Right-of-way at the next intersection</td>
<td align="center">Right-of-way at the next intersection</td>
</tr>
<tr>
<td align="center">Speed limit (70km/h)</td>
<td align="center">Speed limit (70km/h)</td>
</tr>
<tr>
<td align="center">Pedestrians</td>
<td align="center">Pedestrians</td>
</tr></tbody></table>
<h4><a id="user-content-analyze-performance" class="anchor" aria-hidden="true" href="#analyze-performance"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Analyze Performance</h4>
<p>The model was able to correctly guess 5 of the 6 traffic signs, which gives an accuracy of 0.8333.</p>
<h4><a id="user-content-output-top-5-softmax-probabilities-for-each-image-found-on-the-web" class="anchor" aria-hidden="true" href="#output-top-5-softmax-probabilities-for-each-image-found-on-the-web"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Output Top 5 Softmax Probabilities For Each Image Found on the Web</h4>
<p>For the first image, the model is relatively sure that this is a No vehicles sign (probability of 0.99), but the image does not contain a No vehicles sign. The top five soft max probabilities were</p>
<table>
<thead>
<tr>
<th align="center">Probability</th>
<th align="center">Prediction</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">.99</td>
<td align="center">No vehicles</td>
</tr>
<tr>
<td align="center">.005</td>
<td align="center">Speed limit (100km/h)</td>
</tr>
<tr>
<td align="center">.000001</td>
<td align="center">Speed limit (60km/h)</td>
</tr>
<tr>
<td align="center">.0000005</td>
<td align="center">Children crossing</td>
</tr>
<tr>
<td align="center">.00000005</td>
<td align="center">Speed limit (20km/h)</td>
</tr></tbody></table>
<p>Seems something wrong here...</p>
</article>
  </div>

  </div>

  <details class="details-reset details-overlay details-overlay-dark">
    <summary data-hotkey="l" aria-label="Jump to line"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump" aria-label="Jump to line">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form Box-body d-flex" action="" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
        <button type="submit" class="btn" data-close-dialog>Go</button>
</form>    </details-dialog>
  </details>


  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>

    </div>
  </div>

  </div>

        
<div class="footer container-lg px-3" role="contentinfo">
  <div class="position-relative d-flex flex-justify-between pt-6 pb-2 mt-6 f6 text-gray border-top border-gray-light ">
    <ul class="list-style-none d-flex flex-wrap ">
      <li class="mr-3">&copy; 2018 <span title="0.23825s from unicorn-57d764b8b-6pmlt">GitHub</span>, Inc.</li>
        <li class="mr-3"><a data-ga-click="Footer, go to terms, text:terms" href="https://github.com/site/terms">Terms</a></li>
        <li class="mr-3"><a data-ga-click="Footer, go to privacy, text:privacy" href="https://github.com/site/privacy">Privacy</a></li>
        <li class="mr-3"><a href="https://help.github.com/articles/github-security/" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li class="mr-3"><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a data-ga-click="Footer, go to help, text:help" href="https://help.github.com">Help</a></li>
    </ul>

    <a aria-label="Homepage" title="GitHub" class="footer-octicon mr-lg-4" href="https://github.com">
      <svg height="24" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="24" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
   <ul class="list-style-none d-flex flex-wrap ">
        <li class="mr-3"><a data-ga-click="Footer, go to contact, text:contact" href="https://github.com/contact">Contact GitHub</a></li>
        <li class="mr-3"><a href="https://github.com/pricing" data-ga-click="Footer, go to Pricing, text:Pricing">Pricing</a></li>
      <li class="mr-3"><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li class="mr-3"><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
        <li class="mr-3"><a href="https://blog.github.com" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>

    </ul>
  </div>
  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 text-gray-light"></span>
  </div>
</div>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
    </button>
    You can’t perform that action at this time.
  </div>


    
    <script crossorigin="anonymous" integrity="sha512-9NU5KrrxF1N3QQF3lgKNzC7bZtHyXp9AASP+E5y5W3lEHA9HuFDiniVXCMN+UBCvqKLfBEQvfig7tlSxgSDmtQ==" type="application/javascript" src="https://assets-cdn.github.com/assets/frameworks-bb24e24eb672a7eeb917e84344c24a3f.js"></script>
    
    <script crossorigin="anonymous" async="async" integrity="sha512-Y//M0zEM+aaLZ2xtSgn9LtjIY0sJKhpN4/IE0z9/BVUMB7MrdFzTynH9IXln5qTKP1HGUg3szw1+hY042Cu/Ng==" type="application/javascript" src="https://assets-cdn.github.com/assets/github-72f4a85fb2995694e894281c3b7065d4.js"></script>
    
    
    
  <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
  <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
    </button>
  </div>
</div>

  <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark" open>
    <summary aria-haspopup="dialog" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast">
      <button class="m-3 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
        <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
      </button>
      <div class="octocat-spinner my-6 js-details-dialog-spinner"></div>
    </details-dialog>
  </details>
</template>

  <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box box-shadow-large" style="width:360px;">
  </div>
</div>

<div id="hovercard-aria-description" class="sr-only">
  Press h to open a hovercard with more details.
</div>


  </body>
</html>

