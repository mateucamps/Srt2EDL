# Srt2EDL
Finds specific strings in subtitle files (SRT) and exports them into an EDL file.

This program made in C++ goes through a SRT file and looks for specified text strings. Then, these are exported
into an EDL file (plain text) for later editing in Adobe Premiere (tested, working), Final Cut (not tested) or
Sony Vegas (it crashes when parsing standard EDL files).

In the included example ('sample' folder) we use a subtitle file from the TV series 'Sillicon Valley', where we
want to extract every line which has the word 'F**k' (a very common word in the series). So we need to:

  1. Place the SRT file in the same folder as the binary file (usually 'bin/Release' or 'bin/Debug').
  2. Note down the SRT filename.
  3. Look up the framerate of the associated video file and note it down.
  4. Make a list of words to find. The search is case sensitive, so make case combinations like 'word', 'WORD', 'Word'.

Once you've done the above steps, run the executable 'srt2edl.exe' and follow the on-screen instructions.

> Project made with Code::Blocks 15.12, compiled using GCC 4.9.2 (32bit) under Windows 10