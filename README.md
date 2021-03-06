# parallaxification
Just another Parallax Library

## Installation
### Dependencies 
Parallaxification uses jQuery, so you'll need to throw that in your header.
```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
``` 

### Usage
#### 1. Add the script to your header

```javascript 
<script type="text/javascript" src="js/parallax.min.js"></script>
```

#### 2. Start Parallaxin' 

The syntax is simple. First we identify the element we want to parallaxify by setting a `class="parallax"`. <br/>
Secondly, we specify the parent container with ``` parallax-parent="#myParent" ```. Parallax will automatically transition you through your starting and ending state over the height of this parent, so choose accordingly. <br/>
Our last step is to provide the starting and ending states of our effect. This is done with `parallax-start="some css properties"` and `parallax-end="some changed css properties"`. 

#### An Example: 
```html 
<div 
	class="parallax" 
	parallax-parent="#section1" 
	parallax-start="opacity: 1; width: 300px" 
	parallax-end="opacity: 0; width: 0px">
```

#### Parallax Background

##### CSS
```css
.par_background {
	background-image: url("http://www.bloglmn.com/wp-content/uploads/Ocean1.jpg");
	background-position: 50% 0%;
	background-size: auto 150%;
}
```

##### HTML
```html 
<section id="one" class="par_background" class="parallax" parallax-parent="#one" parallax-start="background-position: 50% 0%" parallax-end="background-position: 50% -50%"></section>
```

