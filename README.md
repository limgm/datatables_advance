## datatables_advance

This repo provides an advanced template to create an *interactive* table with the help of [DataTables](https://datatables.net/). 

Click the link for online demo: https://limgm.github.io/datatables_advance/

If you are unfamiliar with html and javascript, refer to the [basic template](https://github.com/limgm/datatables_basic) first.

## Advantages
Main adv of creating an online *interactive* table:
* Share info online
* Enhance user experience
* Version control by github

## Usage
To create the table, the only file needed is [index.html](https://github.com/limgm/datatables_basic/blob/master/index.html), refer to the code for more details.

To view the table online, github.io page is used to host the webpage.

## Features
* Buttons (copy, csv, excel, pdf, print)
* Individual column search
* Search panes
* Column (reordering, visibility)

To add more features, you can refer to [examples in DataTables](https://datatables.net/examples/index) and the procedures are basically:

Other than the three files listed below (jquery-3.3.1.js, jquery.dataTables.css and jquery.dataTables.js), add any additional **Javascript** and **CSS library files** required to run the example.
```
<head>
  <script src="https://code.jquery.com/jquery-3.3.1.js"></script>
  <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.10.20/css/jquery.dataTables.css"/>
  <script src="https://cdn.datatables.net/1.10.20/js/jquery.dataTables.js"></script>  
</head>
```

Modify the things inside
```
<script type="text/javascript">
  $(document).ready(function() {
      $('#example').DataTable();
  });
</script>
```

Then try it out to see if it works, take note that some features cannot coexist (e.g. enabling scrollX/scrollY will have issue with individual column search)

