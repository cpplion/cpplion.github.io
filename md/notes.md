### reference
https://developer.chrome.com/docs/chromium/videong

- The goal of any modern video playback engine with efficiency in mind is to minimize bandwidth between the decoder and the final rendering step.
- Keeping everything in one place from decoding all the way to rendering can lead to incredible power efficiency.
- Chromium's playback stack uses **a "pull" based architecture**, meaning each component in the stack requests its inputs from the one below it in hierarchical order.
- At the top of the stack is the rendering of audio and video frames, next lower is decoding, followed by demuxing, and finally I/O.

