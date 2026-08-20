# How to swap sounds

## Music files
Replace or add `.mp3` or `.wav` files in this directory:
- `music_knights.mp3` - Knights of Cydonia (Muse)
- `music_friends.mp3` - I'll Be There For You (Friends Theme)

Then in `index.html`, find the `CONFIG` object at the top of the `<script>` block and set the paths:
```js
const CONFIG = {
  music: {
    knights: 'sounds/music_knights.mp3',
    friends: 'sounds/music_friends.mp3',
  },
```

## Clap sound
Add a `clap.wav` or `clap.mp3` file here, then set:
```js
  clap: 'sounds/clap.wav',
```

## Note icons
In the `CONFIG` object, change the `noteIcons` array to use different emoji or text:
```js
  noteIcons: ['A', 'B', 'C', 'D', 'E'],
```

## Reset to synthetic audio
Set any path to `null` to fall back to the built-in Web Audio synthesizer:
```js
  music: { knights: null, friends: null },
  clap: null,
```
