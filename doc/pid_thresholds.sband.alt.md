





<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
  <link rel="dns-prefetch" href="https://github.githubassets.com">
  <link rel="dns-prefetch" href="https://avatars0.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars1.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars2.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars3.githubusercontent.com">
  <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
  <link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">



  <link crossorigin="anonymous" media="all" integrity="sha512-pWLt6abkYhNeAHaDrPVG0yXCtIGRuCkwSUqQpsyN6smAIpIt+Iuq2IZKmoH9l3Cy/9ZnjvVrFZnvFFjGiqE3EA==" rel="stylesheet" href="https://github.githubassets.com/assets/frameworks-a3b8a10d4a9e37a78f033ef4a4f525f5.css" />
  <link crossorigin="anonymous" media="all" integrity="sha512-IST8JspDNfKOavszhBp7Z1zxXIrncPzvWLWp2S6A1FqFE74R5iIldEl/vpqtSMwUDbHHZZQO0KUQRC/rkDPlcg==" rel="stylesheet" href="https://github.githubassets.com/assets/github-b5621ac7a31fa904b2627bcd0f6079bc.css" />
  
  
  
  
  

  <meta name="viewport" content="width=device-width">
  
  <title>lrose-core/pid_thresholds.sband.alt.md at master · NCAR/lrose-core</title>
    <meta name="description" content="Core C/C++ code for LROSE. . Contribute to NCAR/lrose-core development by creating an account on GitHub.">
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    
    <meta property="og:image" content="https://avatars3.githubusercontent.com/u/2007542?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="NCAR/lrose-core" /><meta property="og:url" content="https://github.com/NCAR/lrose-core" /><meta property="og:description" content="Core C/C++ code for LROSE. . Contribute to NCAR/lrose-core development by creating an account on GitHub." />

  <link rel="assets" href="https://github.githubassets.com/">
  <link rel="web-socket" href="wss://live.github.com/_sockets/VjI6MzY0MDU2MjgxOmM1ZDRiOTI1OWU2Y2MzMjZiZTNmOTY2ZmUxZjNmYzhkMmEzZTEwMmRkZDhiZTBkNjM3MjRlYmZiM2MyNzlhNTA=--993815c960ac4f2c41dfe163314d7c3fac12109e">
  <meta name="pjax-timeout" content="1000">
  <link rel="sudo-modal" href="/sessions/sudo_modal">
  <meta name="request-id" content="C6BE:1381:E67D1:1BB6C6:5C47A006" data-pjax-transient>


  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

      <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
    <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">

  <meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-request_id" content="C6BE:1381:E67D1:1BB6C6:5C47A006" /><meta name="octolytics-dimension-region_edge" content="iad" /><meta name="octolytics-dimension-region_render" content="iad" /><meta name="octolytics-actor-id" content="31932009" /><meta name="octolytics-actor-login" content="jcdehart" /><meta name="octolytics-actor-hash" content="8b02d8075e36da4cd836f5d07ae8ee9fa56e2ce8dcf9bad57275cd73911791ed" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />



    <meta name="google-analytics" content="UA-3769691-2">

  <meta class="js-ga-set" name="userId" content="85d69660b8277439a0066ac826ae6268" %>

<meta class="js-ga-set" name="dimension1" content="Logged In">



  

      <meta name="hostname" content="github.com">
    <meta name="user-login" content="jcdehart">

      <meta name="expected-hostname" content="github.com">
    <meta name="js-proxy-site-detection-payload" content="ODEzZGNhZGUwZGY0MGNkNGQwNjUyOGJhMTBmNjEwNzM5MGU5MmEyMGMzZTFlZmRkZmZhZjg3YzQxZmE1NjY5NHx7InJlbW90ZV9hZGRyZXNzIjoiMTI5LjgyLjUwLjEwIiwicmVxdWVzdF9pZCI6IkM2QkU6MTM4MTpFNjdEMToxQkI2QzY6NUM0N0EwMDYiLCJ0aW1lc3RhbXAiOjE1NDgxOTc5MDIsImhvc3QiOiJnaXRodWIuY29tIn0=">

    <meta name="enabled-features" content="DASHBOARD_V2_LAYOUT,UNIVERSE_BANNER,MARKETPLACE_PLAN_RESTRICTION_EDITOR,NOTIFY_ON_BLOCK,RELATED_ISSUES,MARKETPLACE_INSIGHTS_V2">

  <meta name="html-safe-nonce" content="dd5acf04b46f8ce52660accd09e8718b6d43ae31">

  <meta http-equiv="x-pjax-version" content="b531aac8345ddc67dadb38f97fa9f5ec">
  

      <link href="https://github.com/NCAR/lrose-core/commits/master.atom" rel="alternate" title="Recent Commits to lrose-core:master" type="application/atom+xml">

  <meta name="go-import" content="github.com/NCAR/lrose-core git https://github.com/NCAR/lrose-core.git">

  <meta name="octolytics-dimension-user_id" content="2007542" /><meta name="octolytics-dimension-user_login" content="NCAR" /><meta name="octolytics-dimension-repository_id" content="51408988" /><meta name="octolytics-dimension-repository_nwo" content="NCAR/lrose-core" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="false" /><meta name="octolytics-dimension-repository_network_root_id" content="51408988" /><meta name="octolytics-dimension-repository_network_root_nwo" content="NCAR/lrose-core" /><meta name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" content="false" />


    <link rel="canonical" href="https://github.com/NCAR/lrose-core/blob/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md" data-pjax-transient>


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <link rel="mask-icon" href="https://github.githubassets.com/pinned-octocat.svg" color="#000000">
  <link rel="icon" type="image/x-icon" class="js-site-favicon" href="https://github.githubassets.com/favicon.ico">

<meta name="theme-color" content="#1e2327">


  <meta name="u2f-support" content="true">

  <link rel="manifest" href="/manifest.json" crossOrigin="use-credentials">

  </head>

  <body class="logged-in env-production emoji-size-boost page-blob">
    

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
      <nav class="d-flex" aria-label="Global">
            <div class="">
              <div class="header-search scoped-search site-scoped-search js-site-search position-relative js-jump-to"
  role="combobox"
  aria-owns="jump-to-results"
  aria-label="Search or jump to"
  aria-haspopup="listbox"
  aria-expanded="false"
>
  <div class="position-relative">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-site-search-form" data-scope-type="Repository" data-scope-id="51408988" data-scoped-search-url="/NCAR/lrose-core/search" data-unscoped-search-url="/search" action="/NCAR/lrose-core/search" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
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
          aria-label="Search or jump to…"
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations#csrf-token=Xkx+YmwWT0k/L3qLExyl12bH3vW2pcSNyhuyUHsMJAbmVGurJLpjJXyp7nUK27ZnixXgYAWYZsdHMeIvKlTYGA=="
          spellcheck="false"
          autocomplete="off"
          >
          <input type="hidden" class="js-site-search-type-field" name="type" >
            <img src="https://github.githubassets.com/images/search-key-slash.svg" alt="" class="mr-2 header-search-key-slash">

            <div class="Box position-absolute overflow-hidden d-none jump-to-suggestions js-jump-to-suggestions-container">
              
<ul class="d-none js-jump-to-suggestions-template-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-suggestion" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
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
  <li class="d-flex flex-justify-center flex-items-center f5 d-none js-jump-to-suggestion p-2">
    <span class="text-gray">No suggested jump to results</span>
  </li>
</ul>

<ul id="jump-to-results" role="listbox" class="p-0 m-0 js-navigation-container jump-to-suggestions-results-container js-jump-to-suggestions-results-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-scoped-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
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

  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-global-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
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


    <li class="d-flex flex-justify-center flex-items-center p-0 f5 js-jump-to-suggestion">
      <img src="https://github.githubassets.com/images/spinners/octocat-spinner-128.gif" alt="Octocat Spinner Icon" class="m-2" width="28">
    </li>
</ul>

            </div>
      </label>
</form>  </div>
</div>

            </div>

          <ul class="d-flex pl-2 flex-items-center text-bold list-style-none">
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-hotkey="g p" data-ga-click="Header, click, Nav menu - item:pulls context:user" aria-label="Pull requests you created" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls" href="/pulls">
                Pull requests
</a>            </li>
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-hotkey="g i" data-ga-click="Header, click, Nav menu - item:issues context:user" aria-label="Issues you created" data-selected-links="/issues /issues/assigned /issues/mentioned /issues" href="/issues">
                Issues
</a>            </li>
              <li class="position-relative">
                <a class="js-selected-navigation-item HeaderNavlink px-2" data-ga-click="Header, click, Nav menu - item:marketplace context:user" data-octo-click="marketplace_click" data-octo-dimensions="location:nav_bar" data-selected-links=" /marketplace" href="/marketplace">
                   Marketplace
</a>                  
              </li>
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-ga-click="Header, click, Nav menu - item:explore" data-selected-links="/explore /trending /trending/developers /integrations /integrations/feature/code /integrations/feature/collaborate /integrations/feature/ship showcases showcases_search showcases_landing /explore" href="/explore">
                Explore
</a>            </li>
          </ul>
      </nav>

      <div class="d-flex">
        
<ul class="user-nav d-flex flex-items-center list-style-none" id="user-links">
  <li class="dropdown">
    <span class="d-inline-block  px-2">
      
    <a aria-label="You have no unread notifications" class="notification-indicator tooltipped tooltipped-s  js-socket-channel js-notification-indicator" data-hotkey="g n" data-ga-click="Header, go to notifications, icon:read" data-channel="notification-changed:31932009" href="/notifications">
        <span class="mail-status "></span>
        <svg class="octicon octicon-bell" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 12v1H0v-1l.73-.58c.77-.77.81-2.55 1.19-4.42C2.69 3.23 6 2 6 2c0-.55.45-1 1-1s1 .45 1 1c0 0 3.39 1.23 4.16 5 .38 1.88.42 3.66 1.19 4.42l.66.58H14zm-7 4c1.11 0 2-.89 2-2H5c0 1.11.89 2 2 2z"/></svg>
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
    <span title="NCAR/lrose-core">This repository</span>
  </div>
    <a role="menuitem" class="dropdown-item" href="/NCAR/lrose-core/issues/new" data-ga-click="Header, create new issue">
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
        <img alt="@jcdehart" class="avatar float-left mr-1" src="https://avatars1.githubusercontent.com/u/31932009?s=40&amp;v=4" height="20" width="20">
        <span class="dropdown-caret"></span>
      </summary>
      <details-menu class="dropdown-menu dropdown-menu-sw">
        <div class="header-nav-current-user css-truncate"><a role="menuitem" class="no-underline user-profile-link px-3 pt-2 pb-2 mb-n2 mt-n1 d-block" href="/jcdehart" data-ga-click="Header, go to profile, text:Signed in as">Signed in as <strong class="css-truncate-target">jcdehart</strong></a></div>
        <div role="none" class="dropdown-divider"></div>

        <div class="px-3 f6 user-status-container js-user-status-context pb-1" data-url="/users/status?compact=1&amp;link_mentions=0&amp;truncate=1">
          
