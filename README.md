This is a relatively simple image "lightbox" popup implementation, using html, jQuery and css.

How to Use
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
5. Replace the images inside the images folder if you don't want to use the defaults.

