# pdkvabs - released under gpl v3.0
vanilla abstractions

- dkaccum - running sum
- dkasyncgrn~ - asynchronous granular synth
- dkautowah~ - automatic wah based on envelope following
- dkbangsync - bang syncer
- dkbinlist - int to binary list
- dkbitred~ - audio-signal bit-reduction based off 3.Bit-Reduction by Alexander Torres Porres.
- dkbitcrush~ - bit-resolution/sample-rate reducer
- dkblkmn~ - generates blackman window according to input from 0 to 1. 
- dkbpm2ms - bpm to ms
- dkcdiv~ - division of two complex signals.
- dkcliktrak~ - click track/metronome
- dkcmult~ - multiplication of two complex signals. 
- dkcnorm~ - normalization of a complex. 
- dkdecrease - detect decreases 
- dkdistort~ - audio-signal distortion based off the work of Landon. Requires zexy.
- dkdownsamp~ - audio-signal downsampler.
- dkeqtemp - degree to equal temperament in Hz
- dkfbdel~ - simple delay with fb
- dkfbvdel~ - simple delay with fb (signal delay time)
- dkfft/fftbinwipe~ - fft bin wiper ported from SuperCollider's PV_BinWipe
- dkfft/fftcomp~ - spectral compressor based on 5.Spectral-Compressor by Alexander Torres Porres.
- dkfft/fftconvolve~ - fft convolver
- dkfft/fftcross~ - spectral cross-synthesis based on 1.Cross-Synthesis by Alexander Torres Porres.
- dkfft/fftgain~ - spectral filter with traceable gain. 
- dkfft/fftgate~ - spectral gate (requires zexy). 
- dkfor - for loop
- dkfreqshift~ - frequency shifter via single sideband modulation
- dkgainenv~ - traceable gain envelope
- dkincrease - detect increases 
- dkincwr~ - incremental tabwriter
- dkint~ - "typecast" signals to integer
- dkincwritepos~ - incremental tabwrite~ with sample position table
- dkkarplus~ - karplus-strong synth
- dkkeysend - send globally via prefixed key
- dkkeyrow2num - maps the key row to floats
- dkloopplay~ - synced looper based around tabplay~
- dkloopwin~ - signal-driven loop windowing
- dkmbang - bang multiplier
- dkmidirt - abstraction to handle midi real-time messages
- dkms2smp - ms to samples
- dknearpow2 - rounds input to a power of 2
- dknobu~ - sample chopper abstraction
- dknot - control-rate bitwise not
- dkoneShotM - a one-shot sample player, left inlet takes a bang to trigger playback, right inlet takes a path for file. 
- dkoneShotS - stereo version 
- dkpaulstretch~ - slightly modified/cleaned up martin brinkmann's (mmb) small_paul1 paulstretcher for use as an abstraction. Unlike small_paul1, it rounds window sizes to the nearest power of 2 and accept signals as position input.
- dkpshift~ - rotating tape head pitchshifter
- dkphasevoc~ - a phase vocoder abstraction lifted from Miller Puckette's I07.phase.vocoder from the help files. Like tabread4~, hot signal inlet indexes by sample. First arg is array name, second is window size.
- dkphsrd~ - phasor sound reader abstraction
- dkpolargraph~ - graph a real fft analysis in polar coords
- dkpolyish1 - polyish abs with no note off
- dkpulsewidth~ - pulse width modulation
- dkrandi - random int within a given range
- dkrandom~ - abstraction simulating the output of the Max/MSP rand~ object.
- dkrunmax - running maximum
- dkrunmin - running minimum
- dkscaledeg_van - borrowed from SuperCollider's Scale object. Maps scale degrees to midi notes. Arguments are scale and starting midi note. Vanilla version of my scaledeg external using tables
- dkselector - a row of 32 toggle boxes whose values are stored in an array (name passed by argument, requires cyclone) 
- dkseqgen1 - timed random sequence generator
- dksisascl~ - SIne SAmple SCaLer
- dksmp2ms - samples to ms
- dkstrippoly - a poly without noteoff messages (or zero velocity notes) 
- dkstutter~ - a delay-based stutter effect
- dksyncloop - a synchronized looper. 
- dkswing - bang swinger
- dksyncb - synchronized banger
- dksyncf - synchronized floats
- dktport - a fancy counter with beats, subdivisions, and measures. 
- dktri~ - nonbandlimited triangle oscillator based off Miller Puckette's  J05.triangle
- dkoutput~ - output abstraction
- dkunit2ms - ms calculator
- dkvancomp~ - vanilla compressor/limiter
- dkvandrk - vanilla drunk random number generator 
- dkvanphs~ - vanilla 3-delay line phaser/chorus effect 
- dkvavg - vanilla float averager
- dkvgcld~ - vanille grain cloud
- dkvisclock - visual clock
- dkvuzi - vanilla uzi/multiple banger
- dkvadsr~ - adsr envelope generator using vline~ based off Matt Davey's  diy-adsr~
- dkxor - control-rate bitwise xor

CONVENIENCE
- dkezadc~ - adc abstraction
- dkezdac~ - dac abstraction

COUNTER
- dktimedctr- on bang, output floats counting up to x 
- dkvanctr - vanilla counter (can go both up and down)

DELAY-BASED
- dkchorus~ - chorus
- dkflanger~ - flanger
- dkphaser~ - phaser

GATE
- dklegt - let through floats lesser or equal to x
- dkgegt - let through floats greater or equal to x
- dkrgate - let through anything x% of the time
- dknzgt - only let nonzero floats through

GRANULAR
- dklgstr1~ - live granular stretcher (uses dksyncgrn~)
- dksyncgrn~ - synchronous granular abstraction
- dkloopgrn~ - granular synchronized looper based on dksyncgrn~

FFT
- dkfftgraph~ - graph fft magnitude of incoming signal

FILTERS
- dkvapcomb~ - allpass filter from two combs
- dkvfbcomb~ - feedback comb filter

FLOAT
- dkfround - round float
- dkfdec - get decimal part of float
- dkfdectol - pass float if within decimal tolerance of int

REVERB
- dkschroeder1~ - a schroeder reverb (1-in,4-out)
- dkschroeder2~ - satrev chowning schroeder reverb (1-in, 2-out)

PANNING
- dkcomppan~ - -4.5 dB panner (compromise panner)
- dkcospan~ - cosine-based equal-power panner
- dklinpan~ - linear panner
- dkstpan~ - stereo-to-stereo panning 

VANILLA SIGNAL BINOPS
- dkeq~ - equal to
- dkge~ - greater than or equal to
- dkgt~ - greater than
- dkle~ - less than or equal to
- dklt~ - less than
- dkne~ - not equal to

STRUCTURE
- pdkst-init - clear scalars and init iterating over given element
- pdkst-nth - get nth scalar of a structure 
- pdkst-textdefine - emulate [text define] methods for text struct member

TEXT
- pdktext-getval - get value from associated key (treating text like a hash table)

WINDOWING
- dkhamm~ - generates hamming window according to input 0 to 1. 
- dkhann~ - generates hann window according to input 0 to 1
- dkhannmaker - constructs hann window. args are array name where window is stored, window size, and overlap.
- dkhannnorm~ - normalizes an incoming signal according to hann window (usu. after an ifft~). args are window size and overlap.
- dktukeymaker - tukey window constructor. ideal for grain envelopes. 

MISC
- dklogidy - abstraction to deal with default settings of logidy umi3

NOT-VANILLA ABSTRACTIONS
- dkamixer~ - abstraction over ggee/shell to set volume with amixer (Linux only)
