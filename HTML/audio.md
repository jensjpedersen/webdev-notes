

# HTMl - Audio
* Add audio 
* `controls`  - add controls to audio
```html
<audio src="audio.mp3" controls></audio>
```


# DOM and audio attributes
**Create custom controls in javascript**

* create audio element. 
```javascript
const audoEl = document.createElement("audio")
```

* `audoEl.controls = true` - add controls to audio
* `audoEl.src = "audio.mp3"` - add src to audio
* `audoEl.play()` - play audio
* `audoEl.pause()` - pause audio
* `audoEl.currentTime = 0` - set current time to 0
* `audoEl.volume = 0.5` - set volume to 50%
* `audoEl.muted = true` - mute audio
* `audoEl.loop = true` - loop audio
* `audoEl.autoplay = true` - autoplay audio
* `audoEl.preload = true` - preload audio




