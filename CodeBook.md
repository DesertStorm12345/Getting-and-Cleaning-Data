



<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>Cleaning_Getting_Data/CodeBook.md at master · AntheaTan/Cleaning_Getting_Data</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="AntheaTan/Cleaning_Getting_Data" name="twitter:title" /><meta content="Contribute to Cleaning_Getting_Data development by creating an account on GitHub." name="twitter:description" /><meta content="https://avatars2.githubusercontent.com/u/8416948?v=2&amp;s=400" name="twitter:image:src" />
<meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars2.githubusercontent.com/u/8416948?v=2&amp;s=400" property="og:image" /><meta content="AntheaTan/Cleaning_Getting_Data" property="og:title" /><meta content="https://github.com/AntheaTan/Cleaning_Getting_Data" property="og:url" /><meta content="Contribute to Cleaning_Getting_Data development by creating an account on GitHub." property="og:description" />

      <meta name="browser-stats-url" content="/_stats">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="conduit-xhr" href="https://ghconduit.com:25035">
    <link rel="xhr-socket" href="/_sockets">
    <meta name="pjax-timeout" content="1000">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>
      <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="DAD46AF2:2E0E:1168072:544BB546" name="octolytics-dimension-request_id" /><meta content="8470269" name="octolytics-actor-id" /><meta content="DesertStorm12345" name="octolytics-actor-login" /><meta content="e2c46ee02ea690afd2583bfc3ea1800770eadeaa68bf6f78d199628f94b096f1" name="octolytics-actor-hash" />
    
    <meta content="Rails, view, blob#show" name="analytics-event" />

    
    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="WXPAXlUbHfKJxWEcz9YyG/VV0mNXUnKC6cozxQgzzW8pupBTCGsN/F+a99SGBEbNMVjLI0FH59mTnmOmzkyVAg==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-fd24da028f7f2d737c9a6d97bdd8aa7a5d7ec419c4cc4e89b169d30c58bed96b.css" media="all" rel="stylesheet" type="text/css" />
    <link href="https://assets-cdn.github.com/assets/github2-e601e4dc2eec6decc441b9f7e15eec77891539a1a5e2d8af7af600d1d061a150.css" media="all" rel="stylesheet" type="text/css" />
    
    


    <meta http-equiv="x-pjax-version" content="e375408a179f2ef68cd4fb7efa2d26f7">

      
  <meta name="description" content="Contribute to Cleaning_Getting_Data development by creating an account on GitHub.">
  <meta name="go-import" content="github.com/AntheaTan/Cleaning_Getting_Data git https://github.com/AntheaTan/Cleaning_Getting_Data.git">

  <meta content="8416948" name="octolytics-dimension-user_id" /><meta content="AntheaTan" name="octolytics-dimension-user_login" /><meta content="25696042" name="octolytics-dimension-repository_id" /><meta content="AntheaTan/Cleaning_Getting_Data" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="25696042" name="octolytics-dimension-repository_network_root_id" /><meta content="AntheaTan/Cleaning_Getting_Data" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/AntheaTan/Cleaning_Getting_Data/commits/master.atom" rel="alternate" title="Recent Commits to Cleaning_Getting_Data:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production  vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      
      


      <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" ga-data-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <form accept-charset="UTF-8" action="/AntheaTan/Cleaning_Getting_Data/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/AntheaTan/Cleaning_Getting_Data/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <input type="text"
    class="js-site-search-field is-clearable"
    data-hotkey="s"
    name="q"
    placeholder="Search"
    data-global-scope-placeholder="Search GitHub"
    data-repo-scope-placeholder="Search"
    tabindex="1"
    autocapitalize="off">
  <div class="scope-badge">This repository</div>
</form>
      </div>
      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item explore">
          <a class="header-nav-link" href="/explore" data-ga-click="Header, go to explore, text:explore">Explore</a>
        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/blog" data-ga-click="Header, go to blog, text:blog">Blog</a>
          </li>
        <li class="header-nav-item">
          <a class="header-nav-link" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a>
        </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name" href="/DesertStorm12345" data-ga-click="Header, go to profile, text:username">
      <img alt="DesertStorm12345" class="avatar" data-user="8470269" height="20" src="https://avatars0.githubusercontent.com/u/8470269?v=2&amp;s=40" width="20" />
      <span class="css-truncate">
        <span class="css-truncate-target">DesertStorm12345</span>
      </span>
    </a>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link js-menu-target tooltipped tooltipped-s" href="#" aria-label="Create new..." data-ga-click="Header, create new, icon:add">
      <span class="octicon octicon-plus"></span>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      
