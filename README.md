# PictureInPicture_Chrome
Bookmarklet to Enable Picture in Picture (PIP) in Chrome when a video in playing on the page.

Create a new Favorites Choose a Name and add this in the URL field.
By clicking on this favorites, you'll enable PIP mode in CHROME



javascript:if("pictureInPictureEnabled"in document&&"querySelectorAll"in document){(async function(){const a=document.querySelectorAll("video");if(0===a.length)window.alert("Sorry, no videos on the page.");else if(0<a.length){const b=a[0];try{b===document.pictureInPictureElement?await document.exitPictureInPicture():await b.requestPictureInPicture()}catch(a){console.error(a)}}})()}else"pictureInPictureEnabled"in document?document.pictureInPictureEnabled||window.alert("Picture-in-Picture not available."):window.alert("Picture-in-Picture is disabled.");



PIP on desktop:

![image](https://user-images.githubusercontent.com/37984399/115051126-c6c93180-9edc-11eb-8c7f-aec09c5f9fd0.png)
