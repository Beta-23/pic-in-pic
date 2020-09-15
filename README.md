# pic-in-pic
pic-in-pic (PiP) allows you to watch videos in a floating window at any location of choice, so you can keep an eye on what you’re watching while interacting with other sites, or applications

[pic-in-pic]()

## Language

```JavaScript-ES6
async function selectMediaStream () {
	try {
		const mediaStream = await navigator.mediaDevices.getDisplayMedia();
		videoElement.srcObject = mediaStream;
		videoElement.onloadedmetadata = () => {
			videoElement.play();
		};
	} catch (error) {
		// Catch Error Here
		console.log('error in the selectMediaStream method:', error);
	}
}

```

## API
> https://fonts.googleapis.com/css2?family=Barlow:wght@100&display=swap
> https://css-tricks.com/an-introduction-to-the-picture-in-picture-web-api/
> https://developer.mozilla.org/en-US/docs/Web/API/Screen_Capture_API/Using_Screen_Capture