# MIXING For SASS 
Author: Sumit Kumar Tiwari
        Web Developer

#### Download mixin file _mixin.scss and import in your main scss file and use

### Media Mixing
 eg. @include tab() {
   width: 100%;
 } 

## list of media
  1. @include large-desktop() { ... }
  2. @include desktop() { ... }
  3. @include mini-desktop() { ... }
  4. @include mini-tab() { ... }
  5. @include mini-mobile() { ... }


### Box Mixings
@mixin box($display, $width: null, $height: null, $background: null) {
  display: $display;
  width: $width;
  height: $height;
  background: $background;
}

#### use
@include box(block, $width: 100%, $height: auto, $background: red);


###Margin And Padding Mixing
 
 #### use
 @include margin(20px....);

 @include padding(20px....);


###Border Mixin

 ####use
 @include border(1px solid red); 


###Position mixing

	###use 
	@include position(position, $top: 10px, $right: 20px, $bottom: 10px, $left: 20px);

	@include position(position, $top: 10px, $right: 20px);


##Linking mixing

	###use
	@include link($link, $visit, $hover, $active);

  use color place of argument and it will work for anchor

##Grid mixing

	###Use
	simply use number of grid and pass it as argument

	include grid(number_of_grid);


##video responsive 

	@mixin video_parent() {
	  position: relative;
	  padding-bottom: 56.25%;
	  height: 0;
	}

	@mixin video_frame() {
		  position: absolute;
	    top: 0;
	    left: 0;
	    width: 100%;
	    height: 100%;
	}	  

	###use
	1. Use this mixing for parent of iframe
	 @include video_parent();

  	1. Use this mixing for iframe
	 @include video_frame();	 


##background
	@mixin background($imgpath,$position:0 0,$repeat: no-repeat) {
	    background: {
	        image: url($imgpath);
	        position: $position;
	        repeat: $repeat;
	    }
	}	 

  ###Use

  Just pass argument
  eg: 

  @include background(path, $position: 100% 100%);


##Animation Mixin
@mixin animation($animation_name, $animation_duration: null, $animation_delay: null, $animation_iteration_count: null);

	###Use 
	@include animation(slide, $animation_duration: 2s, $animation_delay: 1s, $animation_iteration_count: 4);



##Will update more mixin

#Thank you	

  


