# pureDataAbstractions
pure data abstractions 

bangsync.pd - syncs up two bangs. <br>
phasevoc~.pd - a phase vocoder abstraction lifted from Miller Puckette's I07.phase.vocoder.pd from the help files. Like tabread4~, hot signal inlet indexes by sample. First arg is array name, second is window size. <br>
selector.pd - a row of 32 toggle boxes whose values are stored in an array (name passed by argument, requires cyclone) <br>
stutter~.pd - a delay-based stutter effect <br>
syncloop.pd - a synchronized looper, requires bangsync. <br>
oneShotM.pd - a one-shot sample player, left inlet takes a bang to trigger playback, right inlet takes a path for file. <br>
oneShotS.pd - stereo version <br>
