**web2ogg** is a simple transcoder for downloaded video or audio files into Ogg Vorbis with batch mode.
When transcoding is used decoding into a wav-file (decompression) and then encoding into Ogg Vorbis.
Thus, we avoid degradation of quality during transcoding.
This script is very convenient when transcoding downloaded podcasts (spotlight) for later listening in a player or a smartphone.
I hope you will find it useful ))) .

Requirements
-------------

   1. `bash`   ( surprisingly... :) );
   2. `ffmpeg` ( i have 2.8 ).

Examples
---------

   `web2ogg -h` or `web2ogg --help`
   `web2ogg -r 48000 /home/foo/podcasts`
   `web2ogg -c 1 -r 22050 ./`
   `web2ogg .`

Options
--------
   `-r          Set samplerate (default 44100).`
               `Other sampling rates:`
                   `48000, 44100, 32000, 22050, 11025, 8000.`
   `-c          Set channels 1 or 2 (default 2).`
   `-q          Set quality -2...10 (default 8).`
   `-h, --help  For this help.`

The order of the parameters is not important, but the path to the files should be the last argument.
The file path can be a relative or absolute.

Install
--------
   1. `mkdir $HOME/bin` (if not exists).
   2. Copy this script (web2ogg) to `$HOME/bin`.
   3. `cd ~/bin`
   4. `chmod +x web2ogg`

Develop Hennadiy Hudzenko aka mixafree.
november 2017, remixafree@gmail.com
License MIT.