<ul class="dropdown-menu">
  <li>
    <a href="/new"><span class="octicon octicon-repo"></span> New repository</a>
  </li>
  <li>
    <a href="/organizations/new"><span class="octicon octicon-organization"></span> New organization</a>
  </li>


    <li class="dropdown-divider"></li>
    <li class="dropdown-header">
      <span title="AntheaTan/Cleaning_Getting_Data">This repository</span>
    </li>
      <li>
        <a href="/AntheaTan/Cleaning_Getting_Data/issues/new"><span class="octicon octicon-issue-opened"></span> New issue</a>
      </li>
</ul>

    </div>
  </li>

  <li class="header-nav-item">
        <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
        <span class="mail-status all-read"></span>
        <span class="octicon octicon-inbox"></span>
</a>
  </li>

  <li class="header-nav-item">
    <a class="header-nav-link tooltipped tooltipped-s" href="/settings/profile" id="account_settings" aria-label="Settings" data-ga-click="Header, go to settings, icon:settings">
      <span class="octicon octicon-gear"></span>
    </a>
  </li>

  <li class="header-nav-item">
    <form accept-charset="UTF-8" action="/logout" class="logout-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="rIjDkZIHMT9wCtjKUTtsnEymqly0FL9IAZDd2LxXpw0IA6i7R+gBiQ+KqBN+lGktO+adlBNbA/sXjfjjQ8cIsw==" /></div>
      <button class="header-nav-link sign-out-button tooltipped tooltipped-s" aria-label="Sign out" data-ga-click="Header, sign out, icon:logout">
        <span class="octicon octicon-sign-out"></span>
      </button>
</form>  </li>

</ul>


    
  </div>
</div>

      

        


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

    <li class="subscription">
      <form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="0GQVCuLwGbQAi1ihpq++IrlGN2usLsjVJJqMxHQkX8LNuZrT3+5c8CcBSAjnHH4fORXiq6KxPU6ZxoNcWAvjwQ==" /></div>  <input id="repository_id" name="repository_id" type="hidden" value="25696042" />

    <div class="select-menu js-menu-container js-select-menu">
      <a class="social-count js-social-count" href="/AntheaTan/Cleaning_Getting_Data/watchers">
        1
      </a>
      <a href="/AntheaTan/Cleaning_Getting_Data/subscription"
        class="minibutton select-menu-button with-count js-menu-target" role="button" tabindex="0" aria-haspopup="true">
        <span class="js-select-button">
          <span class="octicon octicon-eye"></span>
          Watch
        </span>
      </a>

      <div class="select-menu-modal-holder">
        <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
          <div class="select-menu-header">
            <span class="select-menu-title">Notifications</span>
            <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
          </div> <!-- /.select-menu-header -->

          <div class="select-menu-list js-navigation-container" role="menu">

            <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                <h4>Not watching</h4>
                <span class="description">Be notified when participating or @mentioned.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Watch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                <h4>Watching</h4>
                <span class="description">Be notified of all conversations.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Unwatch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_ignore" name="do" type="radio" value="ignore" />
                <h4>Ignoring</h4>
                <span class="description">Never be notified.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-mute"></span>
                  Stop ignoring
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

          </div> <!-- /.select-menu-list -->

        </div> <!-- /.select-menu-modal -->
      </div> <!-- /.select-menu-modal-holder -->
    </div> <!-- /.select-menu -->

</form>
    </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <form accept-charset="UTF-8" action="/AntheaTan/Cleaning_Getting_Data/unstar" class="js-toggler-form starred js-unstar-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="IuBf/HcWdc0+qScA+UVQgvTshjFfx/J2pEVCglVpUMLkEy86sboj5rMlcf30o70hilktTdRyWqSpjYDTmPPHBw==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Unstar this repository" title="Unstar AntheaTan/Cleaning_Getting_Data">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/AntheaTan/Cleaning_Getting_Data/stargazers">
          0
        </a>
