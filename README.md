# SSW-Funding-Sankey

  <html>
    <head>
      <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
      <script type="text/javascript">
        google.charts.load('current', {'packages':['sankey']});
        google.charts.setOnLoadCallback(drawChart);

      function drawChart() {
        var data = new google.visualization.DataTable();
        data.addColumn('string', 'From');
        data.addColumn('string', 'To');
        data.addColumn('number', 'Weight');
        data.addRows([
          ['IDHS',	'Community Assistance Programs',	1400000],
          ['IDHS',	'Habilitative Systems Inc',	3267500],
          ['IDHS',	'Illinois Action for Children',	1108050],
          ['IDHS',	'Illinois Coalition For Immigrant and Refugee Rights',	2433500],
          ['IDHS',	'Pilsen Wellness Center',	148500],
          ['IDHS',	'Puerto Rican Cultural Center',	301000],
          ['IDHS',	'Rincon Family Services',	1400000],
          ['IDHS',	'University of Illinois at Chicago',	248500],
          ['IDHS',	'YWCA of Metropolitan Chicago',	1310000],
          ['Community Assistance Programs',	'CAP Internal Spending',	322000],
          ['Habilitative Systems Inc',	'HIS Internal Spending',	751525],
          ['Illinois Action for Children',	'IAC Internal Spending',	542944.5],
          ['Illinois Coalition For Immigrant and Refugee Rights',	'ICIRR Internal Spending',	778720],
          ['Pilsen Wellness Center',	'PWC Internal Spending',	75735],
          ['Puerto Rican Cultural Center',	'PRCC Internal Spending',	150500],
          ['Rincon Family Services',	'RFS Internal Spending',	630000],
          ['University of Illinois at Chicago',	'UIC Internal Spending',	248500],
          ['YWCA of Metropolitan Chicago',	'YWCA  Internal Spending',	524000],
          ['Community Assistance Programs',	'34 Partner Orgs',	1078000],
          ['Habilitative Systems Inc',	'29 Partner Orgs',	2515975],
          ['Illinois Action for Children',	'6 Partner Orgs',	565105.5],
          ['Illinois Coalition For Immigrant and Refugee Rights',	'63 Partner Orgs',	1654780],
          ['Pilsen Wellness Center',	'1 Partner Org',	72765],
          ['Puerto Rican Cultural Center',	'5 Partner Orgs',	150500],
          ['Rincon Family Services',	'12 Partner Orgs',	770000],
          ['YWCA of Metropolitan Chicago',	'13 Partner Orgs',	786000]
        ]);

        // Sets chart options.
        var options = {
          width: 600,
        };

        // Instantiates and draws our chart, passing in some options.
        var chart = new google.visualization.Sankey(document.getElementById('sankey_basic'));
        chart.draw(data, options);
      }
    </script>
  </head>
  <body>
    <div id="sankey_basic" style="width: 900px; height: 300px;"></div>
  </body>
</html>
