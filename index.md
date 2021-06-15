<script
  src="https://code.jquery.com/jquery-3.5.1.min.js"
  integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0="
  crossorigin="anonymous"></script>
 
 

<input type="text" name="vaiz">
<button type="submit">Buga Segurança</button>
 


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
