# MIDI on Linux

Interesting older article - [USB MIDI controllers & making music with Ubuntu](https://rafalcieslak.wordpress.com/2012/08/29/usb-midi-controllers-and-making-music-with-ubuntu/) explains some basics.

In essence, ALSA communicats with 100% of USB MIDI controllers. To confirm, run `aconnect -` in the console.

Run `qjackctl` and connect the ports on MIDI devices, from left to right, using the device with the same name. This will make the MIDI-over-USB devices available to Wine and Windows applications installed there.

Use ALSA audio by setting it with `winetricks`. [Source](https://askubuntu.com/questions/77210/how-to-change-the-default-audio-in-wine-to-alsa-only)