</form>
    <form accept-charset="UTF-8" action="/AntheaTan/Cleaning_Getting_Data/star" class="js-toggler-form unstarred js-star-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="oRTG3EHn3SR1B3NXFVkB7GnpXkhX3Km9Ic8sLpz7D7pskjFcGzy1H9SaHhZsDrUcZZt+pd8XyHnXlmpWHj0UQQ==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Star this repository" title="Star AntheaTan/Cleaning_Getting_Data">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/AntheaTan/Cleaning_Getting_Data/stargazers">
          0
        </a>
</form>  </div>

  </li>


        <li>
          <a href="/AntheaTan/Cleaning_Getting_Data/fork" class="minibutton with-count js-toggler-target fork-button tooltipped-n" title="Fork your own copy of AntheaTan/Cleaning_Getting_Data to your account" aria-label="Fork your own copy of AntheaTan/Cleaning_Getting_Data to your account" rel="nofollow" data-method="post">
            <span class="octicon octicon-repo-forked"></span>
            Fork
          </a>
          <a href="/AntheaTan/Cleaning_Getting_Data/network" class="social-count">0</a>
        </li>

</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/AntheaTan" class="url fn" itemprop="url" rel="author"><span itemprop="title">AntheaTan</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/AntheaTan/Cleaning_Getting_Data" class="js-current-repository js-repo-home-link" data-pjax-container-selector="#js-repo-pjax-container">Cleaning_Getting_Data</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
          </span>

        </h1>
      </div><!-- /.container -->
    </div><!-- /.repohead -->

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline  ">
        <div class="repository-sidebar clearfix">
            
<div class="sunken-menu vertical-right repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders" role="navigation" data-issue-count-url="/AntheaTan/Cleaning_Getting_Data/issues/counts" data-pjax-container-selector="#js-repo-pjax-container">
  <div class="sunken-menu-contents">
    <ul class="sunken-menu-group">
      <li class="tooltipped tooltipped-w" aria-label="Code">
        <a href="/AntheaTan/Cleaning_Getting_Data" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-pjax="true" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /AntheaTan/Cleaning_Getting_Data">
          <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

        <li class="tooltipped tooltipped-w" aria-label="Issues">
          <a href="/AntheaTan/Cleaning_Getting_Data/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /AntheaTan/Cleaning_Getting_Data/issues">
            <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
            <span class="js-issue-replace-counter"></span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>        </li>

      <li class="tooltipped tooltipped-w" aria-label="Pull Requests">
        <a href="/AntheaTan/Cleaning_Getting_Data/pulls" aria-label="Pull Requests" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g p" data-selected-links="repo_pulls /AntheaTan/Cleaning_Getting_Data/pulls">
            <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull Requests</span>
            <span class="js-pull-replace-counter"></span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>


        <li class="tooltipped tooltipped-w" aria-label="Wiki">
          <a href="/AntheaTan/Cleaning_Getting_Data/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item js-disable-pjax" data-hotkey="g w" data-selected-links="repo_wiki /AntheaTan/Cleaning_Getting_Data/wiki">
            <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
            <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>        </li>
    </ul>
    <div class="sunken-menu-separator"></div>
    <ul class="sunken-menu-group">

      <li class="tooltipped tooltipped-w" aria-label="Pulse">
        <a href="/AntheaTan/Cleaning_Getting_Data/pulse/weekly" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-pjax="true" data-selected-links="pulse /AntheaTan/Cleaning_Getting_Data/pulse/weekly">
          <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

      <li class="tooltipped tooltipped-w" aria-label="Graphs">
        <a href="/AntheaTan/Cleaning_Getting_Data/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-pjax="true" data-selected-links="repo_graphs repo_contributors /AntheaTan/Cleaning_Getting_Data/graphs">
          <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>
    </ul>


  </div>
</div>

              <div class="only-with-full-nav">
                
  
<div class="clone-url open"
  data-protocol-type="http"
  data-url="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="https://github.com/AntheaTan/Cleaning_Getting_Data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="https://github.com/AntheaTan/Cleaning_Getting_Data.git" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="ssh"
  data-url="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone">
  <h3><span class="text-emphasized">SSH</span> clone URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="git@github.com:AntheaTan/Cleaning_Getting_Data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="git@github.com:AntheaTan/Cleaning_Getting_Data.git" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="subversion"
  data-url="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group">
    <input type="text" class="input-mini input-monospace js-url-field"
           value="https://github.com/AntheaTan/Cleaning_Getting_Data" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-clipboard-text="https://github.com/AntheaTan/Cleaning_Getting_Data" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>


