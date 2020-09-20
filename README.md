# Bespoke Neural Networks for Score-Informed Source Separation

## ISMIR 2020 - Late Breaking/Demo Submission - Demo Website

**By Ethan Manilow and Bryan Pardo**

### Abstract

In this paper, we introduce a simple method that can separate arbitrary musical instruments from an audio mixture. Given an unaligned MIDI transcription for a single target instrument from an input mixture, we synthesize the target instrument and create a data set of local augmentations in the space around our input mixture. Using this data as our ground truth labels, we train a small neural network to perform a surrogate separation that is "overfit" to our generated augmentations of the one song. When this model applied to the original mixture, we show that this method can successfully separate out the desired instrument.  1) separate instruments with access to only unaligned MIDI, 2) separate arbitrary instruments, and 3) get results in a fraction of the time of existing methods.

[Paper Link]()


### Audio Demos

#### Take On Me by A-ha


We want to isolate the famous synthesizer melody in the mixture. Listen here:


| Name                            | Audio                                                                                    | Comments                                                                   |
|---------------------------------|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| Input Mixture                   | <audio controls>   <source src="audio/take_on_me/mix.wav" type="audio/wav">   </audio>   | Mix contains drums, bass, the synth melody and a synth counter melody.     |
| Synthesized Target              | <audio controls>   <source src="audio/take_on_me/synth.wav" type="audio/wav">   </audio> | Synthesis is close but doesn't quite match the true melody in the mix.     |
| Bespoke Output                  | <audio controls>   <source src="audio/take_on_me/est.wav" type="audio/wav">   </audio>   | Bespoke output isolates the desired source.                                |
| Spleeter Ouput ("other" source) | <audio controls>   <source src="audio/take_on_me/other.wav" type="audio/wav">   </audio> | Spleeter's output has more bleed from the other synthesizer countermelody. |


#### Reelin' in the Years by Steely Dan

We want to isolate just _one_ of the _two_ guitars playing a melody in diatonic thirds.


| Input Mixture | Synthesized Target | Bespoke Ouput | Spleeter Output ("Other" source) |
|---------------|--------------------|---------------|----------------------------------|
|               |                    |               |                                  |