<div class="js-user-status-container user-status-compact" data-team-hovercards-enabled>
  <details class="js-user-status-details details-reset details-overlay details-overlay-dark">
    <summary class="btn-link no-underline js-toggle-user-status-edit toggle-user-status-edit width-full" aria-haspopup="dialog" role="menuitem">
      <div class="f6 d-inline-block v-align-middle  user-status-emoji-only-header pl-0 circle lh-condensed user-status-header " style="max-width: 29px">
        <div class="user-status-emoji-container flex-shrink-0 mr-1">
          <svg class="octicon octicon-smiley" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8s3.58 8 8 8 8-3.58 8-8-3.58-8-8-8zm4.81 12.81a6.72 6.72 0 0 1-2.17 1.45c-.83.36-1.72.53-2.64.53-.92 0-1.81-.17-2.64-.53-.81-.34-1.55-.83-2.17-1.45a6.773 6.773 0 0 1-1.45-2.17A6.59 6.59 0 0 1 1.21 8c0-.92.17-1.81.53-2.64.34-.81.83-1.55 1.45-2.17.62-.62 1.36-1.11 2.17-1.45A6.59 6.59 0 0 1 8 1.21c.92 0 1.81.17 2.64.53.81.34 1.55.83 2.17 1.45.62.62 1.11 1.36 1.45 2.17.36.83.53 1.72.53 2.64 0 .92-.17 1.81-.53 2.64-.34.81-.83 1.55-1.45 2.17zM4 6.8v-.59c0-.66.53-1.19 1.2-1.19h.59c.66 0 1.19.53 1.19 1.19v.59c0 .67-.53 1.2-1.19 1.2H5.2C4.53 8 4 7.47 4 6.8zm5 0v-.59c0-.66.53-1.19 1.2-1.19h.59c.66 0 1.19.53 1.19 1.19v.59c0 .67-.53 1.2-1.19 1.2h-.59C9.53 8 9 7.47 9 6.8zm4 3.2c-.72 1.88-2.91 3-5 3s-4.28-1.13-5-3c-.14-.39.23-1 .66-1h8.59c.41 0 .89.61.75 1z"/></svg>
        </div>
      </div>
      <div class="d-inline-block v-align-middle user-status-message-wrapper f6 lh-condensed ws-normal pt-1">
          <span class="link-gray">Set your status</span>
      </div>
    </summary>
    <details-dialog class="anim-fade-in fast Box Box--overlay" role="dialog" tabindex="-1">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="position-relative flex-auto js-user-status-form" action="/users/status?compact=1&amp;link_mentions=0&amp;truncate=1" accept-charset="UTF-8" data-remote="true" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="_method" value="put" /><input type="hidden" name="authenticity_token" value="A2T8CiC0J6YQ838dExtMzxF59Hfr1WBAdLwUH5gzI5/bVUVh0ZOZfTnm7aJDVhn53xQTy6U+lfFH7ItNI1VN9w==" />
        <div class="Box-header">
          <button class="Box-btn-octicon js-toggle-user-status-edit btn-octicon float-right" type="reset" aria-label="Close dialog" data-close-dialog>
            <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
          </button>
          <h3 class="Box-title text-gray-dark">Edit status</h3>
        </div>
        <input type="hidden" name="emoji" class="js-user-status-emoji-field" value="">
        <input type="hidden" name="organization_id" class="js-user-status-org-id-field" value="">
        <div class="px-3 py-2 text-gray-dark">
          <div class="js-characters-remaining-container js-suggester-container position-relative mt-2">
            <div class="input-group">
              <span class="input-group-button">
                <button type="button" aria-label="Choose an emoji" class="btn-outline btn js-toggle-user-status-emoji-picker">
                  <span class="js-user-status-original-emoji" hidden></span>
                  <span class="js-user-status-custom-emoji"></span>
                  <span class="js-user-status-no-emoji-icon" >
                    <svg class="octicon octicon-smiley" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8s3.58 8 8 8 8-3.58 8-8-3.58-8-8-8zm4.81 12.81a6.72 6.72 0 0 1-2.17 1.45c-.83.36-1.72.53-2.64.53-.92 0-1.81-.17-2.64-.53-.81-.34-1.55-.83-2.17-1.45a6.773 6.773 0 0 1-1.45-2.17A6.59 6.59 0 0 1 1.21 8c0-.92.17-1.81.53-2.64.34-.81.83-1.55 1.45-2.17.62-.62 1.36-1.11 2.17-1.45A6.59 6.59 0 0 1 8 1.21c.92 0 1.81.17 2.64.53.81.34 1.55.83 2.17 1.45.62.62 1.11 1.36 1.45 2.17.36.83.53 1.72.53 2.64 0 .92-.17 1.81-.53 2.64-.34.81-.83 1.55-1.45 2.17zM4 6.8v-.59c0-.66.53-1.19 1.2-1.19h.59c.66 0 1.19.53 1.19 1.19v.59c0 .67-.53 1.2-1.19 1.2H5.2C4.53 8 4 7.47 4 6.8zm5 0v-.59c0-.66.53-1.19 1.2-1.19h.59c.66 0 1.19.53 1.19 1.19v.59c0 .67-.53 1.2-1.19 1.2h-.59C9.53 8 9 7.47 9 6.8zm4 3.2c-.72 1.88-2.91 3-5 3s-4.28-1.13-5-3c-.14-.39.23-1 .66-1h8.59c.41 0 .89.61.75 1z"/></svg>
                  </span>
                </button>
              </span>
              <input type="text" autocomplete="off" autofocus data-maxlength="80" class="js-suggester-field form-control js-user-status-message-field js-characters-remaining-field" placeholder="What's happening?" name="message" required value="" aria-label="What is your current status?">
            </div>
            <div class="suggester-container">
              <div class="suggester js-suggester js-navigation-container" data-url="/autocomplete/user-suggestions" data-no-org-url="/autocomplete/user-suggestions" data-org-url="/suggestions" hidden>
              </div>
            </div>
            <div style="margin-left: 53px" class="my-1 text-small label-characters-remaining js-characters-remaining" data-suffix="remaining" hidden>
              80 remaining
            </div>
          </div>
          <include-fragment class="js-user-status-emoji-picker" data-url="/users/status/emoji"></include-fragment>
          <div class="overflow-auto" style="max-height: 33vh">
            <div class="user-status-suggestions js-user-status-suggestions">
              <h4 class="f6 text-normal my-3">Suggestions:</h4>
              <div class="mx-3 mt-2 clearfix">
                  <div class="float-left col-6">
                      <button type="button" value=":palm_tree:" class="d-flex flex-items-baseline flex-items-stretch lh-condensed f6 btn-link link-gray no-underline js-predefined-user-status mb-1">
                        <div class="emoji-status-width mr-2 v-align-middle js-predefined-user-status-emoji">
                          <g-emoji alias="palm_tree" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f334.png">🌴</g-emoji>
                        </div>
                        <div class="d-flex flex-items-center no-underline js-predefined-user-status-message" style="border-left: 1px solid transparent">
                          On vacation
                        </div>
                      </button>
                      <button type="button" value=":face_with_thermometer:" class="d-flex flex-items-baseline flex-items-stretch lh-condensed f6 btn-link link-gray no-underline js-predefined-user-status mb-1">
                        <div class="emoji-status-width mr-2 v-align-middle js-predefined-user-status-emoji">
                          <g-emoji alias="face_with_thermometer" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f912.png">🤒</g-emoji>
                        </div>
                        <div class="d-flex flex-items-center no-underline js-predefined-user-status-message" style="border-left: 1px solid transparent">
                          Out sick
                        </div>
                      </button>
                  </div>
                  <div class="float-left col-6">
                      <button type="button" value=":house:" class="d-flex flex-items-baseline flex-items-stretch lh-condensed f6 btn-link link-gray no-underline js-predefined-user-status mb-1">
                        <div class="emoji-status-width mr-2 v-align-middle js-predefined-user-status-emoji">
                          <g-emoji alias="house" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3e0.png">🏠</g-emoji>
                        </div>
                        <div class="d-flex flex-items-center no-underline js-predefined-user-status-message" style="border-left: 1px solid transparent">
                          Working from home
                        </div>
                      </button>
                      <button type="button" value=":dart:" class="d-flex flex-items-baseline flex-items-stretch lh-condensed f6 btn-link link-gray no-underline js-predefined-user-status mb-1">
                        <div class="emoji-status-width mr-2 v-align-middle js-predefined-user-status-emoji">
                          <g-emoji alias="dart" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3af.png">🎯</g-emoji>
                        </div>
                        <div class="d-flex flex-items-center no-underline js-predefined-user-status-message" style="border-left: 1px solid transparent">
                          Focusing
                        </div>
                      </button>
                  </div>
              </div>
            </div>
            <div class="user-status-limited-availability-container">
              <div class="form-checkbox my-0">
                <input type="checkbox" name="limited_availability" value="1" class="js-user-status-limited-availability-checkbox" data-default-message="I may be slow to respond." aria-describedby="limited-availability-help-text-truncate-true" id="limited-availability-truncate-true">
                <label class="d-block f5 text-gray-dark mb-1" for="limited-availability-truncate-true">
                  Busy
                </label>
                <p class="note" id="limited-availability-help-text-truncate-true">
                  When others mention you, assign you, or request your review,
                  GitHub will let them know that you have limited availability.
                </p>
              </div>
            </div>
          </div>
          <include-fragment class="js-user-status-org-picker" data-url="/users/status/organizations"></include-fragment>
        </div>
        <div class="d-flex flex-items-center flex-justify-between p-3 border-top">
          <button type="submit" disabled class="width-full btn btn-primary mr-2 js-user-status-submit">
            Set status
          </button>
          <button type="button" disabled class="width-full js-clear-user-status-button btn ml-2 ">
            Clear status
          </button>
        </div>
</form>    </details-dialog>
  </details>

</div>

        </div>
        <div role="none" class="dropdown-divider"></div>

        <a role="menuitem" class="dropdown-item" href="/jcdehart" data-ga-click="Header, go to profile, text:your profile">Your profile</a>
        <a role="menuitem" class="dropdown-item" href="/jcdehart?tab=repositories" data-ga-click="Header, go to repositories, text:your repositories">Your repositories</a>


        <a role="menuitem" class="dropdown-item" href="/jcdehart?tab=stars" data-ga-click="Header, go to starred repos, text:your stars">Your stars</a>
          <a role="menuitem" class="dropdown-item" href="https://gist.github.com/" data-ga-click="Header, your gists, text:your gists">Your gists</a>

        <div role="none" class="dropdown-divider"></div>
        <a role="menuitem" class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a>
        <a role="menuitem" class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">Settings</a>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="logout-form" action="/logout" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="6dHo3igOJyi4B4zESVPaOXBMmTu6OyqjPpPBdxnmcFM/MIT/pxxi2ups8oQfP3SXsP24Wuun0cEnjksRFjl/EA==" />
          
          <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout" role="menuitem">
            Sign out
          </button>
</form>      </details-menu>
    </details>
  </li>
</ul>



        <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="sr-only right-0" action="/logout" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="6wSIz1RowvLVYXH4EOs65KG627YGHk4BKjVvlbacNek95eTu23qHAIcKD7hGh5RKYQv611eCtWMzKOXzuUM6qg==" />
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



  <div role="main" class="application-main " data-commit-hovercards-enabled>
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode" class="">
    <div id="js-repo-pjax-container" data-pjax-container >
      


  


  




  <div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav  ">
    <div class="repohead-details-container clearfix container">

      <ul class="pagehead-actions">
  <li>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form data-remote="true" class="js-social-form js-social-container" action="/notifications/subscribe" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="/0FihZ8TzJMnOs3OQlFuz8wB7MNWKemc2y4VCEcOJZVHtXDUufv0ypUWJX7gnEEV+MsUK5NgQgLWjQGuRKKiQw==" />      <input type="hidden" name="repository_id" id="repository_id" value="51408988" class="form-control" />

      <details class="details-reset details-overlay select-menu float-left">
        <summary class="btn btn-sm btn-with-count select-menu-button" data-ga-click="Repository, click Watch settings, action:blob#show">
          <span data-menu-button>
              <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
              Watch
          </span>
        </summary>
        <details-menu class="select-menu-modal position-absolute mt-5" style="z-index: 99;">
          <div class="select-menu-header">
            <span class="select-menu-title">Notifications</span>
          </div>
          <div class="select-menu-list">
            <button type="submit" name="do" value="included" class="select-menu-item width-full" aria-checked="true" role="menuitemradio">
              <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
              <div class="select-menu-item-text">
                <span class="select-menu-item-heading">Not watching</span>
                <span class="description">Be notified only when participating or @mentioned.</span>
                <span class="hidden-select-button-text" data-menu-button-contents>
                  <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                  Watch
                </span>
              </div>
            </button>

            <button type="submit" name="do" value="release_only" class="select-menu-item width-full" aria-checked="false" role="menuitemradio">
              <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
              <div class="select-menu-item-text">
                <span class="select-menu-item-heading">Releases only</span>
                <span class="description">Be notified of new releases, and when participating or @mentioned.</span>
                <span class="hidden-select-button-text" data-menu-button-contents>
                  <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                  Unwatch releases
                </span>
              </div>
            </button>

            <button type="submit" name="do" value="subscribed" class="select-menu-item width-full" aria-checked="false" role="menuitemradio">
              <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
              <div class="select-menu-item-text">
                <span class="select-menu-item-heading">Watching</span>
                <span class="description">Be notified of all conversations.</span>
                <span class="hidden-select-button-text" data-menu-button-contents>
                  <svg class="octicon octicon-eye v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                  Unwatch
                </span>
              </div>
            </button>

            <button type="submit" name="do" value="ignore" class="select-menu-item width-full" aria-checked="false" role="menuitemradio">
              <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
              <div class="select-menu-item-text">
                <span class="select-menu-item-heading">Ignoring</span>
                <span class="description">Never be notified.</span>
                <span class="hidden-select-button-text" data-menu-button-contents>
                  <svg class="octicon octicon-mute v-align-text-bottom" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 2.81v10.38c0 .67-.81 1-1.28.53L3 10H1c-.55 0-1-.45-1-1V7c0-.55.45-1 1-1h2l3.72-3.72C7.19 1.81 8 2.14 8 2.81zm7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06L11.44 8 9.47 9.97l1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06L13.56 8l1.97-1.97z"/></svg>
                  Stop ignoring
                </span>
              </div>
            </button>
          </div>
        </details-menu>
      </details>
      <a class="social-count js-social-count"
        href="/NCAR/lrose-core/watchers"
        aria-label="22 users are watching this repository">
        22
      </a>