<p class="clone-options">You can clone with
      <a href="#" class="js-clone-selector" data-protocol="http">HTTPS</a>,
      <a href="#" class="js-clone-selector" data-protocol="ssh">SSH</a>,
      or <a href="#" class="js-clone-selector" data-protocol="subversion">Subversion</a>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</p>



                <a href="/AntheaTan/Cleaning_Getting_Data/archive/master.zip"
                   class="minibutton sidebar-button"
                   aria-label="Download the contents of AntheaTan/Cleaning_Getting_Data as a zip file"
                   title="Download the contents of AntheaTan/Cleaning_Getting_Data as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/AntheaTan/Cleaning_Getting_Data/blob/4566633033c030a77a549da98ec6a158219f1e99/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:c9f9693b795f37bd7f675cbd18e4f01e -->

<div class="file-navigation">
  
<div class="select-menu js-menu-container js-select-menu left">
  <span class="minibutton select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-master-branch="master"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <span class="octicon octicon-git-branch"></span>
    <i>branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div> <!-- /.select-menu-header -->

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" class="js-select-menu-tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" class="js-select-menu-tab">Tags</a>
            </li>
          </ul>
        </div><!-- /.select-menu-tabs -->
      </div><!-- /.select-menu-filters -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <div class="select-menu-item js-navigation-item selected">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/AntheaTan/Cleaning_Getting_Data/blob/master/CodeBook.md"
                 data-name="master"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="master">master</a>
            </div> <!-- /.select-menu-item -->
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

    </div> <!-- /.select-menu-modal -->
  </div> <!-- /.select-menu-modal-holder -->
</div> <!-- /.select-menu -->

  <div class="button-group right">
    <a href="/AntheaTan/Cleaning_Getting_Data/find/master"
          class="js-show-file-finder minibutton empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button class="js-zeroclipboard minibutton zeroclipboard-button"
          data-clipboard-text="CodeBook.md"
          aria-label="Copy to clipboard"
          data-copied-hint="Copied!">
      <span class="octicon octicon-clippy"></span>
    </button>
  </div>

  <div class="breadcrumb">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/AntheaTan/Cleaning_Getting_Data" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">Cleaning_Getting_Data</span></a></span></span><span class="separator"> / </span><strong class="final-path">CodeBook.md</strong>
  </div>
</div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="AntheaTan" class="avatar" data-user="8416948" height="24" src="https://avatars0.githubusercontent.com/u/8416948?v=2&amp;s=48" width="24" />
        <span class="author"><a href="/AntheaTan" rel="author">AntheaTan</a></span>
        <time datetime="2014-10-25T14:24:27Z" is="relative-time">Oct 25, 2014</time>
        <div class="commit-title">
            <a href="/AntheaTan/Cleaning_Getting_Data/commit/4566633033c030a77a549da98ec6a158219f1e99" class="message" data-pjax="true" title="Update CodeBook.md">Update CodeBook.md</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>1</strong>
           contributor
        </a>
      </p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list">
          <li class="facebox-user-list-item">
            <img alt="AntheaTan" data-user="8416948" height="24" src="https://avatars0.githubusercontent.com/u/8416948?v=2&amp;s=48" width="24" />
            <a href="/AntheaTan">AntheaTan</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file-box">
  <div class="file">
    <div class="meta clearfix">
      <div class="info file-name">
          <span>117 lines (100 sloc)</span>
          <span class="meta-divider"></span>
        <span>5.193 kb</span>
      </div>
      <div class="actions">
        <div class="button-group">
          <a href="/AntheaTan/Cleaning_Getting_Data/raw/master/CodeBook.md" class="minibutton " id="raw-url">Raw</a>
            <a href="/AntheaTan/Cleaning_Getting_Data/blame/master/CodeBook.md" class="minibutton js-update-url-with-hash">Blame</a>
          <a href="/AntheaTan/Cleaning_Getting_Data/commits/master/CodeBook.md" class="minibutton " rel="nofollow">History</a>
        </div><!-- /.button-group -->


              <a class="octicon-button tooltipped tooltipped-n js-update-url-with-hash"
                 aria-label="Clicking this button will fork this project so you can edit the file"
                 href="/AntheaTan/Cleaning_Getting_Data/edit/master/CodeBook.md"
                 data-method="post" rel="nofollow"><span class="octicon octicon-pencil"></span></a>

            <a class="octicon-button danger tooltipped tooltipped-s"
               href="/AntheaTan/Cleaning_Getting_Data/delete/master/CodeBook.md"
               aria-label="Fork this project and delete file"
               data-method="post" data-test-id="delete-blob-file" rel="nofollow">
          <span class="octicon octicon-trashcan"></span>
        </a>
      </div><!-- /.actions -->
    </div>
      <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a name="user-content-codebook" class="anchor" href="#codebook" aria-hidden="true"><span class="octicon octicon-link"></span></a>CodeBook</h1>

