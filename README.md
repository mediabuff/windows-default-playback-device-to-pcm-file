# Windows default playback device to pcm file
Writes any and all audio coming to the currently selected Windows default audio _playback_ device to a file in 16 bit 44.1khz stereo PCM

A blog post with some extra insight: http://rabid.prototyping.xyz/2015/12/29/programmatically-capture-whats-playing-on-windows/

The example audio sink is set up to write any and all audio coming to the currently selected Windows default audio _playback_ device to a file in 16 bit 44.1khz stereo PCM

Which means it can be used to record any audio that is currently playing.

- AudioListener is a cleaned up version of https://msdn.microsoft.com/en-us/library/windows/desktop/dd370800(v=vs.85).aspx
- Only works on Windows (obviously)
- Only tested once on my computer.
- Made in C++ using WASAPI
- Mostly for my personal use in live audio visualization
- Writes to a while named test.pcm
