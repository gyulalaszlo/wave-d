## What's this?

wave-d is a tiny library to load/save WAV audio files.


## Licenses

See UNLICENSE.txt


## Usage


```d

import std.stdio;
import waved;

void main()
{
    Sound input = decodeWAV("my_wav_file.wav");
    writefln("channels = %s", input.numChannels);
    writefln("samplerate = %s", input.sampleRate);
    writefln("samples = %s", input.data.length);

    input.encodeWAV("copy.wav");
}

```