</form>
  </li>

  <li>
      <div class="js-toggler-container js-social-container starring-container ">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="starred js-social-form" action="/NCAR/lrose-core/unstar" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="k/blv4rpEiyjfwBw24XfdFIuDCk+inMCFcb3Oi7RwZ4k2B7zDJQ8COVpSivb6819mi7ppfbD+qaDNRARp3SRfA==" />
      <input type="hidden" name="context" value="repository"></input>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar NCAR/lrose-core"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg class="octicon octicon-star v-align-text-bottom" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/NCAR/lrose-core/stargazers"
           aria-label="21 users starred this repository">
          21
        </a>
</form>
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="unstarred js-social-form" action="/NCAR/lrose-core/star" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="LmP4AN/O1gIDUVM+IuwJISwQ3Dx1td/m97aOw0EG5YxZyNxqxtThMbgGjMIFOfjCSO58P/BtKsOM24k7VSj+Eg==" />
      <input type="hidden" name="context" value="repository"></input>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star NCAR/lrose-core"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg class="octicon octicon-star v-align-text-bottom" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/NCAR/lrose-core/stargazers"
           aria-label="21 users starred this repository">
          21
        </a>
</form>  </div>

  </li>

  <li>
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="btn-with-count" action="/NCAR/lrose-core/fork" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="iXDDx0Ez7qtsXAGWlDdFSHl+f1/t2rtAUD4K8asP1+C7WBXj6RgzhKz80cO7znAKDwWipLulTH/2n+JERw9RTQ==" />
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of NCAR/lrose-core to your account"
                aria-label="Fork your own copy of NCAR/lrose-core to your account">
              <svg class="octicon octicon-repo-forked v-align-text-bottom" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
              Fork
            </button>
</form>
    <a href="/NCAR/lrose-core/network/members" class="social-count"
       aria-label="22 users forked this repository">
      22
    </a>
  </li>
</ul>

      <h1 class="public ">
  <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a class="url fn" rel="author" data-hovercard-type="organization" data-hovercard-url="/orgs/NCAR/hovercard" href="/NCAR">NCAR</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a data-pjax="#js-repo-pjax-container" href="/NCAR/lrose-core">lrose-core</a></strong>

</h1>

    </div>
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax container"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
    aria-label="Repository"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a class="js-selected-navigation-item selected reponav-item" itemprop="url" data-hotkey="g c" aria-current="page" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /NCAR/lrose-core" href="/NCAR/lrose-core">
      <svg class="octicon octicon-code" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a itemprop="url" data-hotkey="g i" class="js-selected-navigation-item reponav-item" data-selected-links="repo_issues repo_labels repo_milestones /NCAR/lrose-core/issues" href="/NCAR/lrose-core/issues">
        <svg class="octicon octicon-issue-opened" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg>
        <span itemprop="name">Issues</span>
        <span class="Counter">39</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a data-hotkey="g p" itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /NCAR/lrose-core/pulls" href="/NCAR/lrose-core/pulls">
      <svg class="octicon octicon-git-pull-request" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="Counter">1</span>
      <meta itemprop="position" content="3">
</a>  </span>


    <a data-hotkey="g b" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /NCAR/lrose-core/projects" href="/NCAR/lrose-core/projects">
      <svg class="octicon octicon-project" viewBox="0 0 15 16" version="1.1" width="15" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      Projects
      <span class="Counter" >0</span>
</a>

    <a class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /NCAR/lrose-core/wiki" href="/NCAR/lrose-core/wiki">
      <svg class="octicon octicon-book" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M3 5h4v1H3V5zm0 3h4V7H3v1zm0 2h4V9H3v1zm11-5h-4v1h4V5zm0 2h-4v1h4V7zm0 2h-4v1h4V9zm2-6v9c0 .55-.45 1-1 1H9.5l-1 1-1-1H2c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h5.5l1 1 1-1H15c.55 0 1 .45 1 1zm-8 .5L7.5 3H2v9h6V3.5zm7-.5H9.5l-.5.5V12h6V3z"/></svg>
      Wiki
</a>
    <a class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors dependency_graph pulse alerts security people /NCAR/lrose-core/pulse" href="/NCAR/lrose-core/pulse">
      <svg class="octicon octicon-graph" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
      Insights
</a>

</nav>


  </div>

<div class="container new-discussion-timeline experiment-repo-nav  ">
  <div class="repository-content ">

    
    



  
    <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/NCAR/lrose-core/blob/e450b6543bc34030c0bc4aa894a418e8f905d5ed/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md">Permalink</a>

    <!-- blob contrib key: blob_contributors:v21:058e92e4ae0c3713dd5866d8505d5027 -->

    

    <div class="file-navigation">
      
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left js-load-contents"
  data-contents-url="/NCAR/lrose-core/ref-list/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md?source_action=show&amp;source_controller=blob">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" aria-expanded="false" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax>
    <div class="select-menu-modal">
      <div class="js-select-menu-deferred-content"></div>
      <div class="select-menu-loading-overlay anim-pulse">
        <svg height="32" class="octicon octicon-octoface" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M14.7 5.34c.13-.32.55-1.59-.13-3.31 0 0-1.05-.33-3.44 1.3-1-.28-2.07-.32-3.13-.32s-2.13.04-3.13.32c-2.39-1.64-3.44-1.3-3.44-1.3-.68 1.72-.26 2.99-.13 3.31C.49 6.21 0 7.33 0 8.69 0 13.84 3.33 15 7.98 15S16 13.84 16 8.69c0-1.36-.49-2.48-1.3-3.35zM8 14.02c-3.3 0-5.98-.15-5.98-3.35 0-.76.38-1.48 1.02-2.07 1.07-.98 2.9-.46 4.96-.46 2.07 0 3.88-.52 4.96.46.65.59 1.02 1.3 1.02 2.07 0 3.19-2.68 3.35-5.98 3.35zM5.49 9.01c-.66 0-1.2.8-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.54-1.78-1.2-1.78zm5.02 0c-.66 0-1.2.79-1.2 1.78s.54 1.79 1.2 1.79c.66 0 1.2-.8 1.2-1.79s-.53-1.78-1.2-1.78z"/></svg>
      </div>
    </div>
  </div>
</div>

      <div class="BtnGroup float-right">
        <a href="/NCAR/lrose-core/find/master"
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
        <span class="repo-root js-repo-root"><span class="js-path-segment"><a data-pjax="true" href="/NCAR/lrose-core"><span>lrose-core</span></a></span></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/NCAR/lrose-core/tree/master/docs"><span>docs</span></a></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/NCAR/lrose-core/tree/master/docs/apps"><span>apps</span></a></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/NCAR/lrose-core/tree/master/docs/apps/radx"><span>radx</span></a></span><span class="separator">/</span><span class="js-path-segment"><a data-pjax="true" href="/NCAR/lrose-core/tree/master/docs/apps/radx/dualpol"><span>dualpol</span></a></span><span class="separator">/</span><strong class="final-path">pid_thresholds.sband.alt.md</strong>
      </div>
    </div>


    <include-fragment src="/NCAR/lrose-core/contributors/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md" class="commit-tease commit-loader">
      <div>
        Fetching contributors&hellip;
      </div>

      <div class="commit-tease-contributors">
          <img alt="" class="loader-loading float-left" src="https://github.githubassets.com/images/spinners/octocat-spinner-32-EAF2F5.gif" width="16" height="16" />
        <span class="loader-error">Cannot retrieve contributors at this time</span>
      </div>
</include-fragment>



    <div class="file ">
      
<div class="file-header">

  <div class="file-actions">


    <div class="BtnGroup">
      <a id="raw-url" class="btn btn-sm BtnGroup-item" href="/NCAR/lrose-core/raw/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md">Raw</a>
        <a class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b" href="/NCAR/lrose-core/blame/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md">Blame</a>
      <a rel="nofollow" class="btn btn-sm BtnGroup-item" href="/NCAR/lrose-core/commits/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="https://desktop.github.com"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:mac">
            <svg class="octicon octicon-device-desktop" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"/></svg>
        </a>

          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form js-update-url-with-hash" action="/NCAR/lrose-core/edit/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="rosstP9VRpPZQ2mwn2QgUibd5/9Xe+jlCMr0acuQqnPvVZS9mKTdWTyvFRsxn0UAvZhqLWZNGyESfcdy2vSexQ==" />
            <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
              aria-label="Fork this project and edit the file" data-hotkey="e" data-disable-with>
              <svg class="octicon octicon-pencil" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
            </button>
</form>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form" action="/NCAR/lrose-core/delete/master/docs/apps/radx/dualpol/pid_thresholds.sband.alt.md" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="STFWDrO62bvFDtpFLwf2Bw52Zv0DUE2iwjW0a6XeQUQTVMpNkqlnChOTHDUgi18s/X9Pe4TVxfQdyl88qpr6Qw==" />
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Fork this project and delete the file" data-disable-with>
            <svg class="octicon octicon-trashcan" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
          </button>
</form>  </div>

  <div class="file-info">
      656 lines (595 sloc)
      <span class="file-info-divider"></span>
    36.2 KB
  </div>
</div>

      
  <div id="readme" class="readme blob instapaper_body js-code-block-container">
    <article class="markdown-body entry-content" itemprop="text"><pre><code>
# PID Fuzzy Logic parameters - S-band Alternating Mode radars
#
# ---------------------------------
# begin comments with the "#" sign
# the mnemonics are forced to lower case so
# the capitalization is just for readability
#
# field mnemonics "zdr","zh","ldr","kdp","rhv","tmp","svr","sdzdr","sphi"
# line identifiers   "mmr", "tbl", "tpf", "wts", "thr"
# thresholding relations "lt", "gt", "le", "ge", "notch"

# Manditory user assigned pid codes
#
pid.cl	    (1)	 # Cloud                        
pid.drz     (2)  # Drizzle                      
pid.lr	    (3)  # Light_Rain                   
pid.mr	    (4)  # Moderate_Rain                
pid.hr	    (5)  # Heavy_Rain                   
pid.ha	    (6)  # Hail                         
pid.rh	    (7)  # Rain_Hail_Mixture            
pid.gsh     (8)  # Graupel_Small_Hail           
pid.grr     (9)  # Graupel_Rain                 
pid.ds	    (10) # Dry_Snow                     
pid.ws	    (11) # Wet_Snow                     
pid.ic	    (12) # Ice_Crystals                 
pid.iic     (13) # Irreg_Ice_Crystals           
pid.sld     (14) # Supercooled_Liquid_Droplets  
pid.bgs     (15) # Flying_Insects               
pid.trip2   (16) # Second trip                  
pid.gcl     (17) # Ground_Clutter          
pid.sat     (18) # Receiver saturation
#
# define Cloud                        1     //   "CL"
# define Drizzle                      2     //   "DRZ"
# define Light_Rain                   3     //   "LR"
# define Moderate_Rain                4     //   "MR"
# define Heavy_Rain                   5     //   "HR"
# define Hail                         6     //   "HA"
# define Rain_Hail_Mixture            7     //   "RH"
# define Graupel_Small_Hail           8     //   "GSH"
# define Graupel_Rain                 9     //   "GRR"
# define Dry_Snow                     10    //   "DS"
# define Wet_Snow                     11    //   "WS"
# define Ice_Crystals                 12    //   "IC"
# define Irreg_Ice_Crystals           13    //   "IIC"
# define Supercooled_Liquid_Droplets  14    //   "SLD"
# define Flying_Insects               15    //   "BGS" (bugs - Aphids, Mosquitos, etc.)
# define Second_trip                  16    //   "TRIP2"
# define Ground_Clutter               17    //   "GCL"
#
#
# Define a height vs temperature profile (km,C)


# 2011/10/16 GAN 2Z sounding

Tpf (0,25) (2.5,11.7) (4.0,4.5) (4.8,0.0) (6.0,-6.1) (10.0, -32.3) (20.0, -69.6)

#Tpf (0,25.6) (0.94,15.2) (2.1,13.0) (3.1,6.2) (3.4,4.1) (3.9,-0.9) (4.2,-2.5) (4.8,-5.5) (5.8,-12.1) (6.9,-20.5) (8.9,-20.5) (10.2,-45.5) (11.2,-51.1) (14.0,-61.1) (15.6,-70.7) (18.1,-65.9) (20.6,-63.1) # brisbane Dec 2008
#Tpf (0,28.0) (1.6,23.0) (2.3,16.0) (2.9,12.0) (3.5,8.3) (4.0,0.0) (5.2,-5.0) (6.4,-10.0) (8.0,-20) (10.2,-40.0) # brisbane March 2008

