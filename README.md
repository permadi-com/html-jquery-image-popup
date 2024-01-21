## Intro
This is a relatively simple image "lightbox" popup implementation, using html, jQuery and css. It's relatively compact and straightforward. Only images are supported out-of-the-box (no text, no slideshow), you're welcome to extend it.

I simply wanted to be able to click on an image and show a popup containing the image. I tried other lightboxes but found them too complex for my need. My requirements were: 
1. The popup should be contained within the browser window. Large image should shright to fit the window while maintaining the aspect-ratio.
2. The popup should be centered, not only horizontally but also vertically.

Requirement 2 is the one that I have most issues with, because the lightboxes that I found weren't centering vertically.

## How to Use
1. Include <b>image-modal.js</b> and <b>image-modal.css</b>. Note: jQuery use is assumed, otherwise you need to include it.
```
<script src="js/image-modal.js"></script>
<link rel="stylesheet" href="css/style.css">
```
3. Add <b>image-popup</b> class to the images that you want the lightbox enabled.
```
<img src="images/300x300.gif" class="image-popup" ></img>
```
3. Add the following html code somewhere on your page (I recommend at the end of the page). This is the placeholder <div> that will render the popup, it is initially invisible.
```
<!-- Popup -->
<div id="image-modal-popup">
	<div id="image-modal-container">
		<div id="image-modal-dialog">
			<img id="image-modal-image" src=""></img>
			<div id="image-modal-loader"></div>
			<div id="image-modal-close-button"></div>
		</div>
	</div>
</div>
```
## Optional
1. Replace the <b>loader.gif</b> and <b>close-button.gif</b> in the <b>images</b> folder if you want to modifi them.
2. Edit <b>css/style.css</b> styling to your liking. 


![alt text](https://permadi.com/temp/0.png)
