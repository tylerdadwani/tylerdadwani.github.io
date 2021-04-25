
```html
<html style="height: 100%;">

<head>
<script>window.NREUM||(NREUM={});NREUM.info={"beacon":"bam-cell.nr-data.net","errorBeacon":"bam-cell.nr-data.net","licenseKey":"199e8a4832","applicationID":"2972453","transactionName":"c11cQBFeWw5TSh9TXlFARkdMQl8NQQ==","queueTime":0,"applicationTime":7,"agent":""}</script>
<script>(window.NREUM||(NREUM={})).loader_config={licenseKey:"199e8a4832",applicationID:"2972453"};window.NREUM||(NREUM={}),__nr_require=function(e,t,n){function r(n){if(!t[n]){var i=t[n]={exports:{}};e[n][0].call(i.exports,function(t){var i=e[n][1][t];return r(i||t)},i,i.exports)}return t[n].exports}if("function"==typeof __nr_require)return __nr_require;for(var i=0;i<n.length;i++)r(n[i]);return r}({1:[function(e,t,n){function r(){}function i(e,t,n){return function(){return o(e,[u.now()].concat(c(arguments)),t?null:this,n),t?void 0:this}}var o=e("handle"),a=e(7),c=e(8),f=e("ee").get("tracer"),u=e("loader"),s=NREUM;"undefined"==typeof window.newrelic&&(newrelic=s);var d=["setPageViewName","setCustomAttribute","setErrorHandler","finished","addToTrace","inlineHit","addRelease"],p="api-",l=p+"ixn-";a(d,function(e,t){s[t]=i(p+t,!0,"api")}),s.addPageAction=i(p+"addPageAction",!0),s.setCurrentRouteName=i(p+"routeName",!0),t.exports=newrelic,s.interaction=function(){return(new r).get()};var m=r.prototype={createTracer:function(e,t){var n={},r=this,i="function"==typeof t;return o(l+"tracer",[u.now(),e,n],r),function(){if(f.emit((i?"":"no-")+"fn-start",[u.now(),r,i],n),i)try{return t.apply(this,arguments)}catch(e){throw f.emit("fn-err",[arguments,this,e],n),e}finally{f.emit("fn-end",[u.now()],n)}}}};a("actionText,setName,setAttribute,save,ignore,onEnd,getContext,end,get".split(","),function(e,t){m[t]=i(l+t)}),newrelic.noticeError=function(e,t){"string"==typeof e&&(e=new Error(e)),o("err",[e,u.now(),!1,t])}},{}],2:[function(e,t,n){function r(){return c.exists&&performance.now?Math.round(performance.now()):(o=Math.max((new Date).getTime(),o))-a}function i(){return o}var o=(new Date).getTime(),a=o,c=e(9);t.exports=r,t.exports.offset=a,t.exports.getLastTimestamp=i},{}],3:[function(e,t,n){function r(e){return!(!e||!e.protocol||"file:"===e.protocol)}t.exports=r},{}],4:[function(e,t,n){function r(e,t){var n=e.getEntries();n.forEach(function(e){"first-paint"===e.name?d("timing",["fp",Math.floor(e.startTime)]):"first-contentful-paint"===e.name&&d("timing",["fcp",Math.floor(e.startTime)])})}function i(e,t){var n=e.getEntries();n.length>0&&d("lcp",[n[n.length-1]])}function o(e){e.getEntries().forEach(function(e){e.hadRecentInput||d("cls",[e])})}function a(e){if(e instanceof m&&!g){var t=Math.round(e.timeStamp),n={type:e.type};t<=p.now()?n.fid=p.now()-t:t>p.offset&&t<=Date.now()?(t-=p.offset,n.fid=p.now()-t):t=p.now(),g=!0,d("timing",["fi",t,n])}}function c(e){d("pageHide",[p.now(),e])}if(!("init"in NREUM&&"page_view_timing"in NREUM.init&&"enabled"in NREUM.init.page_view_timing&&NREUM.init.page_view_timing.enabled===!1)){var f,u,s,d=e("handle"),p=e("loader"),l=e(6),m=NREUM.o.EV;if("PerformanceObserver"in window&&"function"==typeof window.PerformanceObserver){f=new PerformanceObserver(r);try{f.observe({entryTypes:["paint"]})}catch(v){}u=new PerformanceObserver(i);try{u.observe({entryTypes:["largest-contentful-paint"]})}catch(v){}s=new PerformanceObserver(o);try{s.observe({type:"layout-shift",buffered:!0})}catch(v){}}if("addEventListener"in document){var g=!1,w=["click","keydown","mousedown","pointerdown","touchstart"];w.forEach(function(e){document.addEventListener(e,a,!1)})}l(c)}},{}],5:[function(e,t,n){function r(e,t){if(!i)return!1;if(e!==i)return!1;if(!t)return!0;if(!o)return!1;for(var n=o.split("."),r=t.split("."),a=0;a<r.length;a++)if(r[a]!==n[a])return!1;return!0}var i=null,o=null,a=/Version\/(\S+)\s+Safari/;if(navigator.userAgent){var c=navigator.userAgent,f=c.match(a);f&&c.indexOf("Chrome")===-1&&c.indexOf("Chromium")===-1&&(i="Safari",o=f[1])}t.exports={agent:i,version:o,match:r}},{}],6:[function(e,t,n){function r(e){function t(){e(a&&document[a]?document[a]:document[i]?"hidden":"visible")}"addEventListener"in document&&o&&document.addEventListener(o,t,!1)}t.exports=r;var i,o,a;"undefined"!=typeof document.hidden?(i="hidden",o="visibilitychange",a="visibilityState"):"undefined"!=typeof document.msHidden?(i="msHidden",o="msvisibilitychange"):"undefined"!=typeof document.webkitHidden&&(i="webkitHidden",o="webkitvisibilitychange",a="webkitVisibilityState")},{}],7:[function(e,t,n){function r(e,t){var n=[],r="",o=0;for(r in e)i.call(e,r)&&(n[o]=t(r,e[r]),o+=1);return n}var i=Object.prototype.hasOwnProperty;t.exports=r},{}],8:[function(e,t,n){function r(e,t,n){t||(t=0),"undefined"==typeof n&&(n=e?e.length:0);for(var r=-1,i=n-t||0,o=Array(i<0?0:i);++r<i;)o[r]=e[t+r];return o}t.exports=r},{}],9:[function(e,t,n){t.exports={exists:"undefined"!=typeof window.performance&&window.performance.timing&&"undefined"!=typeof window.performance.timing.navigationStart}},{}],ee:[function(e,t,n){function r(){}function i(e){function t(e){return e&&e instanceof r?e:e?u(e,f,a):a()}function n(n,r,i,o,a){if(a!==!1&&(a=!0),!l.aborted||o){e&&a&&e(n,r,i);for(var c=t(i),f=v(n),u=f.length,s=0;s<u;s++)f[s].apply(c,r);var p=d[h[n]];return p&&p.push([b,n,r,c]),c}}function o(e,t){y[e]=v(e).concat(t)}function m(e,t){var n=y[e];if(n)for(var r=0;r<n.length;r++)n[r]===t&&n.splice(r,1)}function v(e){return y[e]||[]}function g(e){return p[e]=p[e]||i(n)}function w(e,t){s(e,function(e,n){t=t||"feature",h[n]=t,t in d||(d[t]=[])})}var y={},h={},b={on:o,addEventListener:o,removeEventListener:m,emit:n,get:g,listeners:v,context:t,buffer:w,abort:c,aborted:!1};return b}function o(e){return u(e,f,a)}function a(){return new r}function c(){(d.api||d.feature)&&(l.aborted=!0,d=l.backlog={})}var f="nr@context",u=e("gos"),s=e(7),d={},p={},l=t.exports=i();t.exports.getOrSetContext=o,l.backlog=d},{}],gos:[function(e,t,n){function r(e,t,n){if(i.call(e,t))return e[t];var r=n();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(e,t,{value:r,writable:!0,enumerable:!1}),r}catch(o){}return e[t]=r,r}var i=Object.prototype.hasOwnProperty;t.exports=r},{}],handle:[function(e,t,n){function r(e,t,n,r){i.buffer([e],r),i.emit(e,t,n)}var i=e("ee").get("handle");t.exports=r,r.ee=i},{}],id:[function(e,t,n){function r(e){var t=typeof e;return!e||"object"!==t&&"function"!==t?-1:e===window?0:a(e,o,function(){return i++})}var i=1,o="nr@id",a=e("gos");t.exports=r},{}],loader:[function(e,t,n){function r(){if(!E++){var e=x.info=NREUM.info,t=l.getElementsByTagName("script")[0];if(setTimeout(u.abort,3e4),!(e&&e.licenseKey&&e.applicationID&&t))return u.abort();f(h,function(t,n){e[t]||(e[t]=n)});var n=a();c("mark",["onload",n+x.offset],null,"api"),c("timing",["load",n]);var r=l.createElement("script");r.src="https://"+e.agent,t.parentNode.insertBefore(r,t)}}function i(){"complete"===l.readyState&&o()}function o(){c("mark",["domContent",a()+x.offset],null,"api")}var a=e(2),c=e("handle"),f=e(7),u=e("ee"),s=e(5),d=e(3),p=window,l=p.document,m="addEventListener",v="attachEvent",g=p.XMLHttpRequest,w=g&&g.prototype;if(d(p.location)){NREUM.o={ST:setTimeout,SI:p.setImmediate,CT:clearTimeout,XHR:g,REQ:p.Request,EV:p.Event,PR:p.Promise,MO:p.MutationObserver};var y=""+location,h={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net",agent:"js-agent.newrelic.com/nr-1208.min.js"},b=g&&w&&w[m]&&!/CriOS/.test(navigator.userAgent),x=t.exports={offset:a.getLastTimestamp(),now:a,origin:y,features:{},xhrWrappable:b,userAgent:s};e(1),e(4),l[m]?(l[m]("DOMContentLoaded",o,!1),p[m]("load",r,!1)):(l[v]("onreadystatechange",i),p[v]("onload",r)),c("mark",["firstbyte",a.getLastTimestamp()],null,"api");var E=0}},{}],"wrap-function":[function(e,t,n){function r(e,t){function n(t,n,r,f,u){function nrWrapper(){var o,a,s,p;try{a=this,o=d(arguments),s="function"==typeof r?r(o,a):r||{}}catch(l){i([l,"",[o,a,f],s],e)}c(n+"start",[o,a,f],s,u);try{return p=t.apply(a,o)}catch(m){throw c(n+"err",[o,a,m],s,u),m}finally{c(n+"end",[o,a,p],s,u)}}return a(t)?t:(n||(n=""),nrWrapper[p]=t,o(t,nrWrapper,e),nrWrapper)}function r(e,t,r,i,o){r||(r="");var c,f,u,s="-"===r.charAt(0);for(u=0;u<t.length;u++)f=t[u],c=e[f],a(c)||(e[f]=n(c,s?f+r:r,i,f,o))}function c(n,r,o,a){if(!m||t){var c=m;m=!0;try{e.emit(n,r,o,t,a)}catch(f){i([f,n,r,o],e)}m=c}}return e||(e=s),n.inPlace=r,n.flag=p,n}function i(e,t){t||(t=s);try{t.emit("internal-error",e)}catch(n){}}function o(e,t,n){if(Object.defineProperty&&Object.keys)try{var r=Object.keys(e);return r.forEach(function(n){Object.defineProperty(t,n,{get:function(){return e[n]},set:function(t){return e[n]=t,t}})}),t}catch(o){i([o],n)}for(var a in e)l.call(e,a)&&(t[a]=e[a]);return t}function a(e){return!(e&&e instanceof Function&&e.apply&&!e[p])}function c(e,t){var n=t(e);return n[p]=e,o(e,n,s),n}function f(e,t,n){var r=e[t];e[t]=c(r,n)}function u(){for(var e=arguments.length,t=new Array(e),n=0;n<e;++n)t[n]=arguments[n];return t}var s=e("ee"),d=e(8),p="nr@original",l=Object.prototype.hasOwnProperty,m=!1;t.exports=r,t.exports.wrapFunction=c,t.exports.wrapInPlace=f,t.exports.argsToArray=u},{}]},{},["loader"]);</script>
  <script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
  <script type="text/javascript" src="//thingspeak.com/highcharts-3.0.8.js"></script>
  <script src="/assets/application-e457bbf6a86124b0fc75d277cda64b0e85d6f59c4aaf9e70cadc9a9509387d59.js"></script>
    <script type="text/javascript">
    // user's timezone offset
    var myOffset = new Date().getTimezoneOffset();

    // converts date format from JSON
    function getChartDate(d) {
      // offset in minutes is converted to milliseconds and subtracted so that chart's x-axis is correct
      return Date.parse(d) - (myOffset * 60000);
    }

    $(document).on('page:load ready', function() {
      // blank array for holding chart data
      var chartData = [];
      // variable for the local date in milliseconds
      var localDate;
      // variable for the last date added to the chart
      var last_date;
      // get the data with a webservice call
      $.getJSON('https://thingspeak.com/channels/1370705/field/1.json?&amp;offset=0&amp;results=60', function(data) {

          // if no access
          if (data == '-1') {
            $('#chart-container').append('This channel is not public.  To embed charts, the channel must be public or a read key must be specified.');
          }

          // iterate through each feed
          $.each(data.feeds, function() {
            var p = new Highcharts.Point();
            // set the proper values
            var v = this.field1;
            p.x = getChartDate(this.created_at);
            p.y = parseFloat(v);
            // add location if possible
            if (this.location) {
              p.name = this.location;
            }
            // if a numerical value exists add it
            if (!isNaN(parseInt(v))
                            ) {
              chartData.push(p);
            }
          });

          // specify the chart options
          var chartOptions = {
            chart: {
              renderTo: 'chart-container',
              defaultSeriesType: "line",
              backgroundColor: '#ffffff',
              events: {
                load: function() {
                  //if dynamic and no "timeslice" options are set
                  //   GAK 02/16/2013 Let's try to add the last "average" slice if @chart_attr[:average]

                  var url = 'https://thingspeak.com/channels/1370705/feed/last.json?&amp;offset=0&amp;location=true&amp;results=60';
                  if ("".length > 0) {
                    url = 'https://thingspeak.com/channels/1370705/feed/last_average.json?&amp;offset=0&amp;location=true&amp;average=&amp;results=60';
                  } else if ("".length > 0) {
                    url = 'https://thingspeak.com/channels/1370705/feed/last_median.json?&amp;offset=0&amp;location=true&amp;median=&amp;results=60';
                  } else if ("".length > 0) {
                    url = 'https://thingspeak.com/channels/1370705/feed/last_sum.json?&amp;offset=0&amp;location=true&amp;sum=&amp;results=60';
                  }

                  if ('true' === 'true' && (''.length < 1)) {
                    // push data every 15 seconds
                    setInterval(function() {
                      // get the data with a webservice call if we're just getting the last channel
                      $.getJSON(url, function(data) {
                        // if data exists
                        if (data && data.field1) {

                          var p = new Highcharts.Point();
                          // set the proper values
                          var v = data.field1;

                          p.x = getChartDate(data.created_at);
                          p.y = parseFloat(v);
                          // add location if possible
                          if (data.location) {
                            p.name = data.location;
                          }
                          // get the last date if possible
                          if (dynamicChart.series[0].data.length > 0) {
                            last_date = dynamicChart.series[0].data[dynamicChart.series[0].data.length - 1].x;
                          }
                          var shift = false; //default for shift

                          //if push is requested in parameters
                          // then if results is and data.length is < results, shift = false
                          var results = 60;
                          if (results && dynamicChart.series[0].data.length + 1 >= results) {
                            shift = true;
                          }
                          // if a numerical value exists and it is a new date, add it
                          if (!isNaN(parseInt(v)) && (p.x != last_date)
                                                        ) {
                            dynamicChart.series[0].addPoint(p, true, shift);
                          } else {
                            dynamicChart.series[0].data[dynamicChart.series[0].data.length - 1].update(p);
                          }
                        }
                      });

                    }, 15000);
                  }
                }
              }
            },
            title: {
              text: ''
            },
            plotOptions: {
              line: {
                color: '#d62020'
              },
              bar: {
                color: '#d62020'
              },
              column: {
                color: '#d62020'
              },
              spline: {
                color: '#d62020'
              },
              series: {
                marker: {
                  radius: 3
                },
                animation: true,
                step: false,
                borderWidth: 0,
                turboThreshold: 0
              }
            },
            tooltip: {
              // reformat the tooltips so that local times are displayed
              formatter: function() {
                var d = new Date(this.x + (myOffset * 60000));
                var n = (this.point.name === undefined) ? '' : '<br/>' + this.point.name;
                return this.series.name + ':<b>' + this.y + '</b>' + n + '<br/>' + d.toDateString() + '<br/>' + d.toTimeString().replace(/\(.*\)/, "");
              }
            },
            xAxis: {
              type: 'datetime',
              title: {
                text: 'test'
              }
            },
            yAxis: {
              title: {
                text: ''
              },
              min: null ,
              max: null,
              startOnTick: false,
              endOnTick: false
            },
            legend: {
              enabled: false
            },
            series: [{
              name: data.channel.field1
            }],
            credits: {
              text: 'ThingSpeak.com',
              href: 'https://thingspeak.com/',
              style: {
                color: '#D62020'
              }
            }
          };

          // add the data to the chart
          chartOptions.series[0].data = chartData;

          // set chart labels here so that decoding occurs properly
          chartOptions.title.text = data.channel.name;
          chartOptions.xAxis.title.text = 'Date';
          chartOptions.yAxis.title.text = data.channel.field1;

          // draw the chart
          var dynamicChart = new Highcharts.Chart(chartOptions);

          // end getJSON success
        })
        // chained to getjson, on error
        .fail(function() {
          $('#chart-container').html('Invalid Chart options');
        });

    }); // end document.ready
    </script>
</head>

<body style='background-color: #ffffff; height: 100%; margin: 0; padding: 0;'>
  <div id="chart-container" style="width: 425px; height: 225px; display: block; position:absolute; bottom:0; top:0; left:0; right:0; margin: 5px 15px 15px 0; overflow: hidden;">
    <img style="position: absolute; margin: auto; top: 0; left: 0; right: 0; bottom: 0;" src="/assets/loader-transparent-10d4bf629c8a97ca233fc8342ef4d5e547b22b8b99c4071b0651b77d5b326637.gif" />
  </div>
</body>

</html>
