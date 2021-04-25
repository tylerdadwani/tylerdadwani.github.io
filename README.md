# tylerdadwani.github.io
```html

<!DOCTYPE html>
<html>
  <head>
<script>window.NREUM||(NREUM={});NREUM.info={"beacon":"bam-cell.nr-data.net","errorBeacon":"bam-cell.nr-data.net","licenseKey":"199e8a4832","applicationID":"2972453","transactionName":"c11cQBFeWw5TSh9TXlFcXFEPQhgSRFFGUUJVbUFcDEY=","queueTime":0,"applicationTime":106,"agent":""}</script>
<script>(window.NREUM||(NREUM={})).loader_config={licenseKey:"199e8a4832",applicationID:"2972453"};window.NREUM||(NREUM={}),__nr_require=function(e,t,n){function r(n){if(!t[n]){var i=t[n]={exports:{}};e[n][0].call(i.exports,function(t){var i=e[n][1][t];return r(i||t)},i,i.exports)}return t[n].exports}if("function"==typeof __nr_require)return __nr_require;for(var i=0;i<n.length;i++)r(n[i]);return r}({1:[function(e,t,n){function r(){}function i(e,t,n){return function(){return o(e,[u.now()].concat(c(arguments)),t?null:this,n),t?void 0:this}}var o=e("handle"),a=e(7),c=e(8),f=e("ee").get("tracer"),u=e("loader"),s=NREUM;"undefined"==typeof window.newrelic&&(newrelic=s);var d=["setPageViewName","setCustomAttribute","setErrorHandler","finished","addToTrace","inlineHit","addRelease"],p="api-",l=p+"ixn-";a(d,function(e,t){s[t]=i(p+t,!0,"api")}),s.addPageAction=i(p+"addPageAction",!0),s.setCurrentRouteName=i(p+"routeName",!0),t.exports=newrelic,s.interaction=function(){return(new r).get()};var m=r.prototype={createTracer:function(e,t){var n={},r=this,i="function"==typeof t;return o(l+"tracer",[u.now(),e,n],r),function(){if(f.emit((i?"":"no-")+"fn-start",[u.now(),r,i],n),i)try{return t.apply(this,arguments)}catch(e){throw f.emit("fn-err",[arguments,this,e],n),e}finally{f.emit("fn-end",[u.now()],n)}}}};a("actionText,setName,setAttribute,save,ignore,onEnd,getContext,end,get".split(","),function(e,t){m[t]=i(l+t)}),newrelic.noticeError=function(e,t){"string"==typeof e&&(e=new Error(e)),o("err",[e,u.now(),!1,t])}},{}],2:[function(e,t,n){function r(){return c.exists&&performance.now?Math.round(performance.now()):(o=Math.max((new Date).getTime(),o))-a}function i(){return o}var o=(new Date).getTime(),a=o,c=e(9);t.exports=r,t.exports.offset=a,t.exports.getLastTimestamp=i},{}],3:[function(e,t,n){function r(e){return!(!e||!e.protocol||"file:"===e.protocol)}t.exports=r},{}],4:[function(e,t,n){function r(e,t){var n=e.getEntries();n.forEach(function(e){"first-paint"===e.name?d("timing",["fp",Math.floor(e.startTime)]):"first-contentful-paint"===e.name&&d("timing",["fcp",Math.floor(e.startTime)])})}function i(e,t){var n=e.getEntries();n.length>0&&d("lcp",[n[n.length-1]])}function o(e){e.getEntries().forEach(function(e){e.hadRecentInput||d("cls",[e])})}function a(e){if(e instanceof m&&!g){var t=Math.round(e.timeStamp),n={type:e.type};t<=p.now()?n.fid=p.now()-t:t>p.offset&&t<=Date.now()?(t-=p.offset,n.fid=p.now()-t):t=p.now(),g=!0,d("timing",["fi",t,n])}}function c(e){d("pageHide",[p.now(),e])}if(!("init"in NREUM&&"page_view_timing"in NREUM.init&&"enabled"in NREUM.init.page_view_timing&&NREUM.init.page_view_timing.enabled===!1)){var f,u,s,d=e("handle"),p=e("loader"),l=e(6),m=NREUM.o.EV;if("PerformanceObserver"in window&&"function"==typeof window.PerformanceObserver){f=new PerformanceObserver(r);try{f.observe({entryTypes:["paint"]})}catch(v){}u=new PerformanceObserver(i);try{u.observe({entryTypes:["largest-contentful-paint"]})}catch(v){}s=new PerformanceObserver(o);try{s.observe({type:"layout-shift",buffered:!0})}catch(v){}}if("addEventListener"in document){var g=!1,w=["click","keydown","mousedown","pointerdown","touchstart"];w.forEach(function(e){document.addEventListener(e,a,!1)})}l(c)}},{}],5:[function(e,t,n){function r(e,t){if(!i)return!1;if(e!==i)return!1;if(!t)return!0;if(!o)return!1;for(var n=o.split("."),r=t.split("."),a=0;a<r.length;a++)if(r[a]!==n[a])return!1;return!0}var i=null,o=null,a=/Version\/(\S+)\s+Safari/;if(navigator.userAgent){var c=navigator.userAgent,f=c.match(a);f&&c.indexOf("Chrome")===-1&&c.indexOf("Chromium")===-1&&(i="Safari",o=f[1])}t.exports={agent:i,version:o,match:r}},{}],6:[function(e,t,n){function r(e){function t(){e(a&&document[a]?document[a]:document[i]?"hidden":"visible")}"addEventListener"in document&&o&&document.addEventListener(o,t,!1)}t.exports=r;var i,o,a;"undefined"!=typeof document.hidden?(i="hidden",o="visibilitychange",a="visibilityState"):"undefined"!=typeof document.msHidden?(i="msHidden",o="msvisibilitychange"):"undefined"!=typeof document.webkitHidden&&(i="webkitHidden",o="webkitvisibilitychange",a="webkitVisibilityState")},{}],7:[function(e,t,n){function r(e,t){var n=[],r="",o=0;for(r in e)i.call(e,r)&&(n[o]=t(r,e[r]),o+=1);return n}var i=Object.prototype.hasOwnProperty;t.exports=r},{}],8:[function(e,t,n){function r(e,t,n){t||(t=0),"undefined"==typeof n&&(n=e?e.length:0);for(var r=-1,i=n-t||0,o=Array(i<0?0:i);++r<i;)o[r]=e[t+r];return o}t.exports=r},{}],9:[function(e,t,n){t.exports={exists:"undefined"!=typeof window.performance&&window.performance.timing&&"undefined"!=typeof window.performance.timing.navigationStart}},{}],ee:[function(e,t,n){function r(){}function i(e){function t(e){return e&&e instanceof r?e:e?u(e,f,a):a()}function n(n,r,i,o,a){if(a!==!1&&(a=!0),!l.aborted||o){e&&a&&e(n,r,i);for(var c=t(i),f=v(n),u=f.length,s=0;s<u;s++)f[s].apply(c,r);var p=d[h[n]];return p&&p.push([b,n,r,c]),c}}function o(e,t){y[e]=v(e).concat(t)}function m(e,t){var n=y[e];if(n)for(var r=0;r<n.length;r++)n[r]===t&&n.splice(r,1)}function v(e){return y[e]||[]}function g(e){return p[e]=p[e]||i(n)}function w(e,t){s(e,function(e,n){t=t||"feature",h[n]=t,t in d||(d[t]=[])})}var y={},h={},b={on:o,addEventListener:o,removeEventListener:m,emit:n,get:g,listeners:v,context:t,buffer:w,abort:c,aborted:!1};return b}function o(e){return u(e,f,a)}function a(){return new r}function c(){(d.api||d.feature)&&(l.aborted=!0,d=l.backlog={})}var f="nr@context",u=e("gos"),s=e(7),d={},p={},l=t.exports=i();t.exports.getOrSetContext=o,l.backlog=d},{}],gos:[function(e,t,n){function r(e,t,n){if(i.call(e,t))return e[t];var r=n();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(e,t,{value:r,writable:!0,enumerable:!1}),r}catch(o){}return e[t]=r,r}var i=Object.prototype.hasOwnProperty;t.exports=r},{}],handle:[function(e,t,n){function r(e,t,n,r){i.buffer([e],r),i.emit(e,t,n)}var i=e("ee").get("handle");t.exports=r,r.ee=i},{}],id:[function(e,t,n){function r(e){var t=typeof e;return!e||"object"!==t&&"function"!==t?-1:e===window?0:a(e,o,function(){return i++})}var i=1,o="nr@id",a=e("gos");t.exports=r},{}],loader:[function(e,t,n){function r(){if(!E++){var e=x.info=NREUM.info,t=l.getElementsByTagName("script")[0];if(setTimeout(u.abort,3e4),!(e&&e.licenseKey&&e.applicationID&&t))return u.abort();f(h,function(t,n){e[t]||(e[t]=n)});var n=a();c("mark",["onload",n+x.offset],null,"api"),c("timing",["load",n]);var r=l.createElement("script");r.src="https://"+e.agent,t.parentNode.insertBefore(r,t)}}function i(){"complete"===l.readyState&&o()}function o(){c("mark",["domContent",a()+x.offset],null,"api")}var a=e(2),c=e("handle"),f=e(7),u=e("ee"),s=e(5),d=e(3),p=window,l=p.document,m="addEventListener",v="attachEvent",g=p.XMLHttpRequest,w=g&&g.prototype;if(d(p.location)){NREUM.o={ST:setTimeout,SI:p.setImmediate,CT:clearTimeout,XHR:g,REQ:p.Request,EV:p.Event,PR:p.Promise,MO:p.MutationObserver};var y=""+location,h={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net",agent:"js-agent.newrelic.com/nr-1208.min.js"},b=g&&w&&w[m]&&!/CriOS/.test(navigator.userAgent),x=t.exports={offset:a.getLastTimestamp(),now:a,origin:y,features:{},xhrWrappable:b,userAgent:s};e(1),e(4),l[m]?(l[m]("DOMContentLoaded",o,!1),p[m]("load",r,!1)):(l[v]("onreadystatechange",i),p[v]("onload",r)),c("mark",["firstbyte",a.getLastTimestamp()],null,"api");var E=0}},{}],"wrap-function":[function(e,t,n){function r(e,t){function n(t,n,r,f,u){function nrWrapper(){var o,a,s,p;try{a=this,o=d(arguments),s="function"==typeof r?r(o,a):r||{}}catch(l){i([l,"",[o,a,f],s],e)}c(n+"start",[o,a,f],s,u);try{return p=t.apply(a,o)}catch(m){throw c(n+"err",[o,a,m],s,u),m}finally{c(n+"end",[o,a,p],s,u)}}return a(t)?t:(n||(n=""),nrWrapper[p]=t,o(t,nrWrapper,e),nrWrapper)}function r(e,t,r,i,o){r||(r="");var c,f,u,s="-"===r.charAt(0);for(u=0;u<t.length;u++)f=t[u],c=e[f],a(c)||(e[f]=n(c,s?f+r:r,i,f,o))}function c(n,r,o,a){if(!m||t){var c=m;m=!0;try{e.emit(n,r,o,t,a)}catch(f){i([f,n,r,o],e)}m=c}}return e||(e=s),n.inPlace=r,n.flag=p,n}function i(e,t){t||(t=s);try{t.emit("internal-error",e)}catch(n){}}function o(e,t,n){if(Object.defineProperty&&Object.keys)try{var r=Object.keys(e);return r.forEach(function(n){Object.defineProperty(t,n,{get:function(){return e[n]},set:function(t){return e[n]=t,t}})}),t}catch(o){i([o],n)}for(var a in e)l.call(e,a)&&(t[a]=e[a]);return t}function a(e){return!(e&&e instanceof Function&&e.apply&&!e[p])}function c(e,t){var n=t(e);return n[p]=e,o(e,n,s),n}function f(e,t,n){var r=e[t];e[t]=c(r,n)}function u(){for(var e=arguments.length,t=new Array(e),n=0;n<e;++n)t[n]=arguments[n];return t}var s=e("ee"),d=e(8),p="nr@original",l=Object.prototype.hasOwnProperty,m=!1;t.exports=r,t.exports.wrapFunction=c,t.exports.wrapInPlace=f,t.exports.argsToArray=u},{}]},{},["loader"]);</script>

    <script src="//assets.adobedtm.com/d0cc0600946eb3957f703b9fe43c3590597a8c2c/satelliteLib-c70de708e9cd05573175cb144bac6233555f70e5.js"></script>

  <link href='//fonts.googleapis.com/css?family=Source+Sans+Pro' rel='stylesheet' type='text/css'>
  <link href='//fonts.googleapis.com/css?family=Raleway' rel='stylesheet' type='text/css'>

  <meta content="width=device-width, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no" name="viewport" />
    <title>home Automation - ThingSpeak IoT</title>  
    <meta name="description" content="home Automation on ThingSpeak. ThingSpeak is the open IoT platform with MATLAB analytics.">
  <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
  <link rel="icon" type="image/png" href="/favicon-32x32.png" sizes="32x32">
  <link rel="icon" type="image/png" href="/favicon-16x16.png" sizes="16x16">
  <link rel="manifest" href="/manifest.json">
  <link rel="mask-icon" href="/safari-pinned-tab.svg" color="#5bbad5">
  <meta name="theme-color" content="#ffffff">

  <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.1.1/css/bootstrap.min.css" />
  <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" media="screen" />
  <link rel="stylesheet" media="screen" href="/assets/application-f0c9f8e380f9ba58f9671da71ab11e6e36e0c2c4392ce20c5752c3ffb9187faa.css" data-turbolinks-track="reload" />

  <script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
  <script type="text/javascript" src="//netdna.bootstrapcdn.com/bootstrap/3.2.0/js/bootstrap.min.js"></script>
  <script type="text/javascript" src="//cdnjs.cloudflare.com/ajax/libs/jquery.tablesorter/2.25.3/js/jquery.tablesorter.combined.min.js"></script>
  <script src="/assets/application-e457bbf6a86124b0fc75d277cda64b0e85d6f59c4aaf9e70cadc9a9509387d59.js" data-turbolinks-track="reload"></script>
  <meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="Yk5O8KMynL9Ad+MZAk4NvE3hJxVRAajv6KhgTnW+gmhtjncrjiDg9COMXiTA3wDqXB+tg8xh8oHG/SdPqHmT/A==" />

  
</head>

  
  <body>

    <div id="wrap">
      <div class="navbar navbar-default navbar-fixed-top" role="navigation">
<div class="container">
  <div class="navbar-header">
    <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
      <span class="sr-only">Toggle navigation</span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
    </button>
    <a href="/">
      <img style="padding: 0 8px; margin-top: 7px;" id="nav-thingspeak-logo" data-turbolinks="false" src="/assets/thingspeak_logo_white-ef4990033a96773df16f2a98e7d72e06f1f497d026145ebbcce1aa9d974e9015.png" width="200" height="35" />
</a>  </div>
  <div class="navbar-collapse collapse" data-turbolinks="false">
    <ul class="nav navbar-nav navbar-right visible-xs visible-sm visible-md">
        <li class="dropdown">
    <a href="#" title="Sanju" role="button" aria-haspopup="true" aria-expanded="false" class="dropdown-toggle" data-toggle="dropdown" id="nav-account">
      <div class="sign-in-display">
        <img class="user-image" onerror="this.src=&#39;/assets/ico-header-account-active-a8b7d1aca3b339fa3ab2e532f542108ebc26f8e6c0cfd66e1b550bc088a6ad98.svg&#39;;" src="https://www.mathworks.com/matlabcentral/profiles/22321759_1619356431865_DEF.jpg" width="25" height="25" />
      </div>
      <div class="sign-in-display sign-in-name">
        <span>Sanju<b class="caret"></b></span>
      </div>
    </a>
    <ul class="dropdown-menu" aria-labelledby="nav-account">
      <li><a id="nav-my-account" data-turbolinks="false" href="/account">My Account</a></li>
      <li><a id="nav-edit-account" data-turbolinks="false" href="/account/profile">My Profile</a></li>
      <li><a id="nav-sign-out" data-turbolinks="false" onclick="setSIDCookie()" href="/logout">Sign Out</a></li>
    </ul>
  </li>

    </ul>
    <ul class="nav navbar-nav">
        <li class="active dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" id="nav-channels-after">Channels <b class="caret"></b></a>
          <ul class="dropdown-menu">
            <li><a id="nav-my-channels" href="/channels">My Channels</a></li>
            <li><a id="nav-watched-channels" href="/channels/watched">Watched Channels</a></li>
            <li><a id="nav-public-channels" href="/channels/public">Public Channels</a></li>
          </ul>
        </li>

        <li class="dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" id="nav-apps-after">Apps <b class="caret"></b></a>
          <ul class="dropdown-menu">
            <li><a id="nav-apps-all" href="/apps">All Apps</a></li>
              <li><a id="nav-matlab-analysis-app" href="/apps/matlab_analyses">MATLAB Analysis</a></li>
              <li><a id="nav-matlab-visualizations-app" href="/apps/matlab_visualizations">MATLAB Visualizations</a></li>
            <li><a id="nav-plugins-app" href="/apps/plugins">Plugins</a></li>
            <li><a id="nav-thingtweet-app" href="/apps/thingtweets">ThingTweet</a></li>
            <li><a id="nav-timecontrols-app" href="/apps/timecontrols">TimeControl</a></li>
            <li><a id="nav-react-app" href="/apps/reacts">React</a></li>
            <li><a id="nav-talkback-app" href="/apps/talkbacks">TalkBack</a></li>
            <li><a id="nav-thinghttp-app" href="/apps/thinghttp">ThingHTTP</a></li>
          </ul>
        </li>

      <li class="dropdown">
        <a href="#" class="dropdown-toggle" data-toggle="dropdown" id="nav-support">Support<b class="caret"></b></a>
        <ul class="dropdown-menu">
          <li><a href="https://www.mathworks.com/help/thingspeak/" target="_blank" id="nav-support-doc">Documentation</a></li>
          <li><a href="https://www.mathworks.com/help/thingspeak/getting-started-with-thingspeak.html" target="_blank" id="nav-support-tutorials">Tutorials</a></li>
          <li><a href="https://www.mathworks.com/help/thingspeak/examples.html" target="_blank" id="nav-support-examples">Examples</a></li>
          <li><a href="https://www.mathworks.com/matlabcentral/topics/thingspeak.html" target="_blank" id="nav-support-forum">Community Support</a></li>
        </ul>
      </li>


    </ul>
    <div id="right-nav">
      <ul class="nav navbar-nav">
        <span class="nav navbar-nav hidden-sm">        
          <li class="dropdown"><a id="commercial-learn-more-nav" href="/pages/commercial_learn_more">Commercial Use</a></li>
        </span>
        <li class="dropdown"><a id="nav-sign-in" href="/prices">How to Buy</a></li>
      </ul>
      <ul class="nav navbar-nav hidden-xs hidden-sm hidden-md">
          <li class="dropdown">
    <a href="#" title="Sanju" role="button" aria-haspopup="true" aria-expanded="false" class="dropdown-toggle" data-toggle="dropdown" id="nav-account">
      <div class="sign-in-display">
        <img class="user-image" onerror="this.src=&#39;/assets/ico-header-account-active-a8b7d1aca3b339fa3ab2e532f542108ebc26f8e6c0cfd66e1b550bc088a6ad98.svg&#39;;" src="https://www.mathworks.com/matlabcentral/profiles/22321759_1619356431865_DEF.jpg" width="25" height="25" />
      </div>
      <div class="sign-in-display sign-in-name">
        <span>Sanju<b class="caret"></b></span>
      </div>
    </a>
    <ul class="dropdown-menu" aria-labelledby="nav-account">
      <li><a id="nav-my-account" data-turbolinks="false" href="/account">My Account</a></li>
      <li><a id="nav-edit-account" data-turbolinks="false" href="/account/profile">My Profile</a></li>
      <li><a id="nav-sign-out" data-turbolinks="false" onclick="setSIDCookie()" href="/logout">Sign Out</a></li>
    </ul>
  </li>

      </ul>
    </div>
  </div><!--/.nav-collapse -->
</div>
</div>

      <div class="container">
        

        <div class="row">
  <div id="invalid_widget_parameter" class="alert alert-danger alert-dismissable" style="display:none; clear:both">
	<a id="invalid_widget_parameter_close" href="#" class="close" aria-label="close"><i class="fa fa-close" aria-hidden="true"></i></a>
	<a href='https://www.mathworks.com/help/thingspeak/channel_display_widgets.html' target="_blank" data-turbolinks="false" id="widget_param_doc" class="exhaustion_alert"> Widget Documentation</a>
	<span id="widget-config-err-msg">
	</span>
</div>

<div id="invalid_widget_type" class="alert alert-danger alert-dismissable" style="display:none; clear:both">
	<a id="invalid_widget_type_close" href="#" class="close" aria-label="close"><i class="fa fa-close" aria-hidden="true"></i></a>
	<span>
		You have selected an invalid widget to be created. Please select a valid widget to be created.
	</span>
</div>
      <div id="exhaustion_div">
 <div class="alert alert-danger alert-dismissable expiration_reminder" style="display:none; clear:both">
  <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
  <span>
    License <strong><span name="license_id_val_expire" id="license_id_val_expire"></span></strong>
   will expire at the end of 
  <strong><span name="expiration_date" id="expiration_date"></span></strong>.
  </span>
  <span>
    <a data-turbolinks="false" id="call_of_action_to_expire" class="exhaustion_alert"> Buy a new license
  </a>
  </span>
</div>

<div class="alert alert-danger alert-dismissable exhaustion_reminder" style="display:none; clear:both">
  <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
  <span>
  Based on your current daily usage rate,
    you
  will run out of messages on:  
  <strong><span name="exp_expiration_date" id="exp_expiration_date"></span></strong>.
  </span>
  <span>
    <a data-turbolinks="false" id="call_of_action_exhaust" class="exhaustion_alert"> Buy a new license
  </a>
  </span>
</div>

 <div class="alert alert-danger alert-dismissable shutoff_expiration_alert" style="display:none; clear:both">
  <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
    <span>
    Your term  has expired at the end of <strong><span name="shut_off_date_exp" id="shut_off_date_exp"></span></strong>.
    </span>
    <span>
    <a data-turbolinks="false" id="call_of_action_expire" class="exhaustion_alert"> Buy a new license</a>
    </span>
</div>

<div class="alert alert-danger alert-dismissable shutoff_alert" style="display:none; clear:both">
  <a href="#" class="close" data-dismiss="alert" aria-label="close">×</a>
    <span>
    You have run out of messages as of: <strong><span name="shut_off_date" id="shut_off_date"></span></strong>.
    </span>
    <span>
    <a data-turbolinks="false" id="call_of_action_shutoff" class="exhaustion_alert" > Buy a new license</a>
    </span>
</div>

</div>



    <!-- Show Channel meta data only when a channel is public or is the user's private channel, g1368777, the parentheses are redundant, since && precedes ||, but they don't hurt-->
    <!-- myChannel? is a  helper method -->
    <h1 class="margin-left" id="channel-name-header">home Automation</h1>
    <div class="row col-xs-12 col-sm-12" style="margin-bottom: 25px;">
      <div class="col-xs-6 col-sm-4">
  <ul class="no_bullets" id="table-channel-metadata">
    <li>Channel ID: <b id="channel-metadata-id">1370705</b></li>
    <li>Author: <a target="_blank" href="/users/mwa0000022321759">mwa0000022321759</a></li>
    <li id="channel-metadata-access">Access: Public</li>
  </ul>
</div>
<div class="col-xs-6 col-sm-4" style="border-left: 1px solid #ccc;">
  
</div>
    </div>

      <div class="row">
        <ul class="nav nav-tabs" style="margin: 25px;" data-turbolinks="false">
          <li role="presentation" class=active>
            <a id="channel_link_private_view" href="/channels/1370705/private_show">Private View</a>
          </li>
          <li role="presentation">
            <a id="channel_link_public_view" href="/channels/1370705">Public View</a>
          </li>
          <li role="presentation">
            <a id="channel_link_settings" href="/channels/1370705/edit">Channel Settings</a>
          </li>
          <li role="presentation">
            <a id="channel_link_sharing" href="/channels/1370705/sharing">Sharing</a>
          </li>
          <li role="presentation">
            <a id="channel_link_api_keys" href="/channels/1370705/api_keys">API Keys</a>
          </li>
          <li role="presentation">
            <a id="channel_link_import" href="/channels/1370705/import_export">Data Import / Export</a>
          </li>
        </ul>
      </div>

  <div class="col-xs-12 col-sm-12">
    <div class="row">
  <div class="col-xs-12 col-sm-6">
        <div id="add_visualization_modal" class="modal">
  <div class="modal-dialog window-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title">Click on a visualization to add it to the Channel</h4>
      </div>
      <div class="modal-body window-body">
        <div id="add_visualization_modal_content_body">
          <!-- empty widget list banner, hidden by default -->
          <h3 id="add_visualization_empty_text" class="text_center" hidden="hidden">No visualizations are available to display.</h3>
        </div>
      </div>
      <div class="modal-footer window-footer">
        <button type="button" id="add_visualization_save" data-dismiss="modal" class="btn btn-primary">Save</button>
        <button type="button" id="add_visualization_cancel" data-dismiss="modal" class="btn btn-default">Cancel</button>
      </div>
    </div>
  </div>
</div>

        <link rel="stylesheet" media="screen" href="/assets/widget-1057f0bbd162015136004c3afc35308fef75815b238ff469e1b3705ebd83f4e8.css" />
<script src="/assets/widget-325d0bf7906d9f455624f0a03a9a1e0f600d5f41aa1f573eae24505f7a66ebe6.js" data-turbolinks-track="reload"></script>
<script src="/assets/htmlUtils-e0123513218182b592fad424cd73a0fbdb891a8a4835d1cbe84f9000fa127370.js" data-turbolinks-track="reload"></script>

<div id="add_widget_modal" class="modal">
  <div class="modal-dialog window-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title">Click on a widget to add it to the Channel</h4>
      </div>
      <div class="modal-body window-body">
        <div id="add_widget_modal_content_body">
          <h3 id="add_widget_empty_text" class="text_center" hidden="hidden">No widgets are available to display.</h3>
          <!-- populate widget preview
               widget_list is an array of hashes
               [ { content_type, content_id, title, image_name } ] -->
            <div id="window_preview_template" class="window-preview-container" title="Gauge" style="background-image: url(/assets/add_widget_gauge-d71b80e4774de3c6071e0434a998561a82f5e161d96db8d432cd0293816f0b3b.svg)" content-type="widget" content-id="">
  <div class="window-header">
    <div class="window-title">Gauge</div>
        <div id="widget-metadata-id" style="display: none;">0</div>
  </div>
</div>

            <div id="window_preview_template" class="window-preview-container" title="Numeric Display" style="background-image: url(/assets/add_numeric_display-d5b1a6e43d55d3c3ae7834c77a6f745ef2b05a98d893113201302b156e72f29f.svg)" content-type="widget" content-id="">
  <div class="window-header">
    <div class="window-title">Numeric Display</div>
        <div id="widget-metadata-id" style="display: none;">1</div>
  </div>
</div>

            <div id="window_preview_template" class="window-preview-container" title="Lamp Indicator" style="background-image: url(/assets/lamp-e06df52dcbe969787a34d96fffbad569b7508a349f30e174036fc4d56b86ce20.svg)" content-type="widget" content-id="">
  <div class="window-header">
    <div class="window-title">Lamp Indicator</div>
        <div id="widget-metadata-id" style="display: none;">2</div>
  </div>
</div>

        </div>
      </div>
      <div class="modal-footer window-footer">
        <button type="button" id="add_widget_next" data-dismiss="modal" data-toggle="modal" data-target="#configure_widget_parameters_modal" class="btn btn-primary">Next</button>
        <button type="button" id="add_widget_cancel" data-dismiss="modal" class="btn btn-default add_widget_cancel">Cancel</button>
      </div>
    </div>
  </div>
</div>

        <div id="configure_widget_parameters_modal" class="modal">
  <div class="modal-dialog window-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <span class="close"> &nbsp; </span>
        <button onclick="window.open('https://www.mathworks.com/help/thingspeak/channel_display_widgets.html', '_blank');" target="_blank" id="widget_config_modal_faq" class="close"><span aria-hidden="true">?</span></button>
        <h4 class="modal-title">Configure widget parameters</h4>
      </div>
      <div class="modal-body window-body">
        <div id="gauge_min_max_error" class="alert alert-danger alert-dismissable error_banner" style="display:none; clear:both">
  <a id="gauge_min_max_error_close" href="#" class="close" aria-label="close"><i class="fa fa-close" aria-hidden="true"></i></a>
  <span id="min_max_error_span">Max Value should be greater than Min Value</span>
</div>

<div id="units_error" class="alert alert-danger alert-dismissable error_banner" style="display:none; clear:both">
  <a id="units_error_close" href="#" class="close" aria-label="close"><i class="fa fa-close" aria-hidden="true"></i></a>
  <span id="units_error_span">Numbers not supported in units field.</span>
</div>
        <div id="configure_widget_modal_content_body">
        </div>
      </div>
      <div class="modal-footer window-footer">
        <button type="button" id="add_widget_create" data-dismiss="modal"  class="btn btn-primary">Create</button>
        <button type="button" id="add_widget_cancel" data-dismiss="modal" class="btn btn-default add_widget_cancel">Cancel</button>
      </div>
    </div>
  </div>
</div>

        <button type="button" data-toggle="modal" data-target="#add_visualization_modal" class="btn btn-default btn-margin-bottom" ><i class='fa fa-plus-square timecontrol_index'></i>&nbsp;Add Visualizations</button>
        <button type="button" data-toggle="modal" data-target="#add_widget_modal" class="btn btn-default btn-margin-bottom" ><i class='fa fa-plus-square timecontrol_index'></i>&nbsp;Add Widgets</button>
      <div id="devinfo_modal" class="modal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title">Export recent data</h4>
      </div>
      <div class="modal-body">

        <table class="table table-striped" >
          <tr>
            <td>home Automation Channel Feed:</td>
            <td>
              <a target="_blank" href="/channels/1370705/feed.json">JSON</a>
              <a target="_blank" href="/channels/1370705/feed.xml">XML</a>
              <a target="_blank" href="/channels/1370705/feed.csv">CSV</a>
            </td>
          </tr>

              <tr>
                <td>Field 1 Data:  Field Label 1 </td>
                <td>
                  <a target="_blank" href="/channels/1370705/field/1.json">JSON</a>
                  <a target="_blank" href="/channels/1370705/field/1.xml">XML</a>
                  <a target="_blank" href="/channels/1370705/field/1.csv">CSV</a>
                </td>
              </tr>
              <tr>
                <td>Field 2 Data:  Field Label 2 </td>
                <td>
                  <a target="_blank" href="/channels/1370705/field/2.json">JSON</a>
                  <a target="_blank" href="/channels/1370705/field/2.xml">XML</a>
                  <a target="_blank" href="/channels/1370705/field/2.csv">CSV</a>
                </td>
              </tr>
              <tr>
                <td>Field 3 Data:  Field Label 3 </td>
                <td>
                  <a target="_blank" href="/channels/1370705/field/3.json">JSON</a>
                  <a target="_blank" href="/channels/1370705/field/3.xml">XML</a>
                  <a target="_blank" href="/channels/1370705/field/3.csv">CSV</a>
                </td>
              </tr>
        </table>

      </div>
    </div>
  </div>
</div>

      <button type="button" data-toggle="modal" data-target="#devinfo_modal" class="btn btn-default btn-margin-bottom" id="channel-data-export-button"><i class='fa fa-external-link-square timecontrol_index'></i>&nbsp;Export recent data</button>


    
  </div>

  <div class="col-sm-6 hidden-xs">
    <div class="pull-right">
        <a class="btn btn-primary btn-margin-bottom" id="channel-matlab-analysis-button" href="/apps/matlab_analyses/templates">MATLAB Analysis</a>
        <a class="btn btn-primary btn-margin-bottom" id="channel-matlab-visualization-button" href="/apps/matlab_visualizations/templates?channel_id=1370705&amp;is_private_view=true">MATLAB Visualization</a>
    </div>
  </div>
</div>
    <div class= "pull-right" data-turbolinks="false">
     </div>

  <div class="row">
    <div class="col-xs-12">
      <h2>Channel Stats</h2>
      <ul class="no_bullets">
        <li>Created: <abbr class="timeago channel_time_text" title="2021-04-25T13:14:55Z" >2021-04-25T13:14:55Z</abbr></li>
          <li>Last entry: <abbr id="channel-last-written-at" class="timeago channel_time_text" title="2021-04-25T19:24:42Z" >2021-04-25T19:24:42Z</abbr></li>
        <li>Entries: <span id="channel-entry-count">175</span></li>
      </ul>
    </div>
  </div>
  
  <script> var channelURL = '/channels/' + 1370705 + '/feeds/last.json'; </script>
  
  <script>
//<![CDATA[
function updateChannelInfo(){
        setInterval(function(){
          jQuery.ajax({url: channelURL})
            .done(function(data){
               if (null !== data){
                 // update the last written at element
                  element = document.getElementById('channel-last-written-at');
                  if (null !== element && undefined !== data.created_at) {
                    // store the previous entry and compare with current. If we get an older date, ignore it.
                    max_created_at = new Date(element.title);
                    current_created_at = new Date(data.created_at);
                    if (current_created_at > max_created_at) {max_created_at = current_created_at;}
                    parentNode = element.parentNode;
                    max_created_at = max_created_at.toISOString();
                    newElement = document.createElement('abbr');
                    newElement.setAttribute('id','channel-last-written-at');
                    newElement.setAttribute('class','timeago channel_time_text');
                    newElement.setAttribute('title',max_created_at);
                    newElement.innerText = jQuery.timeago(max_created_at);
                    // Add element and remove the existing element as it is tied to a timeago timer
                    if (parentNode) {parentNode.appendChild(newElement);parentNode.removeChild(element);}
                  }
                  // update number of entries
                  element = document.getElementById('channel-entry-count');
                  if (null !== element) {
                    oldValue = parseInt(element.innerText);
                    // last.json will return -1 when there are no entries in the channel
                    if (data == -1){
                      // If the old value was >0 and we got a -1, then channel was cleared in another tab
                      if (oldValue > 0) {
                        // channel was cleared. reload page
                        location.reload();
                      }
                    }
                    // Update the entry_id with the entry_id we get back from the call
                    else {
                      if (undefined !== data.entry_id) {
                        // Entry_id for a field's last.json may be less than entry_id of the feed of the channel. Assuming the largest value is the correct one.
                        if (parseInt(data.entry_id) > oldValue) {element.innerText = data.entry_id;}
                      }
                    }
                  }
               }
            });
        },15000);
      }
      updateChannelInfo();
      
//]]>
</script>
  

    <br>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Sortable/1.4.2/Sortable.min.js"></script>

<div class="row">
  <div class="col-xs-12 col-sm-12 col-md-12">
    <div id="windows_container">
        <script src="/assets/widget-325d0bf7906d9f455624f0a03a9a1e0f600d5f41aa1f573eae24505f7a66ebe6.js" data-turbolinks-track="reload"></script>
<link rel="stylesheet" media="screen" href="/assets/widget-1057f0bbd162015136004c3afc35308fef75815b238ff469e1b3705ebd83f4e8.css" />

<div id="window_8187761" class="window-container">
  <div title="Field 1 Chart" class="window-header">  
    <div class="window-title">Field 1 Chart</div>
    <div id="controls" class="window-controls">
        <div id="remove_window_8187761" class="window-icon"><i class="fa fa-times fa-lg"></i></div>
          <div id="options_modal_open_8187761" title="Field 1 Chart Options" class="window-icon" data-toggle="modal" data-target="#window_options_modal_8187761"><i class="fa fa-pencil fa-lg"></i></div>
      <div id="iframe_modal_open_8187761" title="Field 1 Chart IFrame" class="window-icon" data-toggle="modal" data-target="#window_iframe_modal_8187761"><i class="fa fa-comment-o fa-lg"></i></div>
      <div style="padding-top: 2px;">
        <a target="_blank" class="chart-header" href="/channels/1370705/charts/1?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15">
           <i class="fa fa-external-link fa-lg"></i>
</a>      </div>

    </div>
  </div>
  <div class="window-content">
    <iframe id="window_iframe_8187761" class="window-iframe" src="/channels/1370705/charts/1?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15"></iframe>
  </div>
</div>

<div id="window_iframe_modal_8187761" class="modal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button id="iframe_modal_close_8187761" type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>         
        <h4 class="modal-title">Field 1 Chart&nbsp;IFrame</h4>
      </div>
      <div class="modal-body">
        <div id="iframe_modal_content_body_8187761" >
          <pre id="iframe_modal_pre_8187761">&lt;iframe width=&quot;450&quot; height=&quot;260&quot; style=&quot;border: 1px solid #cccccc;&quot; src=&quot;https://thingspeak.com/channels/1370705/charts/1?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15&quot;&gt;&lt;/iframe&gt;</pre>
        </div>
      </div>
    </div>
  </div>
</div>

<div id="window_options_modal_8187761" class="modal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button id="options_modal_close_8187761" type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title">Field 1 Chart&nbsp;Options</h4>
      </div>
      <div class="modal-body">
        <div id="options_modal_content_body_8187761" >
          <div class="row form-group">
  <div class="col-md-6 col-sm-6 col-xs-6">
    <table>
      <tr>
        <td>
          Title:</td>
        <td>
          <input type="text" name="options[title]" id="options_title" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          X-Axis:</td>
        <td>
          <input type="text" name="options[xaxis]" id="options_xaxis" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis:</td>
        <td>
          <input type="text" name="options[yaxis]" id="options_yaxis" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Color:</td>
        <td>
          <input type="text" name="options[color]" id="options_color" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Background:</td>
        <td>
          <input type="text" name="options[bgcolor]" id="options_bgcolor" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Type:</td>
        <td>
          <select name="options[type]" id="options_type" class="form-control"><option value="line">line</option>
<option value="bar">bar</option>
<option value="column">column</option>
<option value="spline">spline</option>
<option value="step">step</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Dynamic?:</td>
        <td>
          <select name="options[dynamic]" id="options_dynamic" class="form-control"><option value="true">true</option>
<option value="false">false</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Days:</td>
        <td>
          <input type="text" name="options[days]" id="options_days" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Results:</td>
        <td>
          <input type="text" name="options[results]" id="options_results" value="" class="form-control" />
        </td>
      </tr>
    </table>
  </div>
  <div class="col-md-6 col-sm-6 col-xs-6">
    <table>
      <tr>
        <td>
          Timescale:</td>
        <td>
          <select name="options[timescale]" id="options_timescale" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Average:</td>
        <td>
          <select name="options[average]" id="options_average" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Median:</td>
        <td>
          <select name="options[median]" id="options_median" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Sum:</td>
        <td>
          <select name="options[sum]" id="options_sum" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Rounding:</td>
        <td>
          <input type="text" name="options[round]" id="options_round" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Data Min: </td>
        <td>
          <input type="text" name="options[min]" id="options_min" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Data Max: </td>
        <td>
          <input type="text" name="options[max]" id="options_max" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis Min: </td>
        <td>
          <input type="text" name="options[yaxismin]" id="options_yaxismin" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis Max: </td>
        <td>
          <input type="text" name="options[yaxismax]" id="options_yaxismax" value="" class="form-control" />
        </td>
      </tr>
    </table>
  </div>
</div>

        </div>
      </div>
      <div class="modal-footer window-footer">
        <button id="window_options_modal_save_8187761" type="button" class="btn btn-primary">Save</button>
        <button id="window_options_modal_cancel_8187761" type="button" data-dismiss="modal" class="btn btn-default">Cancel</button>
      </div>
    </div>
  </div>
</div>


        <script src="/assets/widget-325d0bf7906d9f455624f0a03a9a1e0f600d5f41aa1f573eae24505f7a66ebe6.js" data-turbolinks-track="reload"></script>
<link rel="stylesheet" media="screen" href="/assets/widget-1057f0bbd162015136004c3afc35308fef75815b238ff469e1b3705ebd83f4e8.css" />

<div id="window_8187762" class="window-container">
  <div title="Field 2 Chart" class="window-header">  
    <div class="window-title">Field 2 Chart</div>
    <div id="controls" class="window-controls">
        <div id="remove_window_8187762" class="window-icon"><i class="fa fa-times fa-lg"></i></div>
          <div id="options_modal_open_8187762" title="Field 2 Chart Options" class="window-icon" data-toggle="modal" data-target="#window_options_modal_8187762"><i class="fa fa-pencil fa-lg"></i></div>
      <div id="iframe_modal_open_8187762" title="Field 2 Chart IFrame" class="window-icon" data-toggle="modal" data-target="#window_iframe_modal_8187762"><i class="fa fa-comment-o fa-lg"></i></div>
      <div style="padding-top: 2px;">
        <a target="_blank" class="chart-header" href="/channels/1370705/charts/2?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15">
           <i class="fa fa-external-link fa-lg"></i>
</a>      </div>

    </div>
  </div>
  <div class="window-content">
    <iframe id="window_iframe_8187762" class="window-iframe" src="/channels/1370705/charts/2?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15"></iframe>
  </div>
</div>

<div id="window_iframe_modal_8187762" class="modal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button id="iframe_modal_close_8187762" type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>         
        <h4 class="modal-title">Field 2 Chart&nbsp;IFrame</h4>
      </div>
      <div class="modal-body">
        <div id="iframe_modal_content_body_8187762" >
          <pre id="iframe_modal_pre_8187762">&lt;iframe width=&quot;450&quot; height=&quot;260&quot; style=&quot;border: 1px solid #cccccc;&quot; src=&quot;https://thingspeak.com/channels/1370705/charts/2?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15&quot;&gt;&lt;/iframe&gt;</pre>
        </div>
      </div>
    </div>
  </div>
</div>

<div id="window_options_modal_8187762" class="modal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button id="options_modal_close_8187762" type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title">Field 2 Chart&nbsp;Options</h4>
      </div>
      <div class="modal-body">
        <div id="options_modal_content_body_8187762" >
          <div class="row form-group">
  <div class="col-md-6 col-sm-6 col-xs-6">
    <table>
      <tr>
        <td>
          Title:</td>
        <td>
          <input type="text" name="options[title]" id="options_title" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          X-Axis:</td>
        <td>
          <input type="text" name="options[xaxis]" id="options_xaxis" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis:</td>
        <td>
          <input type="text" name="options[yaxis]" id="options_yaxis" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Color:</td>
        <td>
          <input type="text" name="options[color]" id="options_color" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Background:</td>
        <td>
          <input type="text" name="options[bgcolor]" id="options_bgcolor" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Type:</td>
        <td>
          <select name="options[type]" id="options_type" class="form-control"><option value="line">line</option>
<option value="bar">bar</option>
<option value="column">column</option>
<option value="spline">spline</option>
<option value="step">step</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Dynamic?:</td>
        <td>
          <select name="options[dynamic]" id="options_dynamic" class="form-control"><option value="true">true</option>
<option value="false">false</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Days:</td>
        <td>
          <input type="text" name="options[days]" id="options_days" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Results:</td>
        <td>
          <input type="text" name="options[results]" id="options_results" value="" class="form-control" />
        </td>
      </tr>
    </table>
  </div>
  <div class="col-md-6 col-sm-6 col-xs-6">
    <table>
      <tr>
        <td>
          Timescale:</td>
        <td>
          <select name="options[timescale]" id="options_timescale" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Average:</td>
        <td>
          <select name="options[average]" id="options_average" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Median:</td>
        <td>
          <select name="options[median]" id="options_median" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Sum:</td>
        <td>
          <select name="options[sum]" id="options_sum" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Rounding:</td>
        <td>
          <input type="text" name="options[round]" id="options_round" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Data Min: </td>
        <td>
          <input type="text" name="options[min]" id="options_min" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Data Max: </td>
        <td>
          <input type="text" name="options[max]" id="options_max" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis Min: </td>
        <td>
          <input type="text" name="options[yaxismin]" id="options_yaxismin" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis Max: </td>
        <td>
          <input type="text" name="options[yaxismax]" id="options_yaxismax" value="" class="form-control" />
        </td>
      </tr>
    </table>
  </div>
</div>

        </div>
      </div>
      <div class="modal-footer window-footer">
        <button id="window_options_modal_save_8187762" type="button" class="btn btn-primary">Save</button>
        <button id="window_options_modal_cancel_8187762" type="button" data-dismiss="modal" class="btn btn-default">Cancel</button>
      </div>
    </div>
  </div>
</div>


        <script src="/assets/widget-325d0bf7906d9f455624f0a03a9a1e0f600d5f41aa1f573eae24505f7a66ebe6.js" data-turbolinks-track="reload"></script>
<link rel="stylesheet" media="screen" href="/assets/widget-1057f0bbd162015136004c3afc35308fef75815b238ff469e1b3705ebd83f4e8.css" />

<div id="window_8187763" class="window-container">
  <div title="Field 3 Chart" class="window-header">  
    <div class="window-title">Field 3 Chart</div>
    <div id="controls" class="window-controls">
        <div id="remove_window_8187763" class="window-icon"><i class="fa fa-times fa-lg"></i></div>
          <div id="options_modal_open_8187763" title="Field 3 Chart Options" class="window-icon" data-toggle="modal" data-target="#window_options_modal_8187763"><i class="fa fa-pencil fa-lg"></i></div>
      <div id="iframe_modal_open_8187763" title="Field 3 Chart IFrame" class="window-icon" data-toggle="modal" data-target="#window_iframe_modal_8187763"><i class="fa fa-comment-o fa-lg"></i></div>
      <div style="padding-top: 2px;">
        <a target="_blank" class="chart-header" href="/channels/1370705/charts/3?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15">
           <i class="fa fa-external-link fa-lg"></i>
</a>      </div>

    </div>
  </div>
  <div class="window-content">
    <iframe id="window_iframe_8187763" class="window-iframe" src="/channels/1370705/charts/3?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15"></iframe>
  </div>
</div>

<div id="window_iframe_modal_8187763" class="modal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button id="iframe_modal_close_8187763" type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>         
        <h4 class="modal-title">Field 3 Chart&nbsp;IFrame</h4>
      </div>
      <div class="modal-body">
        <div id="iframe_modal_content_body_8187763" >
          <pre id="iframe_modal_pre_8187763">&lt;iframe width=&quot;450&quot; height=&quot;260&quot; style=&quot;border: 1px solid #cccccc;&quot; src=&quot;https://thingspeak.com/channels/1370705/charts/3?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15&quot;&gt;&lt;/iframe&gt;</pre>
        </div>
      </div>
    </div>
  </div>
</div>

<div id="window_options_modal_8187763" class="modal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button id="options_modal_close_8187763" type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title">Field 3 Chart&nbsp;Options</h4>
      </div>
      <div class="modal-body">
        <div id="options_modal_content_body_8187763" >
          <div class="row form-group">
  <div class="col-md-6 col-sm-6 col-xs-6">
    <table>
      <tr>
        <td>
          Title:</td>
        <td>
          <input type="text" name="options[title]" id="options_title" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          X-Axis:</td>
        <td>
          <input type="text" name="options[xaxis]" id="options_xaxis" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis:</td>
        <td>
          <input type="text" name="options[yaxis]" id="options_yaxis" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Color:</td>
        <td>
          <input type="text" name="options[color]" id="options_color" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Background:</td>
        <td>
          <input type="text" name="options[bgcolor]" id="options_bgcolor" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Type:</td>
        <td>
          <select name="options[type]" id="options_type" class="form-control"><option value="line">line</option>
<option value="bar">bar</option>
<option value="column">column</option>
<option value="spline">spline</option>
<option value="step">step</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Dynamic?:</td>
        <td>
          <select name="options[dynamic]" id="options_dynamic" class="form-control"><option value="true">true</option>
<option value="false">false</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Days:</td>
        <td>
          <input type="text" name="options[days]" id="options_days" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Results:</td>
        <td>
          <input type="text" name="options[results]" id="options_results" value="" class="form-control" />
        </td>
      </tr>
    </table>
  </div>
  <div class="col-md-6 col-sm-6 col-xs-6">
    <table>
      <tr>
        <td>
          Timescale:</td>
        <td>
          <select name="options[timescale]" id="options_timescale" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Average:</td>
        <td>
          <select name="options[average]" id="options_average" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Median:</td>
        <td>
          <select name="options[median]" id="options_median" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Sum:</td>
        <td>
          <select name="options[sum]" id="options_sum" class="mutuallyexclusive form-control"><option value="" label=" "></option><option value="10">10</option>
<option value="15">15</option>
<option value="20">20</option>
<option value="30">30</option>
<option value="60">60</option>
<option value="240">240</option>
<option value="720">720</option>
<option value="1440">1440</option>
<option value="daily">daily</option></select>
        </td>
      </tr>
      <tr>
        <td>
          Rounding:</td>
        <td>
          <input type="text" name="options[round]" id="options_round" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Data Min: </td>
        <td>
          <input type="text" name="options[min]" id="options_min" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Data Max: </td>
        <td>
          <input type="text" name="options[max]" id="options_max" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis Min: </td>
        <td>
          <input type="text" name="options[yaxismin]" id="options_yaxismin" value="" class="form-control" />
        </td>
      </tr>
      <tr>
        <td>
          Y-Axis Max: </td>
        <td>
          <input type="text" name="options[yaxismax]" id="options_yaxismax" value="" class="form-control" />
        </td>
      </tr>
    </table>
  </div>
</div>

        </div>
      </div>
      <div class="modal-footer window-footer">
        <button id="window_options_modal_save_8187763" type="button" class="btn btn-primary">Save</button>
        <button id="window_options_modal_cancel_8187763" type="button" data-dismiss="modal" class="btn btn-default">Cancel</button>
      </div>
    </div>
  </div>
</div>


    </div>

      <div id="add_visualization_window" class="add_visualization_window" data-toggle="modal" data-target="#add_visualization_modal"><i class='fa fa-plus-square timecontrol_index'></i>&nbsp;Add Visualizations</div>
  </div>
</div>

<script type="text/javascript">
  $(document).on('page:load ready', function (){
    window.channel = ThingSpeak.Channel.init({"public_view":false,"current_user_owns":true,"windows":[{"id":8187761,"channel_id":1370705,"position":1,"created_at":"2021-04-25T13:14:55Z","updated_at":"2021-04-25T13:14:55Z","content_type":"chart","public_flag":false,"content_id":1,"options":"bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","options_json":"{\"bgcolor\":\"#ffffff\",\"color\":\"#d62020\",\"dynamic\":\"true\",\"results\":\"60\",\"type\":\"line\",\"update\":\"15\"}","iframe_html":"\u003ciframe width=\"450\" height=\"260\" style=\"border: 1px solid #cccccc;\" src=\"https://thingspeak.com/channels/1370705/charts/1?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15\"\u003e\u003c/iframe\u003e","iframe_src":"/channels/1370705/charts/1?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","preview_image_path":"/assets/add_visualization_chart-a41736c2720006799b06e29c3b76d24b02ce64ea9bd73d824af0809474953d02.svg","url":"/channels/1370705/windows/8187761","title":"Field 1 Chart"},{"id":8187802,"channel_id":1370705,"position":1,"created_at":"2021-04-25T13:28:12Z","updated_at":"2021-04-25T13:28:12Z","content_type":"chart","public_flag":true,"content_id":1,"options":"bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","options_json":"{\"bgcolor\":\"#ffffff\",\"color\":\"#d62020\",\"dynamic\":\"true\",\"results\":\"60\",\"type\":\"line\",\"update\":\"15\"}","iframe_html":"\u003ciframe width=\"450\" height=\"260\" style=\"border: 1px solid #cccccc;\" src=\"https://thingspeak.com/channels/1370705/charts/1?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15\"\u003e\u003c/iframe\u003e","iframe_src":"/channels/1370705/charts/1?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","preview_image_path":"/assets/add_visualization_chart-a41736c2720006799b06e29c3b76d24b02ce64ea9bd73d824af0809474953d02.svg","url":"/channels/1370705/windows/8187802","title":"Field 1 Chart"},{"id":8187762,"channel_id":1370705,"position":2,"created_at":"2021-04-25T13:14:55Z","updated_at":"2021-04-25T13:14:55Z","content_type":"chart","public_flag":false,"content_id":2,"options":"bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","options_json":"{\"bgcolor\":\"#ffffff\",\"color\":\"#d62020\",\"dynamic\":\"true\",\"results\":\"60\",\"type\":\"line\",\"update\":\"15\"}","iframe_html":"\u003ciframe width=\"450\" height=\"260\" style=\"border: 1px solid #cccccc;\" src=\"https://thingspeak.com/channels/1370705/charts/2?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15\"\u003e\u003c/iframe\u003e","iframe_src":"/channels/1370705/charts/2?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","preview_image_path":"/assets/add_visualization_chart-a41736c2720006799b06e29c3b76d24b02ce64ea9bd73d824af0809474953d02.svg","url":"/channels/1370705/windows/8187762","title":"Field 2 Chart"},{"id":8187803,"channel_id":1370705,"position":2,"created_at":"2021-04-25T13:28:12Z","updated_at":"2021-04-25T13:28:12Z","content_type":"chart","public_flag":true,"content_id":2,"options":"bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","options_json":"{\"bgcolor\":\"#ffffff\",\"color\":\"#d62020\",\"dynamic\":\"true\",\"results\":\"60\",\"type\":\"line\",\"update\":\"15\"}","iframe_html":"\u003ciframe width=\"450\" height=\"260\" style=\"border: 1px solid #cccccc;\" src=\"https://thingspeak.com/channels/1370705/charts/2?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15\"\u003e\u003c/iframe\u003e","iframe_src":"/channels/1370705/charts/2?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","preview_image_path":"/assets/add_visualization_chart-a41736c2720006799b06e29c3b76d24b02ce64ea9bd73d824af0809474953d02.svg","url":"/channels/1370705/windows/8187803","title":"Field 2 Chart"},{"id":8187763,"channel_id":1370705,"position":3,"created_at":"2021-04-25T13:14:55Z","updated_at":"2021-04-25T13:14:55Z","content_type":"chart","public_flag":false,"content_id":3,"options":"bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","options_json":"{\"bgcolor\":\"#ffffff\",\"color\":\"#d62020\",\"dynamic\":\"true\",\"results\":\"60\",\"type\":\"line\",\"update\":\"15\"}","iframe_html":"\u003ciframe width=\"450\" height=\"260\" style=\"border: 1px solid #cccccc;\" src=\"https://thingspeak.com/channels/1370705/charts/3?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15\"\u003e\u003c/iframe\u003e","iframe_src":"/channels/1370705/charts/3?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","preview_image_path":"/assets/add_visualization_chart-a41736c2720006799b06e29c3b76d24b02ce64ea9bd73d824af0809474953d02.svg","url":"/channels/1370705/windows/8187763","title":"Field 3 Chart"},{"id":8187804,"channel_id":1370705,"position":3,"created_at":"2021-04-25T13:28:12Z","updated_at":"2021-04-25T13:28:12Z","content_type":"chart","public_flag":true,"content_id":3,"options":"bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","options_json":"{\"bgcolor\":\"#ffffff\",\"color\":\"#d62020\",\"dynamic\":\"true\",\"results\":\"60\",\"type\":\"line\",\"update\":\"15\"}","iframe_html":"\u003ciframe width=\"450\" height=\"260\" style=\"border: 1px solid #cccccc;\" src=\"https://thingspeak.com/channels/1370705/charts/3?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15\"\u003e\u003c/iframe\u003e","iframe_src":"/channels/1370705/charts/3?bgcolor=%23ffffff\u0026color=%23d62020\u0026dynamic=true\u0026results=60\u0026type=line\u0026update=15","preview_image_path":"/assets/add_visualization_chart-a41736c2720006799b06e29c3b76d24b02ce64ea9bd73d824af0809474953d02.svg","url":"/channels/1370705/windows/8187804","title":"Field 3 Chart"}],"channel":{"id":1370705,"user_id":704468,"name":"home Automation","description":"","latitude":"0.0","longitude":"0.0","field1":"Field Label 1","field2":"Field Label 2","field3":"Field Label 3","field4":null,"field5":null,"field6":null,"field7":null,"field8":null,"scale1":null,"scale2":null,"scale3":null,"scale4":null,"scale5":null,"scale6":null,"scale7":null,"scale8":null,"created_at":"2021-04-25T13:14:55Z","updated_at":"2021-04-25T13:28:12Z","elevation":"","last_entry_id":175,"public_flag":true,"options1":null,"options2":null,"options3":null,"options4":null,"options5":null,"options6":null,"options7":null,"options8":null,"status":null,"url":"","video_id":null,"video_type":"youtube","clearing":false,"ranking":30,"user_agent":null,"realtime_io_serial_number":null,"metadata":"","last_write_at":null,"batch_updated_at":null,"show_location":false,"show_video":false,"show_status":false,"license_id":0,"is_updating":null,"is_privately_shared_flag":false,"github_url":null}});
  })
</script>

  </div>
</div>
<script src="https://cdn.jsdelivr.net/momentjs/2.17.1/moment.min.js"></script>
<script>
//<![CDATA[
var meter_data = {"licenses":[{"id":2166125,"license_id":-704468,"licensed_prod_id":-704468,"qty":1,"start_date":"2021-04-25","end_date":"2022-04-24","offering_id":0,"created_at":"2021-04-25T13:13:52.000Z","updated_at":"2021-04-25T13:13:52.000Z","service_date_id":null,"messages_remaining":2999878,"messages_allowed":3000000}],"domain":"https://thingspeak.com/","messages_per_paid_unit":"33000000","free_messages_per_year":"3000000","license_center_link":"https://www.mathworks.com/licensecenter/licenses/:lid","user_type":0,"is_free_user":true,"free_license_id":-704468,"license_type":"Free"}
//]]>
</script>
<script type="text/javascript">
 if( meter_data !== null )
  {
  	loadMeterData(meter_data);
  } 
</script>

<script>
//<![CDATA[
$('#available_licenses').tooltip();
//]]>
</script>

          <script src="https://login.mathworks.com/embedded-login/js/dotcom_embedded_status.js"></script>
<script>
try {
  MWEmbeddedStatus.initialize({
    clientString: "TSPK", 
    embeddedEndpoint: "https://login.mathworks.com/embedded-login/",
    logout: function(){
      window.location.href = "/logout";
    },
    synced: function(){
      redirectToEmbeddedLogin();
    },
    handle3PCookieDisabled: function(){
      redirectToEmbeddedLogin();
    }
  });

  MWEmbeddedStatus.prototype.logout = function(){
    document.cookie = "mwa_SID=;path=/";
    MWEmbeddedStatus.instance.config.logout();
  };

  // to enable SSO in local development and test environments
} catch (error) {
  // pages with links that don't have turbolinks disabled won't load the SSO Status API,
  // or for browsers that don't allow 3p cookies by default, render embedded login form
  if (typeof MWEmbeddedStatus === "undefined"){
    window.location.replace("/login" + "?skipSSOCheck=true");
  }
}

function redirectToEmbeddedLogin(){
  let skipSSOCheckPath = "/login/mwa-sso/check";
  // redirect the user to embedded login page if a synced event is received and the current pathname points to /login/mwa-sso/check
  if (window.location.pathname === skipSSOCheckPath) {
    window.location.replace("/login" + "?skipSSOCheck=true"); 
  }
}
</script>

      </div>
    </div>

    <script type="text/javascript">
var cookieBanner ={
   /* Hide the cookie banner if it was accepted in the last year */
   showIfNotAccepted: function(){
     if ( localStorage ) {
       lastCookieNotificationAcceptedDate = parseInt(localStorage.getItem('tspk-cookie-banner'));
       /* 31536000000 is the number of milliseconds since 365 days ago */
       if (  isNaN(lastCookieNotificationAcceptedDate) || ( lastCookieNotificationAcceptedDate < ((new Date).getTime() - 31536000000) ) ){
         $("#cookie-banner").show();
       } else {
         $("#cookie-banner").hide();
       }
     }
   },

   /* Store time when the cookie notification was accepted in the browser local storage for this site */
   setAcceptanceTime: function() {
     if ( localStorage ) {
       localStorage.setItem('tspk-cookie-banner',(new Date).getTime());
       cookieBanner.showIfNotAccepted();
     }
   }

};
</script>

<div id="cookie-banner" class="cookie-alert-warning">
  <script type="text/javascript">cookieBanner.showIfNotAccepted();</script>
  <div id="cookie-icon" class="text-right"><span class="fa fa-exclamation-triangle"></span></div>
  <div id="cookie-text"><p>This website uses cookies to improve your user experience, personalize content and ads, and analyze website traffic. By continuing to use this website, you consent to our use of cookies. Please see our <a target="_blank" style="font-size: small" href="https://www.mathworks.com/company/aboutus/policies_statements">Privacy Policy</a> to learn more about cookies and how to change your settings.</p></div>
  <div id="cookie-remove"><span class="glyphicon glyphicon-remove" onclick="cookieBanner.setAcceptanceTime();return false;"></span></div>
</div>
    <div id="footer">
  <div class="container">
    <p>
      <span class="hidden-xs pull-left">
        <a href="https://blogs.mathworks.com/iot/" title="IoT Blog" target="_blank">Blog</a> |
        <a href="https://www.mathworks.com/help/thingspeak/" title="ThingSpeak Documentation" target="_blank">Documentation</a> |
        <a href="https://www.mathworks.com/help/thingspeak/getting-started-with-thingspeak.html" title="ThingSpeak Tutorials" target="_blank">Tutorials</a> |
        <a target="_blank" href="https://www.mathworks.com/mw_account/company/aboutus/policies_statements/online-services-agreement.html">Terms</a> |
        <a target="_blank" href="https://www.mathworks.com/company/aboutus/policies_statements">Privacy Policy</a>
      </span>
      <span class="pull-right">
        <a alt="Facebook" target="_blank" href="http://www.facebook.com/thingspeak"><img src="/assets/ico-facebook-864217e7723b63bd8687c81e99e677c0a1efba1db6282794f4077f3d6d5cae86.svg" width="16" height="16" /></a>
        <a alt="Twitter" target="_blank" href="http://www.twitter.com/thingspeak"><img src="/assets/ico-twitter-502ca920ad71f398928c9ec00203b98655f8b1ba821b95f4cf11b4eef72b6d4b.svg" width="16" height="16" /></a>
        <a alt="RSS" target="_blank" href="http://feeds.feedburner.com/internetofthings"><img src="/assets/ico-rss-349a27d6441a574f9218ee6e808d147dc5566204c79d967cf90b33b0bd026171.svg" width="16" height="16" /></a>
        &emsp;&copy; 2021 <a href="https://www.mathworks.com/" target="_blank">The MathWorks, Inc.</a>
      </span>
    </p>
  </div>
</div>

<!-- Qualaroo for thingspeak.com -->
<script type="text/javascript">
  var _kiq = _kiq || [];
  (function(){
    setTimeout(function(){
    var d = document, f = d.getElementsByTagName('script')[0], s = d.createElement('script'); s.type = 'text/javascript';
    s.async = true; s.src = 'https://cl.qualaroo.com/ki.js/49559/htZ.js'; f.parentNode.insertBefore(s, f);
    }, 1);
  })();
</script>

    <script type="text/javascript">_satellite.pageBottom();</script>

  </body>
</html>
```