# Define weights for the particle derived for each variable
Wts  (Tmp,20) (Zh,20) (Zdr,20) (Kdp,5) (Ldr,10) (Rhv,10) (Sdzdr,30) (Sphi,30)
#
# Thresholding information
#
thr.Sld.Zh.lt    (70) # eliminate Sld entirely!!!
thr.Sld.tmp.gt   (0)
thr.Sld.tmp.lt   (-40)
thr.Ha.Zh.lt     (45) # no hail below 45 dBZ
thr.Ds.tmp.gt    (1)
thr.Ic.tmp.gt    (0)
thr.Iic.tmp.gt   (0)
thr.Ic.Zdr.lt    (0.5)
thr.Ws.tmp.gt    (8) 
thr.Ws.tmp.lt    (-8)
thr.Ws.Zdr.lt    (0.3)
thr.Mr.Zdr.le    (0.1)
thr.Hr.Zdr.le    (0.3)
thr.CL.Tmp.lt    (0)
thr.CL.Zdr.gt    (1.0)
thr.DRZ.Tmp.lt   (0)
thr.DRZ.Zdr.gt   (1.5)
thr.Lr.Tmp.lt    (0)
thr.Mr.Tmp.lt    (0)
thr.GRR.Tmp.lt   (-30)
thr.Hr.Tmp.lt    (0)
thr.Rh.Tmp.lt    (-30)
thr.Bgs.Tmp.lt    (0)
thr.Bgs.Zdr.lt    (2)
thr.gcl.Sdzdr.lt  (2)
thr.Trip2.Ldr.lt  (0.0)
#thr.Trip2.Zh.lt   (500.0) # eliminate second trip
#
# for tables:
# the second mnemonic is the independent variable and
# the third mnemonic is the dependent variable
# the fourth menmonic is the particle
#
# "pwl" stands for piecewise linear function
#
 Membership functions for Reflectivity
#
Tbl.Zh.Zh.CL     (-20,90)   (-20,0)  (-15,1) (5,1) (10,0)
Tbl.Zh.Zh.Drz    (-20,90)   (0,0)  (5,1) (25,1) (30,0)
Tbl.Zh.Zh.Lr     (-20,90)   (13,0)  (15,1) (35,1) (40,0)
Tbl.Zh.Zh.Mr     (-20,90)   (30,0)  (35,1) (45,1) (50,0)
Tbl.Zh.Zh.Hr     (-20,90)   (40,0)  (45,1) (55,1) (60,0)
Tbl.Zh.Zh.Ha     (-20,90)   (45,0)  (50,1) (90,1)
Tbl.Zh.Zh.Rh     (-20,90)   (45,0)  (50,1) (90,1)
Tbl.Zh.Zh.Gsh    (-20,90)   (25,0)  (30,1) (50,1) (55,0)
Tbl.Zh.Zh.GRR    (-20,90)   (25,0)  (30,1) (50,1) (55,0)
Tbl.Zh.Zh.Ds     (-20,90)   (10,0)  (15,1) (33,1) (35,0)
Tbl.Zh.Zh.Ws     (-20,90)   (0,0)  (7,1) (45,1) (50,0)
Tbl.Zh.Zh.Ic     (-20,90)   (-10,0)  (0,1)  (15,1) (25,0)
Tbl.Zh.Zh.Iic    (-20,90)   (-10,0) (0,1) (15,1) (25,0)
Tbl.Zh.Zh.Sld    (-20,90)   (-20,1) (30,1)  (35,0)
Tbl.Zh.Zh.Bgs    (-20,90)   (-7,0) (-5,1)  (30,1)   (35,0)
Tbl.Zh.Zh.Trip2  (-20,90)   (-20,1) (30,1) (35,0)
Tbl.Zh.Zh.Gcl    (-20,90)   (-20,0) (-15,1)  (70,1)
#
# Membership functions for ZDR
#
Tbl.Zh.Zdr.CL    (-20.0,-8.0)   (-0.3000,0) (0.0000,1) (0.5940,1) (0.9940,0)
Tbl.Zh.Zdr.CL    (-8.0,-6.0)   (-0.3000,0) (0.0000,1) (0.5286,1) (0.9286,0)
Tbl.Zh.Zdr.CL    (-6.0,-4.0)   (-0.3000,0) (0.0000,1) (0.4736,1) (0.8736,0)
Tbl.Zh.Zdr.CL    (-4.0,-2.0)   (-0.3000,0) (0.0000,1) (0.4290,1) (0.8290,0)
Tbl.Zh.Zdr.CL    (-2.0,0.0)   (-0.3000,0) (0.0000,1) (0.3948,1) (0.7948,0)
Tbl.Zh.Zdr.CL    (0.0,2.0)   (-0.3000,0) (0.0000,1) (0.3710,1) (0.7710,0)
Tbl.Zh.Zdr.CL    (2.0,4.0)   (-0.3000,0) (0.0000,1) (0.3576,1) (0.7576,0)
Tbl.Zh.Zdr.CL    (4.0,6.0)   (-0.3000,0) (0.0000,1) (0.3546,1) (0.7546,0)

Tbl.Zh.Zdr.Drz    (0.0,2.0)   (-0.3000,0) (0.0000,1) (0.3710,1) (0.7710,0)
Tbl.Zh.Zdr.Drz    (2.0,4.0)   (-0.3000,0) (0.0000,1) (0.3576,1) (0.7576,0)
Tbl.Zh.Zdr.Drz    (4.0,6.0)   (-0.3000,0) (0.0000,1) (0.3546,1) (0.7546,0)
Tbl.Zh.Zdr.Drz    (6.0,8.0)   (-0.3000,0) (0.0000,1) (0.3620,1) (0.7620,0)
Tbl.Zh.Zdr.Drz    (8.0,10.0)   (-0.3000,0) (0.0000,1) (0.3798,1) (0.7798,0)
Tbl.Zh.Zdr.Drz    (10.0,12.0)   (-0.3000,0) (0.0000,1) (0.4080,1) (0.8080,0)
Tbl.Zh.Zdr.Drz    (12.0,14.0)   (-0.3000,0) (0.0000,1) (0.4466,1) (0.8466,0)
Tbl.Zh.Zdr.Drz    (14.0,16.0)   (-0.3000,0) (0.0000,1) (0.4956,1) (0.8956,0)
Tbl.Zh.Zdr.Drz    (16.0,18.0)   (-0.3000,0) (0.0000,1) (0.5550,1) (0.9550,0)
Tbl.Zh.Zdr.Drz    (18.0,20.0)   (-0.3000,0) (0.0000,1) (0.6248,1) (1.0248,0)

Tbl.Zh.Zdr.Lr      (19.0,21.0)   (-0.3000,0) (0.0000,1) (0.6636,1) (1.0636,0)
Tbl.Zh.Zdr.Lr      (21.0,23.0)   (-0.3000,0) (0.0000,1) (0.7490,1) (1.1490,0)
Tbl.Zh.Zdr.Lr      (23.0,25.0)   (-0.3000,0) (0.0000,1) (0.8448,1) (1.2448,0)
Tbl.Zh.Zdr.Lr      (25.0,27.0)   (-0.3000,0) (0.0000,1) (0.9510,1) (1.3510,0)
Tbl.Zh.Zdr.Lr      (27.0,29.0)   (-0.3000,0) (0.0000,1) (1.0676,1) (1.4676,0)
Tbl.Zh.Zdr.Lr      (29.0,31.0)   (-0.2904,0) (0.0096,1) (1.1946,1) (1.5946,0)
Tbl.Zh.Zdr.Lr      (31.0,33.0)   (-0.2618,0) (0.0382,1) (1.3320,1) (1.7320,0)
Tbl.Zh.Zdr.Lr      (33.0,35.0)   (-0.2140,0) (0.0860,1) (1.4798,1) (1.8798,0)
Tbl.Zh.Zdr.Lr      (35.0,37.0)   (-0.1472,0) (0.1528,1) (1.6380,1) (2.0380,0)
Tbl.Zh.Zdr.Lr      (37.0,39.0)   (-0.0612,0) (0.2388,1) (1.8066,1) (2.2066,0)

Tbl.Zh.Zdr.Mr      (29.0,31.0)   (-0.2904,0) (0.0096,1) (1.1946,1) (1.5946,0)
Tbl.Zh.Zdr.Mr      (31.0,33.0)   (-0.2618,0) (0.0382,1) (1.3320,1) (1.7320,0)
Tbl.Zh.Zdr.Mr      (33.0,35.0)   (-0.2140,0) (0.0860,1) (1.4798,1) (1.8798,0)
Tbl.Zh.Zdr.Mr      (35.0,37.0)   (-0.1472,0) (0.1528,1) (1.6380,1) (2.0380,0)
Tbl.Zh.Zdr.Mr      (37.0,39.0)   (-0.0612,0) (0.2388,1) (1.8066,1) (2.2066,0)
Tbl.Zh.Zdr.Mr      (39.0,41.0)   (0.0438,0) (0.3438,1) (1.9856,1) (2.3856,0)
Tbl.Zh.Zdr.Mr      (41.0,43.0)   (0.1680,0) (0.4680,1) (2.1750,1) (2.5750,0)
Tbl.Zh.Zdr.Mr      (43.0,45.0)   (0.3112,0) (0.6112,1) (2.3748,1) (2.7748,0)
Tbl.Zh.Zdr.Mr      (45.0,47.0)   (0.4628,0) (0.7628,1) (2.5850,1) (2.9850,0)
Tbl.Zh.Zdr.Mr      (47.0,49.0)   (0.5965,0) (0.8965,1) (2.8056,1) (3.2056,0)
Tbl.Zh.Zdr.Mr      (49.0,51.0)   (0.7111,0) (1.0111,1) (3.0366,1) (3.4366,0)

Tbl.Zh.Zdr.Hr      (39.0,41.0)   (0.0438,0) (0.3438,1) (1.9856,1) (2.3856,0)
Tbl.Zh.Zdr.Hr      (41.0,43.0)   (0.1680,0) (0.4680,1) (2.1750,1) (2.5750,0)
Tbl.Zh.Zdr.Hr      (43.0,45.0)   (0.3112,0) (0.6112,1) (2.3748,1) (2.7748,0)
Tbl.Zh.Zdr.Hr      (45.0,47.0)   (0.4628,0) (0.7628,1) (2.5850,1) (2.9850,0)
Tbl.Zh.Zdr.Hr      (47.0,49.0)   (0.5965,0) (0.8965,1) (2.8056,1) (3.2056,0)
Tbl.Zh.Zdr.Hr      (49.0,51.0)   (0.7111,0) (1.0111,1) (3.0366,1) (3.4366,0)
Tbl.Zh.Zdr.Hr      (51.0,53.0)   (0.8066,0) (1.1066,1) (3.2780,1) (3.6780,0)
Tbl.Zh.Zdr.Hr      (53.0,55.0)   (0.8830,0) (1.1830,1) (3.5298,1) (3.9298,0)
Tbl.Zh.Zdr.Hr      (55.0,57.0)   (0.9403,0) (1.2403,1) (3.7920,1) (4.1920,0)
Tbl.Zh.Zdr.Hr      (57.0,59.0)   (0.9785,0) (1.2785,1) (4.0646,1) (4.4646,0)
Tbl.Zh.Zdr.Hr      (59.0,61.0)   (0.9976,0) (1.2976,1) (4.3476,1) (4.7476,0)

Tbl.Zh.Zdr.Ha    (45,70)    (-3,1) (-1,1) (0.5,0)

Tbl.Zh.Zdr.Rh    (45.0,99.0)   (1,0) (1.4,1) (5.,1) (6,0)

Tbl.Zh.Zdr.Gsh     (25.0,27.0)   (-0.3,0) (-0.1,1) (0.0000,1) (0.3000,0)
Tbl.Zh.Zdr.Gsh     (27.0,29.0)   (-0.3,0) (-0.1,1) (0.0000,1) (0.3000,0)
Tbl.Zh.Zdr.Gsh     (29.0,31.0)   (-0.3,0) (-0.1,1) (0.0096,1) (0.3096,0)
Tbl.Zh.Zdr.Gsh     (31.0,33.0)   (-0.3,0) (-0.1,1) (0.0382,1) (0.3382,0)
Tbl.Zh.Zdr.Gsh     (33.0,35.0)   (-0.3,0) (-0.1,1) (0.0860,1) (0.3860,0)
Tbl.Zh.Zdr.Gsh     (35.0,37.0)   (-0.3,0) (-0.1,1) (0.1528,1) (0.4528,0)
Tbl.Zh.Zdr.Gsh     (37.0,39.0)   (-0.3,0) (-0.1,1) (0.2388,1) (0.5388,0)
Tbl.Zh.Zdr.Gsh     (39.0,41.0)   (-0.3,0) (-0.1,1) (0.3438,1) (0.6438,0)
Tbl.Zh.Zdr.Gsh     (41.0,43.0)   (-0.3,0) (-0.1,1) (0.4680,1) (0.7680,0)
Tbl.Zh.Zdr.Gsh     (43.0,45.0)   (-0.3,0) (-0.1,1) (0.6112,1) (0.9112,0)
Tbl.Zh.Zdr.Gsh     (45.0,47.0)   (-0.3,0) (-0.1,1) (0.7628,1) (1.0628,0)

