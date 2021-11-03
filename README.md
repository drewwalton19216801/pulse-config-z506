# pulse-config-z506
PulseAudio configuration for 5.1 channel audio with the Logitech z506 speaker system.

## PipeWire configuration
You can find this same configuration for PipeWire here: [pipewire-config-z506](https://github.com/drewwalton19216801/pipewire-config-z506)

## About
This PulseAudio configuration is specifically tuned for the Logitech z506 in 5.1 channel mode. It incorporates the following settings:
- Stereo to 5.1 channel remixing/upmixing
- LFE crossover at 300Hz to prevent distortion in non-subwoofer speakers
- s24le as default sample format
- speex-float-5 resample method for a good balance between audio quality and resource usage on modern x86-64 systems

## Installation
Simply drop the files in this repo in /etc/pulse and reboot. Make sure ALSA is configured for "6" channel audio using alsamixer.
