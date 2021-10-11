MOVED to https://git.interhacker.space/sammm/tcview.git

tcview v0.1
By Sam Neurohack

Display Link, OSC, Artnet and Midi timecodes

Listen on all network interfaces and midi interfaces

OSC port : 9001
Artnet port : 6454

Needs timecode, rtmidi, mido


* Link

	- BPM
	- beats

* OSC

	- hour:minutes:seconds:ms (from OSC message received containing /TC like /TC1/time/30 '00:00:02:23')
	- Tested against https://github.com/hautetechnique/OSCTimeCode.git


* Artnet

	- hours:minutes:seconds:frames codetype 
	- OpTimeCode (Film, EBU, DF, SMPTE)
	- Tested against lightingapps.de/software/artnetviewer


* Midi (Clock)

	- BPM computed from received clock messages 
	- MTC (quarterframes). Tested against horae (https://sononum.net/horae) and mtc_generate from https://github.com/jeffmikels/timecode_tools.git


To Run (python 3.8)

python3 tcview.py

