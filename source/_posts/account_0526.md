title: 每日账户变动（20140526）
date: 2014-05-26 22:20:22 
author: Yishuo Deng
categories:
- 账户变动
---

### 1. 资产表变化明细


<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <title>TableID251c389572dd</title>
  <meta http-equiv="content-type" content="text/html;charset=utf-8" />
  <style type="text/css">
    body {
          color: #444444;
          font-family: Arial,Helvetica,sans-serif;
          font-size: 75%;
    }
    a {
          color: #4D87C7;
          text-decoration: none;
    }
  </style>
</head>
<body>
 <!-- Table generated in R 3.0.1 by googleVis 0.4.3 package -->
<!-- Tue May 27 21:59:18 2014 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID251c389572dd () {
  var data = new google.visualization.DataTable();
  var datajson =
[
 [
 "11",
122180,
88996.8,
-33183.2 
],
[
 "27",
172000,
202000,
30000 
],
[
 "8",
19420,
22980,
3560 
],
[
 "Fund_fee_payable",
2483.97,
2512.78,
28.81 
],
[
 "cash",
211837,
211843,
6 
],
[
 "interest_rec",
17,
19,
2 
],
[
 "portfolio.net",
522970,
523326,
356 
],
[
 "total.asset",
525454,
525839,
385 
],
[
 "total.liabilities",
2483.97,
2512.78,
28.81 
] 
];
data.addColumn('string','asset');
data.addColumn('number','money_20140525');
data.addColumn('number','money_20140526');
data.addColumn('number','money_diff');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID251c389572dd() {
  var data = gvisDataTableID251c389572dd();
  var options = {};
options["allowHtml"] = true;

     var chart = new google.visualization.Table(
       document.getElementById('TableID251c389572dd')
     );
     chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  var chartid = "table";

  // Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
  var i, newPackage = true;
  for (i = 0; newPackage && i < pkgs.length; i++) {
    if (pkgs[i] === chartid)
      newPackage = false;
  }
  if (newPackage)
    pkgs.push(chartid);

  // Add the drawChart function to the global list of callbacks
  callbacks.push(drawChartTableID251c389572dd);
})();
function displayChartTableID251c389572dd() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
    var pkgCount = pkgs.length;
    google.load("visualization", "1", { packages:pkgs, callback: function() {
      if (pkgCount != pkgs.length) {
        // Race condition where another setTimeout call snuck in after us; if
        // that call added a package, we must not shift its callback
        return;
      }
      while (callbacks.length > 0)
        callbacks.shift()();
    } });
  }, 100);
}
 
// jsFooter
 </script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID251c389572dd"></script>
 
<!-- divChart -->
  
<div id="TableID251c389572dd"
  style="width: 600px; height: 500px;">
</div>
 <div><span>Data: rec_diff &#8226; Chart ID: <a href="Chart_TableID251c389572dd.html">TableID251c389572dd</a></span><br /> 
<!-- htmlFooter -->
<span> 
R version 3.0.1 (2013-05-16) &#8226; <a href="http://code.google.com/p/google-motion-charts-with-r/">googleVis-0.4.3</a>
&#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; <a href="https://google-developers.appspot.com/chart/interactive/docs/gallery/table.html#Data_Policy">Data Policy</a>
</span></div>
</body>
</html>



### 2. 持仓变化明细

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <title>TableID251c332f7210</title>
  <meta http-equiv="content-type" content="text/html;charset=utf-8" />
  <style type="text/css">
    body {
          color: #444444;
          font-family: Arial,Helvetica,sans-serif;
          font-size: 75%;
    }
    a {
          color: #4D87C7;
          text-decoration: none;
    }
  </style>
</head>
<body>
 <!-- Table generated in R 3.0.1 by googleVis 0.4.3 package -->
