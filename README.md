# pic-in-pic
pic-in-pic (pip) allows you to watch videos in a floating window at any location on your window, so you can keep an eye on what you’re watching while interacting with other sites, or applications.

[pic-in-pic](https://beta-23.github.io/pic-in-pic/)

## How to use:
1. Refresh page ⌘ r
2. Choose your video page or application
3. Press the share button
4. Press the 'Launch' button

## Language

JavaScript-ES6
```
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
> 1.[Google Fonts](https://fonts.googleapis.com/css2?family=Barlow:wght@100&display=swap)
> 2.[Picture-in-Picture intro](https://css-tricks.com/an-introduction-to-the-picture-in-picture-web-api/)
> 3.[API docs](https://developer.mozilla.org/en-US/docs/Web/API/Screen_Capture_API/Using_Screen_Capture)