<p>This code book describes the variables, the data and any transformations or work that you performed to clean up the data.</p>

<h2>
<a name="user-content-the-data-source" class="anchor" href="#the-data-source" aria-hidden="true"><span class="octicon octicon-link"></span></a>The data source</h2>

<ul class="task-list">
<li>Original data: <a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a>
</li>
<li>Original description of the dataset: <a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones</a>
</li>
</ul>

<h2>
<a name="user-content-data-set-information" class="anchor" href="#data-set-information" aria-hidden="true"><span class="octicon octicon-link"></span></a>Data Set Information</h2>

<p>The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. </p>

<p>The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. </p>

<h2>
<a name="user-content-the-data" class="anchor" href="#the-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>The data</h2>

<p>The dataset includes the following files:</p>

<ul class="task-list">
<li>'README.txt'</li>
<li>'features_info.txt': Shows information about the variables used on the feature vector.</li>
<li>'features.txt': List of all features.</li>
<li>'activity_labels.txt': Links the class labels with their activity name.</li>
<li>'train/X_train.txt': Training set.</li>
<li>'train/y_train.txt': Training labels.</li>
<li>'test/X_test.txt': Test set.</li>
<li>'test/y_test.txt': Test labels.</li>
</ul>

<p>The following files are available for the train and test data. Their descriptions are equivalent.</p>

<ul class="task-list">
<li>'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.</li>
<li>'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.</li>
<li>'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.</li>
<li>'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.</li>
</ul>

<h2>
<a name="user-content-transformation-details" class="anchor" href="#transformation-details" aria-hidden="true"><span class="octicon octicon-link"></span></a>Transformation details</h2>

<p>There are 5 parts:</p>

<ul class="task-list">
<li>1) Merges the training and the test sets to create one data set.</li>
<li>2) Extracts only the measurements on the mean and standard deviation for each measurement.</li>
<li>3) Uses descriptive activity names to name the activities in the data set</li>
<li>4) Appropriately labels the data set with descriptive activity names.</li>
<li>5) Creates a second, independent tidy data set with the average of each variable for each activity and each subject.</li>
</ul>

<h2>
<a name="user-content-variables" class="anchor" href="#variables" aria-hidden="true"><span class="octicon octicon-link"></span></a>Variables</h2>