<!-- Tue May 27 21:59:18 2014 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID251c332f7210 () {
  var data = new google.visualization.DataTable();
  var datajson =
[
 [
 "112155",
"11",
82.868,
100,
0,
85.869,
0,
8586.9,
0,
-8586.9 
],
[
 "112179",
"11",
86.424,
70,
0,
88.15,
0,
6170.5,
0,
-6170.5 
],
[
 "112121",
"11",
86.172,
70,
0,
87.443,
0,
6121.01,
0,
-6121.01 
],
[
 "122088",
"11",
98.037,
60,
0,
99.1,
0,
5946,
0,
-5946 
],
[
 "112168",
"11",
78.181,
70,
0,
81.95,
0,
5736.5,
0,
-5736.5 
],
[
 "112094",
"11",
94.233,
60,
0,
95.065,
0,
5703.9,
0,
-5703.9 
],
[
 "112109",
"11",
94.731,
60,
0,
94.95,
0,
5697,
0,
-5697 
],
[
 "112096",
"11",
94.577,
60,
0,
94.79,
0,
5687.4,
0,
-5687.4 
],
[
 "122133",
"11",
85.266,
70,
70,
85.69,
85.75,
5998.3,
6002.5,
4.2 
],
[
 "112160",
"11",
83.515,
70,
70,
84.22,
84.29,
5895.4,
5900.3,
4.9 
],
[
 "122093",
"11",
83.692,
70,
70,
83.52,
83.63,
5846.4,
5854.1,
7.7 
],
[
 "122829",
"11",
92.24,
50,
50,
93.11,
93.27,
4655.5,
4663.5,
8 
],
[
 "112178",
"11",
89.898,
60,
60,
91.168,
91.325,
5470.08,
5479.5,
9.42 
],
[
 "124133",
"11",
89.665,
30,
30,
91.83,
92.18,
2754.9,
2765.4,
10.5 
],
[
 "122162",
"11",
97.758,
60,
60,
97.95,
98.19,
5877,
5891.4,
14.4 
],
[
 "112073",
"11",
87.082,
70,
70,
87.607,
87.9,
6132.49,
6153,
20.51 
],
[
 "112110",
"11",
83.139,
70,
70,
85.239,
85.59,
5966.73,
5991.3,
24.57 
],
[
 "112036",
"11",
93.114,
70,
70,
94.558,
95.09,
6619.06,
6656.3,
37.24 
],
[
 "122107",
"11",
90.539,
60,
60,
91.52,
92.2,
5491.2,
5532,
40.8 
],
[
 "122105",
"11",
86.238,
70,
70,
88.81,
89.4,
6216.7,
6258,
41.3 
],
[
 "122267",
"11",
96.333,
60,
60,
93.45,
94.31,
5607,
5658.6,
51.6 
],
[
 "112155",
"11",
85.431,
0,
50,
0,
85.665,
0,
4283.25,
4283.25 
],
[
 "112168",
"11",
86.172,
0,
70,
0,
82.21,
0,
5754.7,
5754.7 
],
[
 "112121",
"11",
78.181,
0,
70,
0,
87.9,
0,
6153,
6153 
],
[
 "131810",
"27",
1,
172000,
202000,
1,
1,
172000,
202000,
30000 
],
[
 "150012",
"8",
0.968,
20000,
20000,
0.961,
0.962,
19220,
19240,
20 
],
[
 "tiantianfa",
"8",
1,
200,
3740,
1,
1,
200,
3740,
3540 
],
[
 "CASH_FUTURE",
"cash",
1,
211835,
211835,
1,
1,
211835,
211835,
0 
],
[
 "CASH_SEC",
"cash",
1,
2,
8,
1,
1,
2,
8,
6 
],
[
 "Interest_rec",
"interest_rec",
1,
17,
19,
1,
1,
17,
19,
2 
] 
];
data.addColumn('string','securityID');
data.addColumn('string','category');
data.addColumn('number','cost_unit');
data.addColumn('number','amount.x');
data.addColumn('number','amount.y');
data.addColumn('number','last_unit_20140525');
data.addColumn('number','last_unit_20140526');
data.addColumn('number','value_20140525');
data.addColumn('number','value_20140526');
data.addColumn('number','value_diff');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID251c332f7210() {
  var data = gvisDataTableID251c332f7210();
  var options = {};
options["allowHtml"] = true;

     var chart = new google.visualization.Table(
       document.getElementById('TableID251c332f7210')
     );
     chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  var chartid = "table";

  // Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
  var i, newPackage = true;
  for (i = 0; newPackage && i < pkgs.length; i++) {
    if (pkgs[i] === chartid)
      newPackage = false;
  }
  if (newPackage)
    pkgs.push(chartid);

  // Add the drawChart function to the global list of callbacks
  callbacks.push(drawChartTableID251c332f7210);
})();
function displayChartTableID251c332f7210() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
    var pkgCount = pkgs.length;
    google.load("visualization", "1", { packages:pkgs, callback: function() {
      if (pkgCount != pkgs.length) {
        // Race condition where another setTimeout call snuck in after us; if
        // that call added a package, we must not shift its callback
        return;
      }
      while (callbacks.length > 0)
        callbacks.shift()();
    } });
  }, 100);
}
 
// jsFooter
 </script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID251c332f7210"></script>
 
<!-- divChart -->
  
<div id="TableID251c332f7210"
  style="width: 600px; height: 500px;">
</div>
 <div><span>Data: rec_diff &#8226; Chart ID: <a href="Chart_TableID251c332f7210.html">TableID251c332f7210</a></span><br /> 
<!-- htmlFooter -->
<span> 
R version 3.0.1 (2013-05-16) &#8226; <a href="http://code.google.com/p/google-motion-charts-with-r/">googleVis-0.4.3</a>
&#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; <a href="https://google-developers.appspot.com/chart/interactive/docs/gallery/table.html#Data_Policy">Data Policy</a>
</span></div>
</body>
</html>

