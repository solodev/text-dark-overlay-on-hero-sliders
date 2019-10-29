# text-dark-overlay-on-sliders
Ensuring readability is challenging when displaying text over a background image. With a dark overlay behind the text,
you can add contrast and increase readability.

## Tutorial
For detailed instruction's, view Solodev's [How to Add text to your hero sliders with a dark overlay for increased readability](https://www.solodev.com/blog/how-to-add-text-to-your-hero-sliders-with-a-dark-overlay-for-increased-readability.stml) article.

## Demo
  		  
Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/rvmgdtos/1/).

## HTML

The tutorial contains the following basic HTML markup.

```
 <header class="hero-text">
	<div class="hero" data-arrows="true" data-autoplay="true">
	  <!--.hero-slide-->
	  <div class="hero-slide">
         <img alt="Mars Image" class="img-responsive cover" src="https://raw.githubusercontent.com/solodev/text-dark-overlay-on-hero-sliders/master/images/mars-1.jpg">
         <div class="header-content text-white position-absolute col-lg-4">
            <h1 class="mb-4">Be part of the <span class="d-block font-weight-bold">Lunar XPerience</span></h1>  
            <a class="btn btn-primary btn-lg w-max mt-2" href="#" tabindex="0">Tour Our Ships</a>
         </div>
	  </div>
	  <!--.hero-slide-->
	  <div class="hero-slide">
          <img alt="Mars Image" class="img-responsive cover" src="https://raw.githubusercontent.com/solodev/text-dark-overlay-on-hero-sliders/master/images/mars-2.jpg">
          <div class="header-content text-white position-absolute col-lg-4">
                <h1 class="mb-4">LunarXP Voted Best Mars Mission</h1>  
                <p class="font-weight-bold">Inc. magazine today ranked LunarXP as the fastest growing company in the Mars Mission category.</p>
                <a class="btn btn-primary btn-lg w-max mt-2" href="#" tabindex="0">Read More</a>
             </div>
	  </div>
	  <!--.hero-slide-->
	  <div class="hero-slide">
          <img alt="Mars Image" class="img-responsive cover" src="https://raw.githubusercontent.com/solodev/text-dark-overlay-on-hero-sliders/master/images/mars-3.jpg">
          <div class="header-content text-white position-absolute col-lg-4">
                <p class="lead">Our fleet of advanced spacecraft have revolutionized the lunar economy and provided safe travel for thousands of scientists, engineers, technicians, medical staff and civilians. These amazing vessels are also paving the way for reaching Mars in the next decade.</p>  
          </div>
	  </div>
	</div><!--.hero-->
  </header>	
  <script>
	jQuery(document).ready(function ($) {
	  $('.hero').slick({
		dots: false,
		infinite: true,
		speed: 300,
		slidesToShow: 1,
		slidesToScroll: 1,
        autoplay: true,
        draggable: false,
		responsive: [
	    {
		breakpoint: 1024,
		settings: {
		slidesToShow: 1,
		slidesToScroll: 1,
        infinite: true,
		dots: false
		          }
        },
        {
		breakpoint: 768,
		settings: {
        draggable: true,
		          }
		},
		{
		breakpoint: 600,
		settings: {
        slidesToShow: 1,
        draggable: true,
		slidesToScroll: 1
			      }
		},
		{
		breakpoint: 480,
		settings: {
        slidesToShow: 1,
        draggable: true,
		slidesToScroll: 1
		          }
		}
	
			      ]
                  });
        });		
</script>

```

## CSS
All required CSS is contained with style.css

## External Resources
This tutorial includes the following third party resources.

```
<!-- Bootstrap CSS -->
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">
<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/slick-carousel@1.8.1/slick/slick.css" />
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/slick-carousel@1.8.1/slick/slick.min.js"></script>
```
