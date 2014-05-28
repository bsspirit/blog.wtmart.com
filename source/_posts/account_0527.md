title: 每日账户变动（20140527）
date: 2014-05-27 22:20:22 
author: Yishuo Deng
categories:
- 账户变动
---

### 1. 资产表变化明细


<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <title>TableID25d4b50f4e3</title>
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
<!-- Tue May 27 22:05:56 2014 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID25d4b50f4e3 () {
  var data = new google.visualization.DataTable();
  var datajson =
[
 [
 "11",
88996.8,
292158,
203161.2 
],
[
 "27",
202000,
0,
0 
],
[
 "8",
22980,
19670,
-3310 
],
[
 "Fund_fee_payable",
2512.78,
2541.47,
28.69 
],
[
 "cash",
211843,
211843,
0 
],
[
 "interest_rec",
19,
0,
0 
],
[
 "portfolio.net",
523326,
521130,
-2196 
],
[
 "total.asset",
525839,
523671,
-2168 
],
[
 "total.liabilities",
2512.78,
2541.47,
28.69 
] 
];
data.addColumn('string','asset');
data.addColumn('number','money_20140526');
data.addColumn('number','money_20140527');
data.addColumn('number','money_diff');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID25d4b50f4e3() {
  var data = gvisDataTableID25d4b50f4e3();
  var options = {};
options["allowHtml"] = true;

     var chart = new google.visualization.Table(
       document.getElementById('TableID25d4b50f4e3')
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
  callbacks.push(drawChartTableID25d4b50f4e3);
})();
function displayChartTableID25d4b50f4e3() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID25d4b50f4e3"></script>
 
<!-- divChart -->
  
<div id="TableID25d4b50f4e3"
  style="width: 600px; height: 500px;">
</div>
 <div><span>Data: rec_diff &#8226; Chart ID: <a href="Chart_TableID25d4b50f4e3.html">TableID25d4b50f4e3</a></span><br /> 
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
  <title>TableID25d43371833d</title>
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
<!-- Tue May 27 22:05:56 2014 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID25d43371833d () {
  var data = new google.visualization.DataTable();
  var datajson =
[
 [
 "122105",
"11",
86.238,
70,
0,
89.4,
0,
6258,
0,
-6258 
],
[
 "112121",
"11",
78.181,
70,
0,
87.9,
0,
6153,
0,
-6153 
],
[
 "122133",
"11",
85.266,
70,
0,
85.75,
0,
6002.5,
0,
-6002.5 
],
[
 "112110",
"11",
83.139,
70,
0,
85.59,
0,
5991.3,
0,
-5991.3 
],
[
 "112160",
"11",
83.515,
70,
0,
84.29,
0,
5900.3,
0,
-5900.3 
],
[
 "122162",
"11",
97.758,
60,
0,
98.19,
0,
5891.4,
0,
-5891.4 
],
[
 "122093",
"11",
83.692,
70,
0,
83.63,
0,
5854.1,
0,
-5854.1 
],
[
 "112168",
"11",
86.172,
70,
0,
82.21,
0,
5754.7,
0,
-5754.7 
],
[
 "122267",
"11",
96.333,
60,
0,
94.31,
0,
5658.6,
0,
-5658.6 
],
[
 "122107",
"11",
90.539,
60,
0,
92.2,
0,
5532,
0,
-5532 
],
[
 "112178",
"11",
89.898,
60,
0,
91.325,
0,
5479.5,
0,
-5479.5 
],
[
 "122829",
"11",
92.24,
50,
0,
93.27,
0,
4663.5,
0,
-4663.5 
],
[
 "112155",
"11",
85.431,
50,
0,
85.665,
0,
4283.25,
0,
-4283.25 
],
[
 "124133",
"11",
89.665,
30,
0,
92.18,
0,
2765.4,
0,
-2765.4 
],
[
 "112036",
"11",
93.114,
70,
70,
95.09,
95.11,
6656.3,
6657.7,
1.4 
],
[
 "112073",
"11",
87.082,
70,
70,
87.9,
88.3,
6153,
6181,
28 
],
[
 "112165",
"11",
92.399,
0,
70,
0,
92.51,
0,
6475.7,
6475.7 
],
[
 "122143",
"11",
93.944,
0,
70,
0,
93.88,
0,
6571.6,
6571.6 
],
[
 "122060",
"11",
94.304,
0,
70,
0,
94.28,
0,
6599.6,
6599.6 
],
[
 "122181",
"11",
97.537,
0,
70,
0,
97.55,
0,
6828.5,
6828.5 
],
[
 "122134",
"11",
97.916,
0,
70,
0,
97.95,
0,
6856.5,
6856.5 
],
[
 "122113",
"11",
98.883,
0,
70,
0,
98.88,
0,
6921.6,
6921.6 
],
[
 "122088",
"11",
99.292,
0,
70,
0,
99.33,
0,
6953.1,
6953.1 
],
[
 "112133",
"11",
99.806,
0,
70,
0,
99.834,
0,
6988.38,
6988.38 
],
[
 "112053",
"11",
100.775,
0,
70,
0,
100.845,
0,
7059.15,
7059.15 
],
[
 "112071",
"11",
101.266,
0,
70,
0,
101.26,
0,
7088.2,
7088.2 
],
[
 "112116",
"11",
96.754,
0,
71,
0,
100.12,
0,
7108.52,
7108.52 
],
[
 "112056",
"11",
102.496,
0,
70,
0,
102.545,
0,
7178.15,
7178.15 
],
[
 "112048",
"11",
102.973,
0,
70,
0,
103.04,
0,
7212.8,
7212.8 
],
[
 "112087",
"11",
85.694,
0,
80,
0,
90.192,
0,
7215.36,
7215.36 
],
[
 "112014",
"11",
103.773,
0,
70,
0,
103.778,
0,
7264.46,
7264.46 
],
[
 "112178",
"11",
91.242,
0,
80,
0,
91.128,
0,
7290.24,
7290.24 
],
[
 "112142",
"11",
91.532,
0,
80,
0,
91.44,
0,
7315.2,
7315.2 
],
[
 "122077",
"11",
91.419,
0,
80,
0,
91.46,
0,
7316.8,
7316.8 
],
[
 "122107",
"11",
91.009,
0,
80,
0,
92.18,
0,
7374.4,
7374.4 
],
[
 "122110",
"11",
92.366,
0,
80,
0,
92.5,
0,
7400,
7400 
],
[
 "124133",
"11",
92.558,
0,
80,
0,
92.75,
0,
7420,
7420 
],
[
 "112168",
"11",
82.601,
0,
90,
0,
82.81,
0,
7452.9,
7452.9 
],
[
 "122829",
"11",
92.781,
0,
80,
0,
93.78,
0,
7502.4,
7502.4 
],
[
 "122159",
"11",
94.268,
0,
80,
0,
94.42,
0,
7553.6,
7553.6 
],
[
 "112109",
"11",
94.775,
0,
80,
0,
94.53,
0,
7562.4,
7562.4 
],
[
 "122073",
"11",
94.541,
0,
80,
0,
94.55,
0,
7564,
7564 
],
[
 "122093",
"11",
84.09,
0,
90,
0,
84.13,
0,
7571.7,
7571.7 
],
[
 "122267",
"11",
94.996,
0,
80,
0,
94.81,
0,
7584.8,
7584.8 
],
[
 "122811",
"11",
94.884,
0,
80,
0,
94.94,
0,
7595.2,
7595.2 
],
[
 "112160",
"11",
84.627,
0,
90,
0,
84.66,
0,
7619.4,
7619.4 
],
[
 "112094",
"11",
96.123,
0,
80,
0,
96.14,
0,
7691.2,
7691.2 
],
[
 "112155",
"11",
82.903,
0,
90,
0,
86.159,
0,
7754.31,
7754.31 
],
[
 "122133",
"11",
85.455,
0,
90,
0,
86.18,
0,
7756.2,
7756.2 
],
[
 "112110",
"11",
83.808,
0,
90,
0,
86.242,
0,
7761.78,
7761.78 
],
[
 "122162",
"11",
98.79,
0,
80,
0,
98.67,
0,
7893.6,
7893.6 
],
[
 "112121",
"11",
88.714,
0,
90,
0,
88.75,
0,
7987.5,
7987.5 
],
[
 "112179",
"11",
88.759,
0,
90,
0,
88.824,
0,
7994.16,
7994.16 
],
[
 "122105",
"11",
86.991,
0,
90,
0,
89.29,
0,
8036.1,
8036.1 
],
[
 "131810",
"27",
1,
202000,
0,
1,
0,
202000,
0,
-202000 
],
[
 "tiantianfa",
"8",
1,
3740,
450,
1,
1,
3740,
450,
-3290 
],
[
 "150012",
"8",
0.968,
20000,
20000,
0.962,
0.961,
19240,
19220,
-20 
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
8,
8,
1,
1,
8,
8,
0 
],
[
 "Interest_rec",
"interest_rec",
1,
19,
0,
1,
0,
19,
0,
-19 
] 
];
data.addColumn('string','securityID');
data.addColumn('string','category');
data.addColumn('number','cost_unit');
data.addColumn('number','amount.x');
data.addColumn('number','amount.y');
data.addColumn('number','last_unit_20140526');
data.addColumn('number','last_unit_20140527');
data.addColumn('number','value_20140526');
data.addColumn('number','value_20140527');
data.addColumn('number','value_diff');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID25d43371833d() {
  var data = gvisDataTableID25d43371833d();
  var options = {};
options["allowHtml"] = true;

     var chart = new google.visualization.Table(
       document.getElementById('TableID25d43371833d')
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
  callbacks.push(drawChartTableID25d43371833d);
})();
function displayChartTableID25d43371833d() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID25d43371833d"></script>
 
<!-- divChart -->
  
<div id="TableID25d43371833d"
  style="width: 600px; height: 500px;">
</div>
 <div><span>Data: rec_diff &#8226; Chart ID: <a href="Chart_TableID25d43371833d.html">TableID25d43371833d</a></span><br /> 
<!-- htmlFooter -->
<span> 
R version 3.0.1 (2013-05-16) &#8226; <a href="http://code.google.com/p/google-motion-charts-with-r/">googleVis-0.4.3</a>
&#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; <a href="https://google-developers.appspot.com/chart/interactive/docs/gallery/table.html#Data_Policy">Data Policy</a>
</span></div>
</body>
</html>