<ul class="task-list">
<li>subject: 1 to 30 each representing a participant in the study</li>
<li>activityid: activity id that the subject was doing at the time of the measurement</li>
<li>activity: description of activity</li>
<li>time.BodyAcc.mean.X</li>
<li>time.BodyAcc.mean.Y</li>
<li>time.BodyAcc.mean.Z</li>
<li>time.BodyAcc.std.X</li>
<li>time.BodyAcc.std.Y</li>
<li>time.BodyAcc.std.Z</li>
<li>time.GravityAcc.mean.X</li>
<li>time.GravityAcc.mean.Y</li>
<li>time.GravityAcc.mean.Z</li>
<li>time.GravityAcc.std.X</li>
<li>time.GravityAcc.std.Y</li>
<li>time.GravityAcc.std.Z</li>
<li>time.BodyAccJerk.mean.X</li>
<li>time.BodyAccJerk.mean.Y</li>
<li>time.BodyAccJerk.mean.Z</li>
<li>time.BodyAccJerk.std.X</li>
<li>time.BodyAccJerk.std.Y</li>
<li>time.BodyAccJerk.std.Z</li>
<li>time.BodyGyro.mean.X</li>
<li>time.BodyGyro.mean.Y</li>
<li>time.BodyGyro.mean.Z</li>
<li>time.BodyGyro.std.X</li>
<li>time.BodyGyro.std.Y</li>
<li>time.BodyGyrov.std.Z</li>
<li>time.BodyGyroJerk.mean.X</li>
<li>time.BodyGyroJerk.mean.Y</li>
<li>time.BodyGyroJerk.mean.Z</li>
<li>time.BodyGyroJerk.std.X</li>
<li>time.BodyGyroJerk.std.Y</li>
<li>time.BodyGyroJerk.std.Z</li>
<li>time.BodyAccMag.mean</li>
<li>time.BodyAccMag.std</li>
<li>time.GravityAccMag.mean</li>
<li>time.GravityAccMag.std</li>
<li>time.BodyAccJerkMag.mean</li>
<li>time.BodyAccJerkMag.std</li>
<li>time.BodyGyroMag.mean</li>
<li>time.BodyGyroMag.std</li>
<li>time.BodyGyroJerkMag.mean</li>
<li>time.BodyGyroJerkMag.std</li>
<li>FFT.BodyAcc.mean.X</li>
<li>FFT.BodyAcc.mean.Y</li>
<li>FFT.BodyAcc.mean.Z</li>
<li>FFT.BodyAcc.std.X</li>
<li>FFT.BodyAcc.std.Y</li>
<li>FFT.BodyAcc.std.Z</li>
<li>FFT.BodyAccJerk.mean.X</li>
<li>FFT.BodyAccJerk.mean.Y</li>
<li>FFT.BodyAccJerk.mean.Z</li>
<li>FFT.BodyAccJerk.std.X</li>
<li>FFT.BodyAccJerk.std.Y</li>
<li>FFT.BodyAccJerk.std.Z</li>
<li>FFT.BodyGyro.mean.X</li>
<li>FFT.BodyGyro.mean.Y</li>
<li>FFT.BodyGyro.mean.Z</li>
<li>FFT.BodyGyro.std.X</li>
<li>FFT.BodyGyro.std.Y</li>
<li>FFT.BodyGyro.std.Z</li>
<li>FFT.BodyAccMag.mean</li>
<li>FFT.BodyAccMag.std</li>
<li>FFT.BodyBodyAccJerkMag.mean</li>
<li>FFT.BodyBodyAccJerkMag.std</li>
<li>FFT.BodyBodyGyroMag.mean</li>
<li>FFT.BodyBodyGyroMag.std</li>
<li>FFT.BodyBodyGyroJerkMag.mean</li>
<li>FFT.BodyBodyGyroJerkMag.std</li>
</ul>
</article>
  </div>

  </div>
</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <form accept-charset="UTF-8" class="js-jump-to-line-form">
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" autofocus>
    <button type="submit" class="button">Go</button>
  </form>
</div>

        </div>

      </div><!-- /.repo-container -->
      <div class="modal-backdrop"></div>
    </div><!-- /.container -->
  </div><!-- /.site -->


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
      <li><a href="https://status.github.com/">Status</a></li>
      <li><a href="https://developer.github.com">API</a></li>
      <li><a href="http://training.github.com">Training</a></li>
      <li><a href="http://shop.github.com">Shop</a></li>
      <li><a href="/blog">Blog</a></li>
      <li><a href="/about">About</a></li>

    </ul>

    <a href="/" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
    </a>

    <ul class="site-footer-links">
      <li>&copy; 2014 <span title="0.04036s from github-fe127-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="/site/terms">Terms</a></li>
        <li><a href="/site/privacy">Privacy</a></li>
        <li><a href="/security">Security</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
  </div><!-- /.site-footer -->
</div><!-- /.container -->


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents js-suggester-field" placeholder=""></textarea>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped tooltipped-w" aria-label="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped tooltipped-w"
      aria-label="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-x flash-close js-ajax-error-dismiss" aria-label="Dismiss error"></a>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-dabc650f8a51dffd1d4376a3522cbda5536e4807e01d2a86ff7e60d8d6ee3029.js" type="text/javascript"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-d01013daa80c5a341ba3ddb684f2f26679eb369d67459151d5175a634a9e98a5.js" type="text/javascript"></script>
      
      
  </body>
</html>

