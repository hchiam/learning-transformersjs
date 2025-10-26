# Learning Transformers.js

Just one of the things I'm learning. <https://github.com/hchiam/learning>

<https://huggingface.co/docs/transformers.js>

<https://github.com/huggingface/transformers>

## Notes on [Transformers.js: State-of-the-art Machine Learning for the web](<https://www.youtube.com/watch?v=n18Lrbo8VU8>] video

- 14:07 for 3-liner code example for speech recognition on the web
<https://youtu.be/n18Lrbo8VU8?&t=847> this example is 40mb then cached

```js
import { pipeline } from 'https://cdn.jsdelivr.net/npm/@xenova/transformers@2.8.0';
const transcriber = await pipeline('automatic-speech-recognition', 'Xenova/whisper-tiny.en');
const output = await transcriber('mlk.wav');
console.log(output);
```

- 14:28 for word level timestamps​ <https://youtu.be/n18Lrbo8VU8?t=862>

```js
// continuing the code above
const outputWithWordLevelTimestamps = await transcriber('mlk.wav', { return_timestamps: 'word' });
console.log(outputWithWordLevelTimestamps);
```
