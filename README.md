# pureDataAbstractions
pure data abstractions 

<b>bangsync.pd</b> - syncs up two bangs. <br>
<b>cospan~.pd</b> - equal-power cosine panner <br>
<b>fm1~.pd</b> - single-operator FM synthesis based on Miller Puckette's E09.FM.spectrum.pd with added ability to change harmonic of modulator.<br>
<b>fm2~.pd</b> - two-operator FM synthesis based on Miller Puckette's E10.complex.FM.pd<br>
<b>fm3~.pd</b> - three-operator FM synthesis<br>
<b>fm4~.pd</b> - four-operator FM synthesis<br>
<b>karplus~.pd</b> - karplus-strong synth<br>
<b>nearpow2.pd</b> - rounds input to a power of 2<br>
<b>paulstretch~.pd</b> - slightly modified/cleaned up martin brinkmann's (mmb) small_paul1 paulstretcher for use as an abstraction. Unlike small_paul1, it rounds window sizes to the nearest power of 2 and accept signals as position input.<br>
<b>phasevoc~.pd</b> - a phase vocoder abstraction lifted from Miller Puckette's I07.phase.vocoder.pd from the help files. Like tabread4~, hot signal inlet indexes by sample. First arg is array name, second is window size. <br>
<b>pulsewidth~.pd</b> - pulse width modulation<br>
<b>runmax.pd</b> - calculate running maximum<br>
<b>runmin.pd</b> - calculate running minimum<br>
<b>selector.pd</b> - a row of 32 toggle boxes whose values are stored in an array (name passed by argument, requires cyclone) <br>
<b>stutter~.pd </b>- a delay-based stutter effect <br>
<b>syncloop.pd</b> - a synchronized looper, requires bangsync. <br>
<b>oneShotM.pd</b> - a one-shot sample player, left inlet takes a bang to trigger playback, right inlet takes a path for file. <br>
<b>oneShotS.pd</b> - stereo version <br>
<b>tri~.pd</b> - nonbandlimited triangle oscillator based off Miller Puckette's  J05.triangle.pd<br>
<b>vadsr~.pd</b> - adsr envelope generator using vline~ based off Matt Davey's  diy-adsr~.pd<br>