#Tbl.Zh.Zdr.GRR    (25.0,27.0)   (0.5,0) (0.7,1) (0.7000,1) (1.0000,0)
#Tbl.Zh.Zdr.GRR    (27.0,29.0)   (0.5,0) (0.7,1) (0.7000,1) (1.0000,0)
#Tbl.Zh.Zdr.GRR    (29.0,31.0)   (0.5,0) (0.7,1) (0.7132,1) (1.0132,0)
#Tbl.Zh.Zdr.GRR    (31.0,33.0)   (0.5,0) (0.7,1) (0.7529,1) (1.0529,0)
#Tbl.Zh.Zdr.GRR    (33.0,35.0)   (0.5,0) (0.7,1) (0.8190,1) (1.1190,0)
Tbl.Zh.Zdr.GRR     (35.0,55.0)   (0.5,0) (0.8,1) (4,1) (6,0)

Tbl.Zh.Zdr.Ds     (10,35)   (-1.0,0) (0.0,1) (1.1,1) (1.4,0)
Tbl.Zh.Zdr.Ws     (-5,50)   (0.3,0) (0.5,1) (3.00,1) (3.25,0)
Tbl.Zh.Zdr.Ic     (-10,30)   (0.8,0) (1.0,1) (6,1) (7,0)
Tbl.Zh.Zdr.Iic    (-10,30)  (-.5,0) (0.0,1) (0.7,1) (1.0,0)

Tbl.Zh.Zdr.Sld    (-20.0,-8.0)   (-0.3000,0) (0.0000,1) (0.3,0)
Tbl.Zh.Zdr.Sld    (-8.0,-6.0)   (-0.3000,0) (0.0000,1) (0.31,0)
Tbl.Zh.Zdr.Sld    (-6.0,-4.0)   (-0.3000,0) (0.0000,1) (0.33,0)
Tbl.Zh.Zdr.Sld    (-4.0,-2.0)   (-0.3000,0) (0.0000,1) (0.35,0)
Tbl.Zh.Zdr.Sld    (-2.0,0.0)   (-0.3000,0) (0.0000,1) (0.37,0)
Tbl.Zh.Zdr.Sld    (0.0,2.0)   (-0.3000,0) (0.0000,1) (0.3710,0) 
Tbl.Zh.Zdr.Sld    (2.0,4.0)   (-0.3000,0) (0.0000,1) (0.3576,0)
Tbl.Zh.Zdr.Sld    (4.0,6.0)   (-0.3000,0) (0.0000,1) (0.3546,0)
Tbl.Zh.Zdr.Sld    (6.0,8.0)   (-0.3000,0) (0.0000,1) (0.3620,0)
Tbl.Zh.Zdr.Sld    (8.0,10.0)   (-0.3000,0) (0.0000,1) (0.3798,0)
Tbl.Zh.Zdr.Sld    (10.0,12.0)   (-0.3000,0) (0.0000,1) (0.4080,0)
Tbl.Zh.Zdr.Sld    (12.0,14.0)   (-0.3000,0) (0.0000,1) (0.4466,0) 
Tbl.Zh.Zdr.Sld    (14.0,16.0)   (-0.3000,0) (0.0000,1) (0.4956,0) 
Tbl.Zh.Zdr.Sld    (16.0,18.0)   (-0.3000,0) (0.0000,1) (0.5550,0)
Tbl.Zh.Zdr.Sld    (18.0,20.0)   (-0.3000,0) (0.0000,1) (0.6248,0)
Tbl.Zh.Zdr.Sld    (19.0,21.0)   (-0.3000,0) (0.0000,1) (0.6636,0)
Tbl.Zh.Zdr.Sld    (21.0,23.0)   (-0.3000,0) (0.0000,1) (0.7490,0)
Tbl.Zh.Zdr.Sld    (23.0,25.0)   (-0.3000,0) (0.0000,1) (0.8448,0)
Tbl.Zh.Zdr.Sld    (25.0,27.0)   (-0.3000,0) (0.0000,1) (0.9510,0) 
Tbl.Zh.Zdr.Sld    (27.0,29.0)   (-0.3000,0) (0.0000,1) (1.0676,0)
Tbl.Zh.Zdr.Sld    (29.0,31.0)   (-0.2868,0) (0.0132,1) (1.1946,0)
Tbl.Zh.Zdr.Sld    (31.0,33.0)   (-0.2471,0) (0.0529,1) (1.3320,0)
Tbl.Zh.Zdr.Sld    (33.0,35.0)   (-0.1810,0) (0.1190,1) (1.4798,0)

Tbl.Zh.Zdr.Bgs    (-20,-2)   (2,0) (3,1) (12,1)
Tbl.Zh.Zdr.Bgs    (-2,0)    (4,0) (5,1) (12,1)
Tbl.Zh.Zdr.Bgs    (0,2)     (5,0) (6,1) (12,1)
Tbl.Zh.Zdr.Bgs    (2,35)    (6,0) (7,1) (12,1)
Tbl.Zh.Zdr.Trip2  (-20,35)  (-3,1) (0,1) (1,0) (7,0)
Tbl.Zh.Zdr.Gcl    (-20,70)   (-10,1) (5,1) (10,0)
#
# Membership functions for LDR
#

Tbl.Zh.Ldr.CL      (-20,6)    (-35,1) (-33,1) (-30,1) (-28,0)
Tbl.Zh.Ldr.Drz     (0,20)     (-35,1) (-33,1) (-30,1) (-28,0)
Tbl.Zh.Ldr.Lr      (20,40)    (-35,1) (-33,1) (-27,1) (-25,0)

Tbl.Zh.Ldr.Mr      (30.0,32.0)   (-31.5,0) (-31,1) (-27.2143,1) (-25.2143,0)
Tbl.Zh.Ldr.Mr      (32.0,34.0)   (-31.5,0) (-31,1) (-26.9286,1) (-24.9286,0)
Tbl.Zh.Ldr.Mr      (34.0,36.0)   (-31.5,0) (-31,1) (-26.6429,1) (-24.6429,0)
Tbl.Zh.Ldr.Mr      (36.0,38.0)   (-31.5,0) (-31,1) (-26.3571,1) (-24.3571,0)
Tbl.Zh.Ldr.Mr      (38.0,40.0)   (-31.5,0) (-31,1) (-26.0714,1) (-24.0714,0)
Tbl.Zh.Ldr.Mr      (40.0,42.0)   (-31.5,0) (-31,1) (-25.7857,1) (-24.0000,0)
Tbl.Zh.Ldr.Mr      (42.0,44.0)   (-31.5,0) (-31,1) (-25.5000,1) (-24.0000,0)
Tbl.Zh.Ldr.Mr      (44.0,46.0)   (-31.5,0) (-31,1) (-25.2143,1) (-23.0000,0)
Tbl.Zh.Ldr.Mr      (46.0,48.0)   (-31.5,0) (-31,1) (-25.0000,1) (-23.0000,0)
Tbl.Zh.Ldr.Mr      (48.0,50.0)   (-31.5,0) (-31,1) (-24.8510,1) (-23.0000,0)


Tbl.Zh.Ldr.Hr    (40.0,42.0)   (-31.5,0) (-31,1) (-25.7857,1) (-24.0000,0)
Tbl.Zh.Ldr.Hr    (42.0,44.0)   (-31.5,0) (-31,1) (-25.5000,1) (-24.0000,0)
Tbl.Zh.Ldr.Hr    (44.0,46.0)   (-31.5,0) (-31,1) (-25.2143,1) (-23.0000,0)
Tbl.Zh.Ldr.Hr    (46.0,48.0)   (-31.5,0) (-31,1) (-25.0000,1) (-23.0000,0)
Tbl.Zh.Ldr.Hr    (48.0,50.0)   (-31.5,0) (-31,1) (-24.8510,1) (-23.0000,0)
Tbl.Zh.Ldr.Hr    (50.0,52.0)   (-31.5,0) (-31,1) (-24.7112,1) (-23.0000,0)
Tbl.Zh.Ldr.Hr    (52.0,54.0)   (-31.5,0) (-31,1) (-24.5000,1) (-23.0000,0)
Tbl.Zh.Ldr.Hr    (54.0,56.0)   (-31.5,0) (-31,1) (-24.5000,1) (-23.0000,0)
Tbl.Zh.Ldr.Hr    (56.0,58.0)   (-31.5,0) (-31,1) (-24.5000,1) (-23.0000,0)
Tbl.Zh.Ldr.Hr    (58.0,60.0)   (-31.5,0) (-31,1) (-24.5000,1) (-23.0000,0)

Tbl.Zh.Ldr.Ha    (45.0,47.0)   (-27,0) (-25,1) (-20.0000,1) (-18.0000,0)
Tbl.Zh.Ldr.Ha    (47.0,49.0)   (-27,0) (-25,1) (-19.2000,1) (-17.2000,0)
Tbl.Zh.Ldr.Ha    (49.0,51.0)   (-27,0) (-25,1) (-18.4000,1) (-16.4000,0)
Tbl.Zh.Ldr.Ha    (51.0,53.0)   (-27,0) (-25,1) (-17.6000,1) (-15.6000,0)
Tbl.Zh.Ldr.Ha    (53.0,55.0)   (-27,0) (-25,1) (-16.8000,1) (-14.8000,0)
Tbl.Zh.Ldr.Ha    (55.0,57.0)   (-27,0) (-25,1) (-16.0000,1) (-14.0000,0)
Tbl.Zh.Ldr.Ha    (57.0,59.0)   (-27,0) (-25,1) (-15.2000,1) (-13.2000,0)
Tbl.Zh.Ldr.Ha    (59.0,61.0)   (-27,0) (-25,1) (-14.4000,1) (-12.4000,0)
Tbl.Zh.Ldr.Ha    (61.0,63.0)   (-27,0) (-25,1) (-13.6000,1) (-11.6000,0)
Tbl.Zh.Ldr.Ha    (63.0,65.0)   (-27,0) (-25,1) (-12.8000,1) (-10.8000,0)
Tbl.Zh.Ldr.Ha    (65.0,67.0)   (-27,0) (-25,1) (-12.0000,1) (-10.0000,0)
Tbl.Zh.Ldr.Ha    (67.0,69.0)   (-27,0) (-25,1) (-11.2000,1) (-9.2000,0)
Tbl.Zh.Ldr.Ha    (69.0,71.0)   (-27,0) (-25,1) (-10.4000,1) (-8.4000,0)

Tbl.Zh.Ldr.Rh    (45.0,75.0)   (-27.0,0) (-25,1) (-17.,1) (-14,0)

Tbl.Zh.Ldr.Gsh   (25.0,27.0)   (-30.7500,0) (-25,1) (-24.8333,1) (-22.8333,0)
Tbl.Zh.Ldr.Gsh   (27.0,29.0)   (-30.4900,0) (-25,1) (-24.5000,1) (-22.5000,0)
Tbl.Zh.Ldr.Gsh   (29.0,31.0)   (-30.2300,0) (-25,1) (-24.1667,1) (-22.1667,0)
Tbl.Zh.Ldr.Gsh   (31.0,33.0)   (-29.9700,0) (-25,1) (-23.8333,1) (-21.8333,0)
Tbl.Zh.Ldr.Gsh   (33.0,35.0)   (-29.7100,0) (-25,1) (-23.5000,1) (-21.5000,0)
Tbl.Zh.Ldr.Gsh   (35.0,37.0)   (-29.4500,0) (-25,1) (-23.1667,1) (-21.1667,0)
Tbl.Zh.Ldr.Gsh   (37.0,39.0)   (-29.1900,0) (-25,1) (-22.8333,1) (-20.8333,0)
Tbl.Zh.Ldr.Gsh   (39.0,41.0)   (-28.9300,0) (-25,1) (-22.5000,1) (-20.5000,0)
Tbl.Zh.Ldr.Gsh   (41.0,43.0)   (-28.6700,0) (-25,1) (-22.1667,1) (-20.1667,0)
Tbl.Zh.Ldr.Gsh   (43.0,45.0)   (-28.4100,0) (-24,1) (-21.8333,1) (-19.8333,0)
Tbl.Zh.Ldr.Gsh   (45.0,47.0)   (-28.1500,0) (-24,1) (-21.5000,1) (-19.5000,0)
Tbl.Zh.Ldr.Gsh   (47.0,49.0)   (-27.8900,0) (-24,1) (-21.1667,1) (-19.1667,0)
Tbl.Zh.Ldr.Gsh   (49.0,51.0)   (-27.6300,0) (-24,1) (-20.8333,1) (-18.8333,0)
Tbl.Zh.Ldr.Gsh   (51.0,53.0)   (-27.3700,0) (-23,1) (-20.5000,1) (-18.5000,0)
Tbl.Zh.Ldr.Gsh   (53.0,55.0)   (-27.1100,0) (-23,1) (-20.1667,1) (-18.1667,0)

#Tbl.Zh.Ldr.GRR   (25.0,27.0)   (-32.7500,0) (-27,1) (-26.8333,1) (-24.8333,0)
#Tbl.Zh.Ldr.GRR   (27.0,29.0)   (-32.4900,0) (-27,1) (-26.5000,1) (-24.5000,0)
#Tbl.Zh.Ldr.GRR   (29.0,31.0)   (-32.2300,0) (-27,1) (-26.1667,1) (-24.1667,0)
#Tbl.Zh.Ldr.GRR   (31.0,33.0)   (-31.9700,0) (-27,1) (-25.8333,1) (-23.8333,0)
#Tbl.Zh.Ldr.GRR   (33.0,35.0)   (-31.7100,0) (-27,1) (-25.5000,1) (-23.5000,0)
Tbl.Zh.Ldr.GRR    (25.0,55.0)   (-27.0,0) (-25,1) (-20.,1) (-17,0)

