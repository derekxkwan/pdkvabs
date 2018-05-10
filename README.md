# pdkvabs - released under gpl v3.0
vanilla abstractions

(before use, put subfolder contents besides the util folder into main pdkvabs folder)

(also note that this is for personal use and VERY subject to change/renaming so I suggest this repo mainly for educational use)

## GENERAL
- dkattqpt - record attack locations in a soundfile
- dkautowah~ - automatic wah based on envelope following
- dkbangroute - route bangs with bangs
- dkbitcrush~ - bit-resolution/sample-rate reducer
- dkblkmn~ - generates blackman window according to input from 0 to 1.
- dkchangebang~ - bang when detecting changes in a signal
- dkchoprd~ - triggered chopped array reader (analogue to dksndchop)
- dkcliktrak~ - click track/metronome
- dkcoinflip - output 1 a given pct of the time else 0
- dkdelbank~ - delay bank
- dkdellopbank~ - delay bank with lowpass filtering
- dkdistort~ - distortion waveshaper
- dkdownsamp~ - audio-signal downsampler.
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
- dkincwr~ - incremental tabwriter
- dkint~ - "typecast" signals to integer
- dkincwritepos~ - incremental tabwrite~ with sample position table
- dkkarplus~ - karplus-strong synth
- dkkeysend - send globally via prefixed key
- dkkeytonum - maps keys to numbers sequentially by row
- dklisttoclone - distribute list to clone instances
- dkliverev~ - live reverser
- dklooper~ - looper
- dkloopwin~ - signal-driven loop windowing
- dkmbang - multiple banger
- dkmbang_r - multiple banger (but randomly gated)
- dkmiditonote - midi notes to note names
- dkmidirt - abstraction to handle midi real-time messages
- dknobu~ - sample chopper abstraction
- dknot - control-rate bitwise not
- dknotetomidi - note names (case-insensitive) to midi notes
- dkoneShotM - a one-shot sample player, left inlet takes a bang to trigger playback, right inlet takes a path for file. 
- dkoneShotS - stereo version 
- dkpaulstretch~ - slightly modified/cleaned up martin brinkmann's (mmb) small_paul1 paulstretcher for use as an abstraction. Unlike small_paul1, it rounds window sizes to the nearest power of 2 and accept signals as position input.
- dkpshift~ - rotating tape head pitchshifter
- dkphasevoc~ - a phase vocoder abstraction lifted from Miller Puckette's I07.phase.vocoder from the help files. Like tabread4~, hot signal inlet indexes by sample. First arg is array name, second is window size.
- dkphsrd~ - phasor sound reader abstraction
- dkpolargraph~ - graph a real fft analysis in polar coords
- dkpolyish1 - polyish abs with no note off
- dkpulsewidth~ - pulse width modulation
- dkroute2~ - one to two signal router
- dkselector - a row of 32 toggle boxes whose values are stored in an array (name passed by argument, requires cyclone) 
- dkseqgen1 - timed random sequence generator
- dksisascl~ - SIne SAmple SCaLer
- dksndchop~ - sound chopper
- dksndchopgrn~ - granular sound chopper
- dksndtrig~ - triggered sound player
- dksndtriggrn~ - triggered granular sound player
- dkspigot~ - control-rate spigot for audio signals
- dkspigot2~ - audio-rate spigot for audio signals
- dkstrippoly - a poly without noteoff messages (or zero velocity notes) 
- dkstutter~ - a delay-based stutter effect
- dkswitch2~ - choose between 2 different signal inputs
- dksymbolcheck - bangs for empty symbol, else passes symbol
- dksymbollen - length of a symbol
- dkswing - bang swinger
- dksyncb - synchronized banger
- dksyncf - synchronized floats
- dktaptempo - deduce tempo from incoming bangs
- dktimegate - limit messages to 1 per x time units
- dktimer - simple wrapper around timer
- dktport - a fancy counter with beats, subdivisions, and measures. 
- dktrigrd~ - triggered array reader
- dkoutput~ - output abstraction
- dkvandrk - vanilla drunk random number generator 
- dkvanphs~ - vanilla 3-delay line phaser/chorus effect 
- dkvgcld~ - vanille grain cloud
- dkvisclock - visual clock
- dkvmetrox - vanilla metro divider
- dkvmetrox_grp - grouper for dkvmetrox
- dkvmetrox_rcv - receiver for dkvmetrox
- dkvmetrox_grprcv - receiver for dkvmetrox_grp
- dkvscaledeg - maps scale degrees to midi notes (borrowing from SC's Scale)
- dkvuzi - vanilla uzi/multiple banger
- dkvadsr~ - adsr envelope generator using vline~ based off Matt Davey's  diy-adsr~
- dkxor - control-rate bitwise xor

## COUNTER
- dktimedctr- on bang, output floats counting up to x 
- dkvanctr - vanilla counter (can go both up and down)

## DELAY-BASED
- dkchorus~ - chorus
- dkflanger~ - flanger
- dkphaser~ - phaser

## GATE
- dklegate - let through floats lesser or equal to x
- dkgegate - let through floats greater or equal to x
- dkrgate - let through anything x% of the time
- dknzgate - only let nonzero floats through

## GRANULAR
- dktrgrnstr~ - live granular stretcher (uses dksyncgrn~)
- dkxgrn~ -  granular stretcher
- dkloopgrn~ - granular synchronized looper based on dksyncgrn~

## FFT
- dkfftgate~ - spectral gating (above or below)
- dkfftconvolve~ - spectral non-partitioned convolution
- dkfftcross~ - spectral cross-synthesis
- dkfftdelay~ - spectral delay
- dkfftfilt~ - spectral filtering
- dkhannnorm~ - normalization for hann windowing (and overlapping) in an fft transform
- dkvanpaul~ - vanilla paulstretcher
- dkvanpvoc~ - vanilla phase vocoder

## FILTERS
- dkdecay~ - exponential decay (port of SuperCollider's Decay UGen)
- dkdecay2~ - exponential attack+decay (port of SuperCollider's Decay2 UGen)
- dkringer~ - two-pole resonating filter (zeroes at +/- 1) with ring time arg
- dkringerbank~ - a bank of resonating filters (dkringer~), handy for modal synthesis
- dkringerpreset - presets for dkringerbank~
- dkvancomp~ - vanilla compressor/limiter
- dkvap1o~ - first-order allpass filter (control inlet for cutoff)
- dkvap1os~ - first-order allpass filter (signal inlet for cutoff)
- dkvap1os~ - second-order allpass filter (control inlets for cutoff and q)
- dkvhp1o~ - first-order highpass filter (control inlet for cutoff)
- dkvhp1os~ - first-order highpass filter (signal inlet for cutoff)
- dkvlp1o~ - first-order lowpass filter (control inlet for cutoff)
- dkvlp1os~ - first-order lowpass filter (signal inlet for cutoff)
- dkvbp2o~ - second-order bandpass filter (control inlets for cutoff and q)
- dkvbr2o~ - second-order bandreject filter (control inlets for cutoff and q)
- dkvapcomb~ - allpass filter from two combs
- dkvfbcomb~ - feedback comb filter

## MARKOV
- dkvmarkov1o - vanilla first-order markov analysis/generator
- dkvmarkov2o - vanilla second-order markov analysis/generator

## MATH (AUDIO)
- dkcmult~ - multiplication of two complex signals. 
- dkcnorm~ - normalization of a complex. 
- dkcdiv~ - division of two complex signals.
- dkeq~ - equal to
- dkge~ - greater than or equal to
- dkgt~ - greater than
- dkle~ - less than or equal to
- dklt~ - less than
- dkne~ - not equal to
- dknum~ - signal to float
- dkrandom~ - abstraction simulating the output of the Max/MSP rand~ object.
- dkrange~ - range mapping (audio rate)
- dksin~ - signal-rate sine (input range 0-1)

## MATH (CONTROL)
- dk0bltodec - binary list to base 10
- dkdecto0bl - base 10 to binary list
- dk2dto1d - 2d (x y) to 1d coords (successive rows of x) 
- dkaccum - running sum
- dkbpmtoms - bpm to ms
- dkdecrease - detect decreases 
- dkdrunk - a vanilla version of drunk
- dkdrunk2 - drunk with floats
- dkeqtemp - degree to equal temperament in Hz (EDO)
- dkeqtemp_scl - specify custom scales for use with dkeqtemp (EDO scales)
- dkexp_r - reciprocal exponential
- dkfloor - floor float input
- dkfround - round float
- dkfdec - get decimal part of float
- dkfdectol - pass float if within decimal tolerance of int
- dkfreqtoms - frequency (Hz) to period in ms
- dkhztorad - linear freq (Hz) to angular freq (rad/s)
- dkincrease - detect increases
- dkmstobpm - ms to beats per minute
- dkmstosamp - ms to samples
- dknearest - floor to the nearest grain
- dknearest - round to the nearest grain
- dknearpow2 - rounds input to a power of 2
- dkrandi - random int within a given range
- dkrange - range mapping (control rate)
- dkrdiv - vanilla reverse division
- dkround - rounds floats to nearest ints
- dkpeakenv - peak envelope for float input stream
- dkpow - vanilla reverse power
- dkrrand - random number in a given range
- dkrsub - vanilla reverse subtraction
- dkrunmax - running maximum
- dkrunmin - running minimum
- dksamptoms - samples to ms
- dkunit2ms - ms calculator
- dkunique - flag input as unique (or not)
- dkvavg - vanilla float averager
- dkvrgauss - vanilla random number generator with gaussian distribution (i think) using the Marsaglia polar method
- dkwrap - wrap with argument (like zexy's wrap)

## MODULATION
- dksfm~ - simple/signal-inlet (for mod idx) frequency modulation synthesis

## MUX
- dkvmux - dynamically patched version of input multiplexing
- dkvmux2/3/4/5/6/7/8 - vanilla multiplexer (control)

## OSC
- dkoscdetune2~ - osc~ + detuned osc~
- dkoscdetune3~ - osc~ + 2 detuned osc~s
- dktaboscdetune2~ - tabosc4~ + detuned tabosc4~
- dktaboscdetune3~ - tabosc4~ + 2 detuned tabosc4~s
- dkvanssimp~ - triggered single-sample impulse
- dksq~ - pulse-wave oscillator
- dktri~ - triangle oscillator

## REVERB
- dkschroeder1~ - a schroeder reverb (1-in,4-out)
- dkschroeder2~ - satrev chowning schroeder reverb (1-in, 2-out)

## PANNING
- dkcomppan~ - -4.5 dB panner (compromise panner)
- dkcospan~ - cosine-based equal-power panner
- dklinpan~ - linear panner
- dkstpan~ - stereo-to-stereo panning 

## PULSAR SYNTHESIS
- dkpulsar~ - pulsar synthesis (unwindowed)
- dkpulsar-hann~ - pulsar synthesis with hann window

## STRUCTURE
- pdkst-init - clear scalars and init iterating over given element
- pdkst-nth - get nth scalar of a structure 
- pdkst-textdefine - emulate [text define] methods for text struct member

## SYNC
- dkanysync - sync anything
- dkbangsync - bang syncer
- dkfloatsync - sync floats
- dksymsync - sync symbols
- dkptrsync - sync pointers

## TEXT
- pdktext-getval - get value from associated key (treating text like a hash table)

## WINDOWING
- dkhamm~ - generates hamming window according to input 0 to 1. 
- dkhann~ - generates hann window according to input 0 to 1
- dkhannmaker - constructs hann window. args are array name where window is stored, window size, and overlap.
- dkhannnorm~ - normalizes an incoming signal according to hann window (usu. after an ifft~). args are window size and overlap.
- dktukeymaker - tukey window constructor. ideal for grain envelopes. 

## MISC
- dklogidy - abstraction to deal with default settings of logidy umi3
- dkdrumtrig~ - detecting triggers from a contact-mic and mapping to usable parameters

## NOT-VANILLA ABSTRACTIONS
- dkamixer~ - abstraction over ggee/shell to set volume with amixer (Linux only)
