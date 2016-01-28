# pure data abstractions
pure data abstractions 

<b>bangsync.pd</b> - syncs up two bangs. <br>
<b>bitred~.pd</b> - audio-signal bit-reduction based off 3.Bit-Reduction.pd by Alexander Torres Porres. <br>
<b>blkmn~.pd</b> - generates blackman window according to input from 0 to 1. <br>
<b>chorus~.pd</b> - chorus based on the Cycling '74 MSP tutorial.<br>
<b>cdiv~.pd</b> - division of two complex signals. <br>
<b>cospan~.pd</b> - equal-power cosine panner <br>
<b>cmult~.pd</b> - multiplication of two complex signals. <br>
<b>cnorm~.pd</b> - normalization of a complex. <br>
<b>distort~.pd</b> - audio-signal distortion based off the work of LandonPD. Requires zexy.<br>
<b>dkbd~.pd</b> - bass drum synth<br>
<b>dkhh~.pd</b> - hihat synth<br>
<b>dksd~.pd</b> - snare drum synth<br>
<b>downsamp~.pd</b> - audio-signal downsampler.<br>
<b>fbdel~.pd</b> - delay line with feedback<br>
<b>fft/fftbinwipe~.pd</b> - fft bin wiper ported from SuperCollider's PV_BinWipe<br>
<b>fft/fftcomp~.pd</b> - spectral compressor based on 5.Spectral-Compressor by Alexander Torres Porres.<br>
<b>fft/fftconvolve~.pd</b> - fft convolver<br>
<b>fft/fftcross~.pd</b> - spectral cross-synthesis based on 1.Cross-Synthesis by Alexander Torres Porres.<br>
<b>fft/fftgain~.pd</b> - spectral filter with traceable gain. <br>
<b>fft/fftgate~.pd</b> - spectral gate (requires zexy). <br>
<b>fgrain/fgrainstr~.pd</b> - granular stretcher<br>
<b>fgrain/fgrainxfade~.pd</b> - granular stretcher/crossfader<br>
<b>flanger~.pd</b> - flanger based on the Cycling '74 MSP tutorial.<br>
<b>fm1~.pd</b> - single-operator FM synthesis based on Miller Puckette's E09.FM.spectrum.pd with added ability to change harmonic of modulator.<br>
<b>fm2~.pd</b> - two-operator FM synthesis based on Miller Puckette's E10.complex.FM.pd<br>
<b>fm3~.pd</b> - three-operator FM synthesis<br>
<b>fm4~.pd</b> - four-operator FM synthesis<br>
<b>fm5~.pd</b> - five-operator FM synthesis<br>
<b>fm6~.pd</b> - six-operator FM synthesis<br>
<b>freqshift~.pd</b> - frequency shifter via single sideband modulation<br>
<b>gainenv~.pd</b> - traceable gain envelope<br>
<b>hamm~.pd</b> - generates hamming window according to input 0 to 1. <br>
<b>hannmaker.pd</b> - constructs hann window. args are array name where window is stored, window size, and overlap.<br>
<b>hannnorm~.pd</b> - normalizes an incoming signal according to hann window (usu. after an ifft~). args are window size and overlap.<br>
<b>incwrite~.pd</b> - incremental tabwrite~<br>
<b>karplus~.pd</b> - karplus-strong synth<br>
<b>mbang.pd</b> - outputts multiple bangs for each incoming bang according to a given subdivision<br>
<b>nearpow2.pd</b> - rounds input to a power of 2<br>
<b>nobu~.pd</b> - sample chopper with stutter<br>
<b>nobugrain~.pd</b> - sample chopper wit stutter and granular stretching (requires fgrainstr~)<br>
<b>nobupaul~.pd</b> - sample chopper wit stutter and paulstretching (requires paulstretch~)<br>
<b>nobupvoc~.pd</b> - sample chopper wit stutter and phase vocoding (requires phasevoc~)<br>
<b>oneShotM.pd</b> - a one-shot sample player, left inlet takes a bang to trigger playback, right inlet takes a path for file. <br>
<b>oneShotS.pd</b> - stereo version <br>
<b>paulstretch~.pd</b> - slightly modified/cleaned up martin brinkmann's (mmb) small_paul1 paulstretcher for use as an abstraction. Unlike small_paul1, it rounds window sizes to the nearest power of 2 and accept signals as position input.<br>
<b>phasevoc~.pd</b> - a phase vocoder abstraction lifted from Miller Puckette's I07.phase.vocoder.pd from the help files. Like tabread4~, hot signal inlet indexes by sample. First arg is array name, second is window size. <br>
<b>pulsewidth~.pd</b> - pulse width modulation<br>
<b>random~.pd</b> - abstraction simulating the output of the Max/MSP rand~ object.<br>
<b>randgate.pd</b> - randomly-opened spigot. specify percentage of things to let through.<br>
<b>runmax.pd</b> - calculate running maximum<br>
<b>runmin.pd</b> - calculate running minimum<br>
<b>scaledeg.pd</b> - borrowed from SuperCollider's Scale object. Maps scale degrees to midi notes. Arguments are scale and starting midi note. <br>
<b>selector.pd</b> - a row of 32 toggle boxes whose values are stored in an array (name passed by argument, requires cyclone) <br>
<b>stpan~.pd</b> - stereo panning <br>
<b>stutter~.pd </b>- a delay-based stutter effect <br>
<b>syncloop.pd</b> - a synchronized looper. <br>
<b>tport.pd</b> - a fancy counter with beats, subdivisions, and measures. <br>
<b>tri~.pd</b> - nonbandlimited triangle oscillator based off Miller Puckette's  J05.triangle.pd<br>
<b>triggrstr~.pd</b> - triggered granular stretcher (requires fgrainstr~)<br>
<b>tukeymaker.pd</b> - tukey window constructor. ideal for grain envelopes. <br>
<b>vadsr~.pd</b> - adsr envelope generator using vline~ based off Matt Davey's  diy-adsr~.pd<br>