Tbl.Zh.Ldr.Ds    (10,35)    (-28,0) (-26,1) (-23,1) (-21,0)

Tbl.Zh.Ldr.Ws    (-5.0,51.0)   (-26,0) (-25.5,1) (-17.2000,1) (-15.2000,0)

Tbl.Zh.Ldr.Ic    (-10.0,-8.0)   (-32,0)        (-31.0000,1) (-29.0000,0)
Tbl.Zh.Ldr.Ic    (-8.0,-6.0)   (-32,0) (-31,1) (-30.6000,1) (-28.6000,0)
Tbl.Zh.Ldr.Ic    (-6.0,-4.0)   (-32,0) (-31,1) (-30.2000,1) (-28.2000,0)
Tbl.Zh.Ldr.Ic    (-4.0,-2.0)   (-32,0) (-31,1) (-29.8000,1) (-27.8000,0)
Tbl.Zh.Ldr.Ic    (-2.0,0.0)   (-32,0) (-31,1) (-29.4000,1) (-27.4000,0)
Tbl.Zh.Ldr.Ic    (0.0,2.0)   (-32,0) (-31,1) (-29.0000,1) (-27.0000,0)
Tbl.Zh.Ldr.Ic    (2.0,4.0)   (-32,0) (-31,1) (-28.6000,1) (-26.6000,0)
Tbl.Zh.Ldr.Ic    (4.0,6.0)   (-32,0) (-31,1) (-28.2000,1) (-26.2000,0)
Tbl.Zh.Ldr.Ic    (6.0,8.0)   (-32,0) (-31,1) (-27.8000,1) (-25.8000,0)
Tbl.Zh.Ldr.Ic    (8.0,10.0)   (-32,0) (-31,1) (-27.4000,1) (-25.4000,0)
Tbl.Zh.Ldr.Ic    (10.0,12.0)   (-32,0) (-31,1) (-27.0000,1) (-25.0000,0)
Tbl.Zh.Ldr.Ic    (12.0,14.0)   (-32,0) (-31,1) (-26.6000,1) (-24.6000,0)
Tbl.Zh.Ldr.Ic    (14.0,16.0)   (-32,0) (-31,1) (-26.2000,1) (-24.2000,0)
Tbl.Zh.Ldr.Ic    (16.0,18.0)   (-32,0) (-31,1) (-25.8000,1) (-23.8000,0)
Tbl.Zh.Ldr.Ic    (18.0,20.0)   (-32,0) (-31,1) (-25.4000,1) (-23.4000,0)
Tbl.Zh.Ldr.Ic    (20.0,22.0)   (-32,0) (-31,1) (-25.0000,1) (-23.0000,0)
Tbl.Zh.Ldr.Ic    (22.0,24.0)   (-32,0) (-31,1) (-24.6000,1) (-23.0000,0)
Tbl.Zh.Ldr.Ic    (24.0,26.0)   (-32,0) (-31,1) (-24.2000,1) (-23.0000,0)
Tbl.Zh.Ldr.Ic    (26.0,28.0)   (-32,0) (-31,1) (-23.8000,1) (-23.0000,0)
Tbl.Zh.Ldr.Ic    (28.0,30.0)   (-32,0) (-31,1) (-23.4000,1) (-23.0000,0)

#Tbl.Zh.Ldr.Iic    (-10.0,30.0)   (-28,0) (-26,1) (-23,1) (-21,0)

Tbl.Zh.Ldr.Iic    (-20.0,-8.0)   (-32,0)        (-31.0000,1) (-29.0000,0)
Tbl.Zh.Ldr.Iic    (-8.0,-6.0)   (-32,0) (-31,1) (-30.6000,1) (-28.6000,0)
Tbl.Zh.Ldr.Iic    (-6.0,-4.0)   (-32,0) (-31,1) (-30.2000,1) (-28.2000,0)
Tbl.Zh.Ldr.Iic    (-4.0,-2.0)   (-32,0) (-31,1) (-29.8000,1) (-27.8000,0)
Tbl.Zh.Ldr.Iic    (-2.0,0.0)   (-32,0) (-31,1) (-29.4000,1) (-27.4000,0)
Tbl.Zh.Ldr.Iic    (0.0,2.0)   (-32,0) (-31,1) (-29.0000,1) (-27.0000,0)
Tbl.Zh.Ldr.Iic    (2.0,4.0)   (-32,0) (-31,1) (-28.6000,1) (-26.6000,0)
Tbl.Zh.Ldr.Iic    (4.0,6.0)   (-32,0) (-31,1) (-28.2000,1) (-26.2000,0)
Tbl.Zh.Ldr.Iic    (6.0,8.0)   (-32,0) (-31,1) (-27.8000,1) (-25.8000,0)
Tbl.Zh.Ldr.Iic    (8.0,10.0)   (-32,0) (-31,1) (-27.4000,1) (-25.4000,0)
Tbl.Zh.Ldr.Iic    (10.0,12.0)   (-32,0) (-31,1) (-27.0000,1) (-25.0000,0)
Tbl.Zh.Ldr.Iic    (12.0,14.0)   (-32,0) (-31,1) (-26.6000,1) (-24.6000,0)
Tbl.Zh.Ldr.Iic    (14.0,16.0)   (-32,0) (-31,1) (-26.2000,1) (-24.2000,0)
Tbl.Zh.Ldr.Iic    (16.0,18.0)   (-32,0) (-31,1) (-25.8000,1) (-23.8000,0)
Tbl.Zh.Ldr.Iic    (18.0,20.0)   (-32,0) (-31,1) (-25.4000,1) (-23.4000,0)
Tbl.Zh.Ldr.Iic    (20.0,22.0)   (-32,0) (-31,1) (-25.0000,1) (-23.0000,0)
Tbl.Zh.Ldr.Iic    (22.0,24.0)   (-32,0) (-31,1) (-24.6000,1) (-23.0000,0)
Tbl.Zh.Ldr.Iic    (24.0,26.0)   (-32,0) (-31,1) (-24.2000,1) (-23.0000,0)
Tbl.Zh.Ldr.Iic    (26.0,28.0)   (-32,0) (-31,1) (-23.8000,1) (-23.0000,0)
Tbl.Zh.Ldr.Iic    (28.0,30.0)   (-32,0) (-31,1) (-23.4000,1) (-23.0000,0)

Tbl.Zh.Ldr.Sld    (-20,0)    (-35,1) (-33,1) (-30,1) (-28,0)
Tbl.Zh.Ldr.Sld    (0,20)     (-35,1) (-33,1) (-30,1) (-28,0)
Tbl.Zh.Ldr.Sld    (20,30)    (-35,1) (-33,1) (-27,1) (-25,0)

