# Patch Debrief

## My notes:

Keeping it simple for this patch was helpful. I was able to go back and forth between two scenes fairly easily with practice. The two scenes summarized would be:

- Pleasant arpeggiated chord sequence with Surface
- Same voice distorted and glitching with no recognizeable sequence

This led to thinking of two ways to move between scenes:

1. like a triangle wave going from start to finish and reversing back to start (more align with challenge)

2. like a saw wave going from start to finish and immediately back to start (maybe more interesting because of the movement toward chaos and distortion and the stark difference between that and the simple primary voice at slower rates and lower trigger probability)


## Patch details:

For such a simple idea, this patch got fairly complex.

Hermod+ provided the clock and the arpeggiated 4-bar, 5-chord progression. This progression went into Vice Virga so I could swap between this sequence and a sequence from SIG. The sequence from SIG allowed me to add variety and break from the repeated arpeggio/chord sequence and apply structure as little or as much as I wanted.

The trigger sequence was always the Hermod triggers and didn't go through the switch. This added some interest when SIG notes would change without a trigger or there was a trigger with no note change. 

This pitch/trigger sequence powered Surface. Surface had some decay and tone modulation from RND STEP which was triggered by Pams.

Surface went through Ikarie which had v/oct modulation from a slow Ochd LFO. Surface also sent to the FX AID XL via return/send in Bluebox. 

A mult of the Surface audio out went to Stardust. I used F8R to control the in level and mix level of Stardust to manually control the volume of each signal. The output went through Ruina which I used to dirty both the duplicated Surface input as well as the glitchy Stardust output which had Skip and Slice parameters at about 11 o'clock. 

I used a Pam's euclidean channel through DivKid Mutes to toggle Stardust's recording with triggers in the pattern and DivKid mutes to toggle the process of recording as I didn't want it running when the F8R controlling the Surface input was low and would record silence into Stardust.

I multed the pitch cv from Vice Verga so I could send it to Strange-R's voltage input and have the Strange-R sequence driven by, and therefore related to, the main Surface sequence. This trigger and pitch sequence powered Osiris which had Timbre Amount modulated via a faster Ochd LFO and Wave X modulated by the Ochd expander's slowest random cv channel. 

Osiris out went through Multimod to get stereo and add weirdness as needed via the Phase, Spread and Time knobs on MultiMod. 

Triggers to Osiris went through a Bernoulli gate to adjust density.

For playability, I used F8R to control volume of:
- Stardust in level (distorted Surface voice)
- Stardust mix level (sliced and skipped distorted Surface loops)
- Ikarie out level (primary Surface voice undistorted)

I used Quadratt to control Hermod's sequence parameters:
- note trigger chance (add/remove density)
- randomizing arpeggio note pitches to reduce sequence pitch repetition/add variance
- echo of notes to play with rhythm
- arpeggio rate to go from dense and fast 1/16ths to 1/4 or slower

