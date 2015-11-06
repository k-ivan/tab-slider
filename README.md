#Jquery Simple Slider

##How to use
Include jQuery library in your page:
````html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
````
Include the javascript file in your page:
````html
<script src="./src/slider.js"></script>
````
##Example
HTML layout

By default all images have height=auto(for responsive slider) if necessary can set fixed height
````html
<div class="slider-container">
  <div class="slider">
    <div class="slide">
      <img src="img-1.jpg" alt="">
      <span class="caption"><strong>Lorem ipsum dolor sit amet, consectetur adipisicing elit.<a href="">Далее >></a> </span>
    </div>
    <div class="slide">
      <img src="img-2.jpg" alt="">
      <span class="caption">2 Lorem ipsum dolor sit amet, consectetur adipisicing elit. Culpa, facilis.</span>
    </div>
    <div class="slide">
      <img src="img-3.jpg" alt="">
      <span class="caption">3 Lorem ipsum dolor sit amet, consectetur adipisicing elit. Suscipit, culpa!</span>
    </div>
  </div>
    <a href="" class="switch" id="prev"><span></span></a>
    <a href="" class="switch" id="next"><span></span></a>
</div>
````
Init plugin
````javascript
<script>
	$(".slider-container").sliderUi();
</script>
````
Init with options
````javascript
<script>
	$(".slider-container").sliderUi({
		speed: 700,
		cssEasing: "ease-in-out"
	});
</script>
````
##Options
available options and their default values
````javascript
autoPlay: true,
delay: 3000,
controlShow: true,
arrowsShow: true,
caption: false,
speed: 300,
cssEasing: "ease-out"
````