Tbl.Zh.Ldr.Bgs    (-20,35)   (-24,0) (-20,1) (-10,1) (-5,0)
Tbl.Zh.Ldr.Trip2  (-20,35)   (-30,0) (0,0) (1,1) (40,1)
Tbl.Zh.Ldr.Gcl    (-20,70)   (-20,0) (-18,1) (5,1)
#
# Membership functions for KDP
#
Tbl.Zh.Kdp.CL    (-20.0,-8.0)   (-0.0500,0) (-0.0300,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.CL    (-8.0,-6.0)   (-0.0500,0) (-0.0300,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.CL    (-6.0,-4.0)   (-0.0500,0) (-0.0300,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.CL    (-4.0,-2.0)   (-0.0500,0) (-0.0300,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.CL    (-2.0,6.0)   (-0.0499,0) (-0.0299,1) (0.0300,1) (0.0500,0)

Tbl.Zh.Kdp.Drz   (0.0,2.0)   (-0.0499,0) (-0.0299,1) (0.0301,1) (0.0501,0)
Tbl.Zh.Kdp.Drz   (2.0,4.0)   (-0.0499,0) (-0.0299,1) (0.0301,1) (0.0501,0)
Tbl.Zh.Kdp.Drz   (4.0,6.0)   (-0.0498,0) (-0.0298,1) (0.0302,1) (0.0502,0)
Tbl.Zh.Kdp.Drz   (6.0,8.0)   (-0.0498,0) (-0.0298,1) (0.0302,1) (0.0502,0)
Tbl.Zh.Kdp.Drz   (8.0,10.0)   (-0.0497,0) (-0.0297,1) (0.0304,1) (0.0504,0)
Tbl.Zh.Kdp.Drz   (10.0,12.0)   (-0.0495,0) (-0.0295,1) (0.0305,1) (0.0505,0)
Tbl.Zh.Kdp.Drz   (12.0,14.0)   (-0.0493,0) (-0.0293,1) (0.0308,1) (0.0508,0)
Tbl.Zh.Kdp.Drz   (14.0,16.0)   (-0.0489,0) (-0.0289,1) (0.0312,1) (0.0512,0)
Tbl.Zh.Kdp.Drz   (16.0,18.0)   (-0.0484,0) (-0.0284,1) (0.0319,1) (0.0519,0)
Tbl.Zh.Kdp.Drz   (18.0,20.0)   (-0.0477,0) (-0.0277,1) (0.0329,1) (0.0529,0)

Tbl.Zh.Kdp.Lr    (19.0,21.0)   (-0.0473,0) (-0.0273,1) (0.0335,1) (0.0535,0)
Tbl.Zh.Kdp.Lr    (21.0,23.0)   (-0.0460,0) (-0.0260,1) (0.0354,1) (0.0554,0)
Tbl.Zh.Kdp.Lr    (23.0,25.0)   (-0.0442,0) (-0.0242,1) (0.0382,1) (0.0582,0)
Tbl.Zh.Kdp.Lr    (25.0,27.0)   (-0.0415,0) (-0.0215,1) (0.0424,1) (0.0624,0)
Tbl.Zh.Kdp.Lr    (27.0,29.0)   (-0.0376,0) (-0.0176,1) (0.0489,1) (0.0689,0)
Tbl.Zh.Kdp.Lr    (29.0,31.0)   (-0.0319,0) (-0.0119,1) (0.0588,1) (0.0788,0)
Tbl.Zh.Kdp.Lr    (31.0,33.0)   (-0.0236,0) (-0.0036,1) (0.0738,1) (0.0938,0)
Tbl.Zh.Kdp.Lr    (33.0,35.0)   (-0.0115,0) (0.0085,1) (0.0965,1) (0.1165,0)
Tbl.Zh.Kdp.Lr    (35.0,37.0)   (0.0062,0) (0.0262,1) (0.1312,1) (0.1512,0)
Tbl.Zh.Kdp.Lr    (37.0,39.0)   (0.0320,0) (0.0520,1) (0.1838,1) (0.2038,0)
Tbl.Zh.Kdp.Lr    (39.0,41.0)   (0.0697,0) (0.0897,1) (0.2639,1) (0.2839,0)

Tbl.Zh.Kdp.Mr      (29.0,31.0)   (-0.0319,0) (-0.0119,1) (0.1288,1) (0.1488,0)
Tbl.Zh.Kdp.Mr      (31.0,33.0)   (-0.0236,0) (-0.0036,1) (0.1438,1) (0.1638,0)
Tbl.Zh.Kdp.Mr      (33.0,35.0)   (-0.0115,0) (0.0085,1) (0.1665,1) (0.1865,0)
Tbl.Zh.Kdp.Mr      (35.0,37.0)   (0.0062,0) (0.0262,1) (0.2012,1) (0.2212,0)
Tbl.Zh.Kdp.Mr      (37.0,39.0)   (0.0320,0) (0.0520,1) (0.2538,1) (0.2738,0)
Tbl.Zh.Kdp.Mr      (39.0,41.0)   (0.0697,0) (0.0897,1) (0.3339,1) (0.3539,0)
Tbl.Zh.Kdp.Mr      (41.0,43.0)   (0.1246,0) (0.1446,1) (0.4556,1) (0.4756,0)
Tbl.Zh.Kdp.Mr      (43.0,45.0)   (0.2047,0) (0.2247,1) (0.6408,1) (0.6608,0)
Tbl.Zh.Kdp.Mr      (45.0,47.0)   (0.3215,0) (0.3415,1) (0.9222,1) (0.9422,0)
Tbl.Zh.Kdp.Mr      (47.0,49.0)   (0.4920,0) (0.5120,1) (1.3503,1) (1.3703,0)
Tbl.Zh.Kdp.Mr      (49.0,51.0)   (0.7407,0) (0.7607,1) (2.0011,1) (2.0211,0)
Tbl.Zh.Kdp.Mr      (51.0,53.0)   (1.1035,0) (1.1235,1) (2.9907,1) (3.0107,0)

Tbl.Zh.Kdp.Hr      (39.0,41.0)   (0.0697,0) (0.0897,1) (0.3339,1) (0.3539,0)
Tbl.Zh.Kdp.Hr      (41.0,43.0)   (0.1246,0) (0.1446,1) (0.4556,1) (0.4756,0)
Tbl.Zh.Kdp.Hr      (43.0,45.0)   (0.2047,0) (0.2247,1) (0.6408,1) (0.6608,0)
Tbl.Zh.Kdp.Hr      (45.0,47.0)   (0.3215,0) (0.3415,1) (0.9222,1) (0.9422,0)
Tbl.Zh.Kdp.Hr      (47.0,49.0)   (0.4920,0) (0.5120,1) (1.3503,1) (1.3703,0)
Tbl.Zh.Kdp.Hr      (49.0,51.0)   (0.7407,0) (0.7607,1) (2.0011,1) (2.0211,0)
Tbl.Zh.Kdp.Hr      (51.0,53.0)   (1.1035,0) (1.1235,1) (2.9907,1) (3.0107,0)
Tbl.Zh.Kdp.Hr      (53.0,55.0)   (1.6327,0) (1.6527,1) (4.4954,1) (4.5154,0)
Tbl.Zh.Kdp.Hr      (55.0,57.0)   (2.4047,0) (2.4247,1) (6.7834,1) (6.8034,0)
Tbl.Zh.Kdp.Hr      (57.0,59.0)   (3.5310,0) (3.5510,1) (10.2625,1) (10.2825,0)
Tbl.Zh.Kdp.Hr      (59.0,61.0)   (5.1740,0) (5.1940,1) (15.5525,1) (15.5725,0)

Tbl.Zh.Kdp.Ha    (45,99)    (-0.3,0)  (0,1) (0.2,1) (0.4,0)

Tbl.Zh.Kdp.Rh    (45.0,75.0)   (0.3,0) (1.0,1) (5.0,1) (6.5,0) 

Tbl.Zh.Kdp.Gsh  (25.0,27.0)   (0.0,0) (0.08,1) (0.1000,1) (0.1785,0)
Tbl.Zh.Kdp.Gsh  (27.0,29.0)   (0.0,0) (0.08,1) (0.1000,1) (0.1824,0)
Tbl.Zh.Kdp.Gsh  (29.0,31.0)   (0.0,0) (0.08,1) (0.1000,1) (0.1881,0)
Tbl.Zh.Kdp.Gsh  (31.0,33.0)   (0.0,0) (0.08,1) (0.1000,1) (0.1964,0)
Tbl.Zh.Kdp.Gsh  (33.0,35.0)   (0.0,0) (0.08,1) (0.1000,1) (0.2085,0)
Tbl.Zh.Kdp.Gsh  (35.0,37.0)   (0.0,0) (0.08,1) (0.1000,1) (0.2262,0)
Tbl.Zh.Kdp.Gsh  (37.0,39.0)   (0.0,0) (0.08,1) (0.1000,1) (0.2520,0)
Tbl.Zh.Kdp.Gsh  (39.0,41.0)   (0.0,0) (0.08,1) (0.1000,1) (0.2897,0)
Tbl.Zh.Kdp.Gsh  (41.0,43.0)   (0.0,0) (0.08,1) (0.1446,1) (0.3446,0)
Tbl.Zh.Kdp.Gsh  (43.0,45.0)   (0.0,0) (0.08,1) (0.2247,1) (0.4247,0)
Tbl.Zh.Kdp.Gsh  (45.0,47.0)   (0.0,0) (0.08,1) (0.3415,1) (0.5415,0)
Tbl.Zh.Kdp.Gsh  (47.0,49.0)   (0.0,0) (0.08,1) (0.5120,1) (0.7120,0)
Tbl.Zh.Kdp.Gsh  (49.0,51.0)   (0.0,0) (0.08,1) (0.7607,1) (0.9607,0)
Tbl.Zh.Kdp.Gsh  (51.0,53.0)   (0.0,0) (0.08,1) (1.1235,1) (1.3235,0)
Tbl.Zh.Kdp.Gsh  (53.0,55.0)   (0.0,0) (0.08,1) (1.6527,1) (1.8527,0)

#Tbl.Zh.Kdp.Gsh    (25.0,55.0)   (0.3,0) (0.5,1) (1.2,1) (1.5,0) 

Tbl.Zh.Kdp.GRR    (25.0,27.0)   (0.0,0)         (0.1000,1) (0.1200,0)
Tbl.Zh.Kdp.GRR    (27.0,29.0)   (0.0,0)         (0.1000,1) (0.1200,0)
Tbl.Zh.Kdp.GRR    (29.0,31.0)   (0.0,0)         (0.1000,1) (0.1200,0)
Tbl.Zh.Kdp.GRR    (31.0,33.0)   (0.0,0)         (0.1000,1) (0.1200,0)
Tbl.Zh.Kdp.GRR    (33.0,35.0)   (0.0,0) (0.1,1) (0.1085,1) (0.1200,0)
Tbl.Zh.Kdp.GRR    (35.0,37.0)   (0.0,0) (0.1,1) (0.1262,1) (0.1272,0)
Tbl.Zh.Kdp.GRR    (37.0,39.0)   (0.0,0) (0.1,1) (0.1520,1) (0.1737,0)
Tbl.Zh.Kdp.GRR    (39.0,41.0)   (0.0,0) (0.1,1) (0.1897,1) (0.2414,0)
Tbl.Zh.Kdp.GRR    (41.0,43.0)   (0.0,0) (0.1,1) (0.2446,1) (0.3402,0)
Tbl.Zh.Kdp.GRR    (43.0,45.0)   (0.0,0) (0.1,1) (0.3247,1) (0.4844,0)
Tbl.Zh.Kdp.GRR    (45.0,47.0)   (0.0,0) (0.1,1) (0.4415,1) (0.6948,0)
Tbl.Zh.Kdp.GRR    (47.0,49.0)   (0.0,0) (0.1,1) (0.6120,1) (1.0016,0)
Tbl.Zh.Kdp.GRR    (49.0,51.0)   (0.0,0) (0.1,1) (0.8607,1) (1.4492,0)
Tbl.Zh.Kdp.GRR    (51.0,53.0)   (0.0,0) (0.1,1) (1.2235,1) (2.1022,0)
Tbl.Zh.Kdp.GRR    (53.0,55.0)   (0.0,0) (0.1,1) (1.7527,1) (3.0548,0)

Tbl.Zh.Kdp.Ds    (10.0,12.0)   (-0.1,0) (0.0,1) (0.1200,1) (0.1700,0)
Tbl.Zh.Kdp.Ds    (12.0,14.0)   (-0.1,0) (0.0,1) (0.1240,1) (0.1740,0)
Tbl.Zh.Kdp.Ds    (14.0,16.0)   (-0.1,0) (0.0,1) (0.1280,1) (0.1780,0)
Tbl.Zh.Kdp.Ds    (16.0,18.0)   (-0.1,0) (0.0,1) (0.1320,1) (0.1820,0)
Tbl.Zh.Kdp.Ds    (18.0,20.0)   (-0.1,0) (0.0,1) (0.1360,1) (0.1860,0)
Tbl.Zh.Kdp.Ds    (20.0,22.0)   (-0.1,0) (0.0,1) (0.1400,1) (0.1900,0)
Tbl.Zh.Kdp.Ds    (22.0,24.0)   (-0.1,0) (0.0,1) (0.1440,1) (0.1940,0)
Tbl.Zh.Kdp.Ds    (24.0,26.0)   (-0.1,0) (0.0,1) (0.1480,1) (0.1980,0)
Tbl.Zh.Kdp.Ds    (26.0,28.0)   (-0.1,0) (0.0,1) (0.1520,1) (0.2020,0)
Tbl.Zh.Kdp.Ds    (28.0,30.0)   (-0.1,0) (0.0,1) (0.1560,1) (0.2060,0)
Tbl.Zh.Kdp.Ds    (30.0,32.0)   (-0.1,0) (0.0,1) (0.1600,1) (0.2100,0)
Tbl.Zh.Kdp.Ds    (32.0,34.0)   (-0.1,0) (0.0,1) (0.1640,1) (0.2140,0)
Tbl.Zh.Kdp.Ds    (34.0,36.0)   (-0.1,0) (0.0,1) (0.1680,1) (0.2180,0)

#Tbl.Zh.Kdp.Ws   (15.0,17.0)   (-0.05,0) (0.0,1) (0.1300,1) (0.1800,0)
#Tbl.Zh.Kdp.Ws   (17.0,19.0)   (-0.05,0) (0.0,1) (0.1340,1) (0.1840,0)
#Tbl.Zh.Kdp.Ws   (19.0,21.0)   (-0.05,0) (0.0,1) (0.1380,1) (0.1880,0)
#Tbl.Zh.Kdp.Ws   (21.0,23.0)   (-0.05,0) (0.0,1) (0.1420,1) (0.1920,0)
#Tbl.Zh.Kdp.Ws   (23.0,25.0)   (-0.05,0) (0.0,1) (0.1460,1) (0.1960,0)
#Tbl.Zh.Kdp.Ws   (25.0,27.0)   (-0.05,0) (0.0,1) (0.1500,1) (0.2000,0)
#Tbl.Zh.Kdp.Ws   (27.0,29.0)   (-0.05,0) (0.0,1) (0.1540,1) (0.2040,0)
#Tbl.Zh.Kdp.Ws   (29.0,31.0)   (-0.05,0) (0.0,1) (0.1580,1) (0.2080,0)
#Tbl.Zh.Kdp.Ws   (31.0,33.0)   (-0.05,0) (0.0,1) (0.1620,1) (0.2120,0)
#Tbl.Zh.Kdp.Ws   (33.0,35.0)   (-0.05,0) (0.0,1) (0.1660,1) (0.2160,0)

Tbl.Zh.Kdp.Ws    (-5.0,50.0)   (-0.05,0) (0.1,1) (1.0,1) (1.2,0)

Tbl.Zh.Kdp.Ic    (-10.0,-8.0)   (-0.0200,0) (0.0800,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (-8.0,-6.0)   (-0.0160,0) (0.0840,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (-6.0,-4.0)   (-0.0120,0) (0.0880,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (-4.0,-2.0)   (-0.0080,0) (0.0920,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (-2.0,0.0)   (-0.0040,0) (0.0960,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (0.0,2.0)   (0.0000,0) (0.1000,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (2.0,4.0)   (0.0040,0) (0.1040,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (4.0,6.0)   (0.0080,0) (0.1080,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (6.0,8.0)   (0.0120,0) (0.1120,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (8.0,10.0)   (0.0160,0) (0.1160,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (10.0,12.0)   (0.0200,0) (0.1200,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (12.0,14.0)   (0.0240,0) (0.1240,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (14.0,16.0)   (0.0280,0) (0.1280,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (16.0,18.0)   (0.0320,0) (0.1320,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (18.0,20.0)   (0.0360,0) (0.1360,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (20.0,22.0)   (0.0400,0) (0.1400,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (22.0,24.0)   (0.0440,0) (0.1440,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (24.0,26.0)   (0.0480,0) (0.1480,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (26.0,28.0)   (0.0520,0) (0.1520,1) (0.6,1) (0.7,0)
Tbl.Zh.Kdp.Ic    (28.0,30.0)   (0.0560,0) (0.1560,1) (0.6,1) (0.7,0)

Tbl.Zh.Kdp.Iic    (-10,30.0)    (-0.1,0) (0.0,1) (0.1,1) (0.2,0)

Tbl.Zh.Kdp.Sld    (-20.0,-8.0)   (-0.05,0) (0.0,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.Sld    (-8.0,-6.0)   (-0.05,0) (0.0,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.Sld    (-6.0,-4.0)   (-0.05,0) (0.0,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.Sld    (-4.0,-2.0)   (-0.05,0) (0.0,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.Sld    (-2.0,0.0)   (-0.05,0) (0.0,1) (0.0300,1) (0.0500,0)
Tbl.Zh.Kdp.Sld    (0.0,2.0)   (-0.05,0) (0.0,1) (0.0301,1) (0.0501,0)
Tbl.Zh.Kdp.Sld    (2.0,4.0)   (-0.05,0) (0.0,1) (0.0301,1) (0.0501,0)
Tbl.Zh.Kdp.Sld    (4.0,6.0)   (-0.05,0) (0.0,1) (0.0302,1) (0.0502,0)
Tbl.Zh.Kdp.Sld    (6.0,8.0)   (-0.05,0) (0.0,1) (0.0302,1) (0.0502,0)
Tbl.Zh.Kdp.Sld    (8.0,10.0)   (-0.05,0) (0.0,1) (0.0304,1) (0.0504,0)
Tbl.Zh.Kdp.Sld    (10.0,12.0)   (-0.05,0) (0.0,1) (0.0305,1) (0.0505,0)
Tbl.Zh.Kdp.Sld    (12.0,14.0)   (-0.05,0) (0.0,1) (0.0308,1) (0.0508,0)
Tbl.Zh.Kdp.Sld    (14.0,16.0)   (-0.05,0) (0.0,1) (0.0312,1) (0.0512,0)
Tbl.Zh.Kdp.Sld    (16.0,18.0)   (-0.05,0) (0.0,1) (0.0319,1) (0.0519,0)
Tbl.Zh.Kdp.Sld    (18.0,20.0)   (-0.05,0) (0.0,1) (0.0329,1) (0.0529,0)
Tbl.Zh.Kdp.Sld    (19.0,21.0)   (-0.05,0) (0.0,1) (0.0335,1) (0.0535,0)
Tbl.Zh.Kdp.Sld    (21.0,23.0)   (-0.05,0) (0.0,1) (0.0354,1) (0.0554,0)
Tbl.Zh.Kdp.Sld    (23.0,25.0)   (-0.05,0) (0.0,1) (0.0382,1) (0.0582,0)
Tbl.Zh.Kdp.Sld    (25.0,27.0)   (-0.05,0) (0.0,1) (0.0424,1) (0.0624,0)
Tbl.Zh.Kdp.Sld    (27.0,29.0)   (-0.05,0) (0.0,1) (0.0489,1) (0.0689,0)
Tbl.Zh.Kdp.Sld    (29.0,31.0)   (-0.05,0) (0.0,1) (0.0588,1) (0.0788,0)
Tbl.Zh.Kdp.Sld    (31.0,33.0)   (-0.05,0) (0.0,1) (0.0738,1) (0.0938,0)
Tbl.Zh.Kdp.Sld    (33.0,35.0)   (-0.05,0) (0.0,1) (0.0965,1) (0.1165,0)
Tbl.Zh.Kdp.Sld    (35.0,37.0)   (-0.05,0) (0.0,1) (0.1312,1) (0.1512,0)

Tbl.Zh.Kdp.Bgs    (-20,35)      (-0.1,1) (0,1) (0.05,1) (.1,0)
Tbl.Zh.Kdp.Trip2  (-20,35.0)    (-0.1,0) (0.0,1) (0.1,1) (0.2,0)
Tbl.Zh.Kdp.Gcl    (-20,70)       (-0.1,1) (0,1) (0.05,1) (.1,0) 

#
# Membership functions for RHOHV
#
Tbl.Zh.Rhv.CL    (-20,6)   (0.7,0) (0.98,0) (0.99,1) (1.1,1)
Tbl.Zh.Rhv.Drz   (0,20)    (0.7,0) (0.98,0) (0.99,1) (1.1,1)
Tbl.Zh.Rhv.Lr    (20,40)   (0.7,0) (0.98,0) (0.99,1) (1.1,1)
Tbl.Zh.Rhv.Mr    (30,45)   (0.7,0) (0.98,0) (0.99,1) (1.1,1)
Tbl.Zh.Rhv.Mr    (45,50)   (0.7,0) (0.97,0) (0.98,1) (1.1,1)
Tbl.Zh.Rhv.Hr    (40,45)   (0.7,0) (0.98,0) (0.99,1) (1.1,1)
Tbl.Zh.Rhv.Hr    (45,60)   (0.7,0) (0.97,0) (0.98,1) (1.1,1)

Tbl.Zh.Rhv.Ha    (45.0,47.0)   (0.8,0) (0.9187,1) (0.9687,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (47.0,49.0)   (0.8,0) (0.9163,1) (0.9662,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (49.0,51.0)   (0.8,0) (0.9137,1) (0.9637,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (51.0,53.0)   (0.8,0) (0.9113,1) (0.9612,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (53.0,55.0)   (0.8,0) (0.9087,1) (0.9587,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (55.0,57.0)   (0.8,0) (0.9062,1) (0.9562,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (57.0,59.0)   (0.8,0) (0.9037,1) (0.9537,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (59.0,61.0)   (0.8,0) (0.9012,1) (0.9512,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (61.0,63.0)   (0.8,0) (0.8987,1) (0.9487,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (63.0,65.0)   (0.8,0) (0.8962,1) (0.9462,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (65.0,67.0)   (0.8,0) (0.8937,1) (0.9437,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (67.0,69.0)   (0.8,0) (0.8912,1) (0.9412,1) (1.1,0)
Tbl.Zh.Rhv.Ha    (69.0,71.0)   (0.8,0) (0.8887,1) (0.9387,1) (1.1,0)

Tbl.Zh.Rhv.Rh     (45.0,77.0)   (0.8,0) (0.8687,1) (0.97,1) (0.98,0)

Tbl.Zh.Rhv.Gsh    (25.0,27.0)   (0.85,0) (0.8937,1) (0.9937,1) (1.0437,0)
Tbl.Zh.Rhv.Gsh    (27.0,29.0)   (0.85,0) (0.8912,1) (0.9912,1) (1.0413,0)
Tbl.Zh.Rhv.Gsh    (29.0,31.0)   (0.85,0) (0.8887,1) (0.9887,1) (1.0387,0)
Tbl.Zh.Rhv.Gsh    (31.0,33.0)   (0.85,0) (0.8862,1) (0.9862,1) (1.0362,0)
Tbl.Zh.Rhv.Gsh    (33.0,35.0)   (0.85,0) (0.8837,1) (0.9837,1) (1.0337,0)
Tbl.Zh.Rhv.Gsh    (35.0,37.0)   (0.85,0) (0.8812,1) (0.9812,1) (1.0312,0)
Tbl.Zh.Rhv.Gsh    (37.0,39.0)   (0.85,0) (0.8787,1) (0.9787,1) (1.0287,0)
Tbl.Zh.Rhv.Gsh    (39.0,41.0)   (0.85,0) (0.8762,1) (0.9762,1) (1.0262,0)
Tbl.Zh.Rhv.Gsh    (41.0,43.0)   (0.85,0) (0.8737,1) (0.9737,1) (1.0237,0)
Tbl.Zh.Rhv.Gsh    (43.0,45.0)   (0.85,0) (0.8712,1) (0.9712,1) (1.0212,0)
Tbl.Zh.Rhv.Gsh    (45.0,47.0)   (0.85,0) (0.8687,1) (0.9687,1) (1.0187,0)
Tbl.Zh.Rhv.Gsh    (47.0,49.0)   (0.85,0) (0.8662,1) (0.9662,1) (1.0162,0)
Tbl.Zh.Rhv.Gsh    (49.0,51.0)   (0.85,0) (0.8637,1) (0.9637,1) (1.0137,0)
Tbl.Zh.Rhv.Gsh    (51.0,53.0)   (0.85,0) (0.8612,1) (0.9612,1) (1.0112,0)
Tbl.Zh.Rhv.Gsh    (53.0,55.0)   (0.85,0) (0.8587,1) (0.9587,1) (1.0087,0)

Tbl.Zh.Rhv.GRR    (25.0,55.0)   (0.82,0) (0.8512,1) (0.98,1) (0.99,0)

Tbl.Zh.Rhv.Ds     (10,35)   (0.7,0) (0.97,0) (0.98,1) (1.1,1)
Tbl.Zh.Rhv.Ws     (-5,50)   (0.7,0) (0.75,1) (0.98,1) (0.99,0)
Tbl.Zh.Rhv.Ic     (-10,30)   (0.7,0) (0.97,0) (0.98,1) (1.1,1)
Tbl.Zh.Rhv.Iic    (-10,30)   (0.7,0) (0.97,0) (0.98,1) (1.1,1)

Tbl.Zh.Rhv.Sld    (-20,30)   (0.7,0) (0.97,0) (0.98,1) (1.1,1)

Tbl.Zh.Rhv.Bgs    (-20,35)   (0.7,0) (0.8,1) (0.9,1) (1.0,0)
Tbl.Zh.Rhv.Trip2  (-20,35)   (0.7,0) (0.97,0) (0.98,1) (1.1,1)
Tbl.Zh.Rhv.Gcl    (-20,70)   (.2,1) (.7,1) (.8,0)

#
# Membership functions for Temperature

Tbl.Zh.Tmp.CL     (-20,6)   (-10,0) (-1,1) (40,1)
Tbl.Zh.Tmp.Drz    (0,20)   (-1,0) (1,1) (40,1)
Tbl.Zh.Tmp.Lr     (20,40)   (-1,0) (1,1) (40,1)
Tbl.Zh.Tmp.Mr     (30,50)   (-1,0) (1,1) (40,1)
Tbl.Zh.Tmp.Hr     (40,60)   (-1,0) (1,1) (40,1)
Tbl.Zh.Tmp.Ha     (45,70)   (-100,0) (-50,1) (20,1) (30,0) #changed this!!!
Tbl.Zh.Tmp.Rh     (45,70)   (-30,0) (-25,1) (20,1) (30,0)
Tbl.Zh.Tmp.Gsh    (25,55)   (-100,0) (-50,1) (20,1) (30,0) #changed this!!
Tbl.Zh.Tmp.GRR    (25,55)   (-30,0) (-25,1) (20,1) (25,0)
Tbl.Zh.Tmp.Ds     (10,35)   (-100,1) (-50,1) (-1,1) (1,0)
Tbl.Zh.Tmp.Ws     (-5,50)   (-8,0) (-4,1) (6,1) (8,0)
Tbl.Zh.Tmp.Ic     (-10,30)   (-100,1) (-50,1) (-1,1) (1,0)
Tbl.Zh.Tmp.Iic    (-10,30)  (-100,1) (-50,1) (-1,1) (1,0)
Tbl.Zh.Tmp.Sld    (-20,30)  (-30,0) (-10,1) (-1,1) (1,0)
Tbl.Zh.Tmp.Bgs    (-20,35)   (10,0) (15,1) (40,1) (50,0)
Tbl.Zh.Tmp.Trip2  (-20,35)  (-52,0) (-50,1) (-1,1) (40,1)
Tbl.Zh.Tmp.Gcl    (-20,70)   (-25,0) (-10,1) (40,1)(50,0)  
#
# Membership functions for Std dev ZDR
#
Tbl.Zh.SDZDR.CL     (-20,6)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Drz    (0,20)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Lr     (20,40)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Mr     (30,50)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Hr     (40,60)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Ha     (45,70)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Rh     (45,70)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Gsh    (25,55)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.GRR    (25,55)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Ds     (10,35)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Ws     (-5,50)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Ic     (-10,30)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Iic    (-10,30)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Sld    (-20,30)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Bgs    (-20,35)   (0.5,0)  (0.7,1) (3,1)  (3.2,0)
Tbl.Zh.SDZDR.Trip2  (-20,35)   (0,1)  (1,1) (1.1,0)
Tbl.Zh.SDZDR.Gcl    (-20,70)   (0,0) (1,0)  (1.1,1) (100,1)
#
# Membership functions for Std dev PHI
#
Tbl.Zh.SPHI.CL     (-20,6)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Drz    (0,20)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Lr     (20,40)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Mr     (30,50)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Hr     (40,60)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Ha     (45,70)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Rh     (45,70)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Gsh    (25,55)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.GRR    (25,55)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Ds     (10,35)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Ws     (-5,50)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Ic     (-10,30)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Iic    (-10,30)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Sld    (-20,30)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Bgs    (-20,35)   (5,0)  (10,1) (35,1)  (40,0)
Tbl.Zh.SPHI.Trip2  (-20,35)   (0,1)  (10,1) (15,0)
Tbl.Zh.SPHI.Gcl    (-20,70)   (0,0) (10,0)  (15,1) (100,1)

</code></pre>
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
      <li class="mr-3">&copy; 2019 <span title="0.38440s from unicorn-64b5768cb7-nkl7g">GitHub</span>, Inc.</li>
        <li class="mr-3"><a data-ga-click="Footer, go to terms, text:terms" href="https://github.com/site/terms">Terms</a></li>
        <li class="mr-3"><a data-ga-click="Footer, go to privacy, text:privacy" href="https://github.com/site/privacy">Privacy</a></li>
        <li class="mr-3"><a href="/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li class="mr-3"><a href="https://githubstatus.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
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
        <li class="mr-3"><a href="https://github.blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
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


    
    <script crossorigin="anonymous" integrity="sha512-3wgtWW5loG8Clfq/c7EBLsxN//2dHrHnWZYEQJAm/N6xftU0RloC1R1P3VdvqAlaBbARZO962vvmj2aWdc89Mw==" type="application/javascript" src="https://github.githubassets.com/assets/frameworks-c2be165e13b944c2a95ecf55c257be15.js"></script>
    
    <script crossorigin="anonymous" async="async" integrity="sha512-HALtspRn9/yL25Aoybs/qbguZDWm8Gg7IJFWDy1vvLisNZuyKcckgfphlNyFcL24PStrr02V1LlJZkUGQDG+cQ==" type="application/javascript" src="https://github.githubassets.com/assets/github-55ff70261637e7602d9fc1169c6804f1.js"></script>
    
    
    
  <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
  <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default text-gray-dark" open>
    <summary aria-haspopup="dialog" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast">
      <button class="Box-btn-octicon m-0 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
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

  <div aria-live="polite" class="js-global-screen-reader-notice sr-only"></div>

  </body>
</html>

