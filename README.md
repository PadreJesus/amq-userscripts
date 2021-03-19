# AMQ scripts

## `userscripts`

Collection of \*monkey userscripts for Anime Music Quiz

### `amqCoopPaste.user.js`

Kinda defunct now with official teams mode but still gives more XP per right answer if everyone is on their own.
When turned on, automatically pastes your answer into the chat.

Maybe I will eventually add the ability to automatically copy paste someone else's answer from chat into your own box.

### `amqVideoBackground.user.js`

Changes AMQ background to the specified video.

## `encoding`

Scripts to make encoding for AMQ more braindead.

### `amq_encode.sh`

bash script that does 2-pass VP9 encoding with CRF 20 and tries to normalize audio to -17dB. Generates output files named `720.webm`, `480.webm`, and `audio.mp3`.

#### Usage

Same as ffmpeg for input files/timing. Put it in your home directory so you can call it with `~/amq_encode.sh`

```bash
# example usages
~/amq_encode.sh -i INPUTFILE
~/amq_encode.sh -i INPUTFILE -ss START -to END
~/amq_encode.sh -i INPUTFILE -ss START -t SECONDS
```

Windows version coming never cuz batch syntax is awful.
