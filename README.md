# Web-Development
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8"/>
	<title>Lakmal Foto</title>
	<link href="css/style.css" rel="stylesheet" type="text/css"/>
	<script type="text/javascript" src="jquery/jquery.min.js"></script>
	<meta name="viewport" content="width=device-width, initial-scale=1">
	
</head>
<body class="body">

	<header>
		<div id="logo">
			<h1>LAKMAL FOTO</h1>
			<p><em>
			Design by Lochana Thenuwara</em></p>
			
			<svg height="150" width="400">
			<defs>
			<linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%" >
				<stop offset="0%"
				style="stop-color:rgb(255,200,0);stop-opacity:1" />
				<stop offset="100%"
				style="stop-color:rgb(255,0,255);stop-opacity:1" />
			</linearGradient>
			</defs>
			<ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
			<text fill="#ffffff" font-size="45" font-family="Lucida Calligraphy" x="35" y="86">LFoto</text>
			</svg>
			
		</div> 
		
		<nav  id="menu">
			<ul>
				<li><a href="index.html" class="current">Home</a></li>
				<li><a href="search.html" >Gallery</a></li>
				<li><a href="#" >AboutUs</a></li>
				<li><div id="backgroundAudio">
					<audio autoplay="" controls="" loop="" preload="">
					<source src="audio/song.mp3" type="audio/mp3" align="right"></source>
					</audio>
				</div>
			</ul>
		</nav>
	</header>
<section class="homepic" >
	<img class="homepic"  width=250% src="images/home_5.jpg" alt="Picture should be here" />
</section>


<script>
	$(function(){
		
		$(".1").mouseover(function(){
			$("img.homepic").attr({src:"images/home_5.jpg"});
			
		});
		$(".2").mouseover(function(){
			$("img.homepic").attr({src:"images/home.jpg"});
			
		});
		$(".3").mouseover(function(){
			$("img.homepic").attr({src:"images/home_2.jpg"});
			
		});
		$(".4").mouseover(function(){
			$("img.homepic").attr({src:"images/home_3.jpg"});
			
		});
	
	   
	});
	

</script>
<script>
$(document).ready(function() {
    function close_accordion_section() {
        $('.accordion .accordion-section-title').removeClass('active');
        $('.accordion .accordion-section-content').slideUp(300).removeClass('open');
    }
 
    $('.accordion-section-title').click(function(e) {

        var currentAttrValue = $(this).attr('href');
 
        if($(e.target).is('.active')) {
            close_accordion_section();
        }else {
            close_accordion_section();

            $(this).addClass('active');

            $('.accordion ' + currentAttrValue).slideDown(300).addClass('open'); 
        }
 
        e.preventDefault();
    });
});
</script>

<aside class="accordion" >
	<h1> Category </h1>
    <div class="accordion-section">
        <a class="accordion-section-title" href="#accordion-1">Wedding</a> 
        <div id="accordion-1" class="accordion-section-content">
            <p>There is several packages available.
				Rs 75000/- : Story Album<br>
				Rs 85000/- : Story Album with Pre Shoot<br>
				Rs 95000/- : Magazine<br>
				Rs 100000/- : Magazine with Pre Shoot
        </div>
    </div>
	
	<div class="accordion-section">
        <a class="accordion-section-title" href="#accordion-2">Nature</a> 
        <div id="accordion-2" class="accordion-section-content">
            <p>There is Nature photography sessions at studio "Lakmal Foto" on every Sunday @8.00 am Onwards....</p>
			<p>Rs 300/- per an Hour!!!</p>
        </div>
    </div>
	
	<div class="accordion-section">
        <a class="accordion-section-title" href="#accordion-3">Life</a> 
        <div id="accordion-3" class="accordion-section-content">
            <p><p>There is Nature photography sessions at studio "Lakmal Foto" on every Saturday @8.00 am Onwards....</p>
			<p>Rs 300/- per an Hour!!!</p></p>
        </div>
    </div>
	<aside >
			<ul class="album">
			<li>
			<img class="1" width="75" height="75" src="images/home_4.jpg"></li>
			<li><img class="2" width="75" height="75" src="images/home_1.jpg"></li>
			<li><img class="3" width="75" height="75" src="images/home_2.jpg"></li>
			<li><img class="4" width="75" height="75" src="images/home_3.jpg"></li>
			</ul>
	</aside>

</aside>
</body>
<footer>
		<section>
			<h3><b>Lakmal Foto</b></h3>
			078-8371711<br><br>
			<address>No:44<br>
			Seenigoda<br>
			Watugedara<br>
			</address>
		</section>
		<section>
			<h3><b>Find Us On</b></h3>
			<ul class="social">
				<li><a href="#"><img src="images/facebook.png"></a></li>
				<li><a href="#"><img src="images/googleplus.png"></a></li>
				<li><a href="#"><img src="images/twitter.png"></a></li>
			</ul>
		</section>
		<aside>
			<h1>Photography is our Passion....</h1>
			<h3>Dream is yours,Our effort is to make that dream a reality</h3>
		</aside>

</footer>
<footer class="second">
		(c)Copyrigth- Lochana Thenuwara 12000817
</footer>


</html>
