# playground

Add ideas, showcases, relevant tutorials here.

How People with Disabilities Use the Web
https://www.w3.org/WAI/people-use-web/

EU study, too detailed
https://cyberpsychology.eu/article/view/6767/6262

Good introductory on what is meant by disability
https://www.youtube.com/watch?v=3f31oufqFSM

Record audio via JS
https://addpipe.com/simple-web-audio-recorder-demo/
https://blog.addpipe.com/using-webaudiorecorder-js-to-record-audio-on-your-website/


# Pieces of code
The following manual interaction demonstrates the various pieces of code needed to support speach recognition from the browser.

1) Activating the mic from the browser, and recording the audio stream
Record audio into waw from the browser
* source code: https://github.com/higuma/web-audio-recorder-js
* demo: https://addpipe.com/simple-web-audio-recorder-demo/

2) Encoding the audio the to goggle supported wav format, and storing it for porocessing
Download to your local computer and name it hackathon.wav (aka push to gcloud application)
hackathon.wav

3) Process the recording via the speach-to-text ML api of google
```
gcloud auth
gcloud ml speech recognize ~/Downloads/hackathon.wav --language-code=en-US --audio-channel-count=2 --separate-channel-recognition
```

