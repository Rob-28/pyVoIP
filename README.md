# pyVoIP
PyVoIP is a pure python VoIP/SIP/RTP library.  Currently, it supports PCMA, PCMU, and telephone-event.

This library does not depend on a sound library, i.e. you can use any sound library that can handle linear sound data i.e. pyaudio or even wave.  Keep in mind PCMU/PCMA only supports 8000Hz, 1 channel, 8 bit audio.

To use G722 codec, supply write_audio with 16khz 16-bit signed bytes.
```
sox -t raw input.wav -r 16k -e signed -b 16 output.pcm
```

## Getting Started
Simply run `pip install pyVoIP G722`, or if installing from source:

```bash
git clone https://github.com/tayler6000/pyVoIP.git
cd pyVoIP
pip install . G722
```

This is a fork, see: https://github.com/tayler6000/pyVoIP