**npVCC2016 - subset of VCC2016 corpus as non-parallel speech corpus**

**npVCC2016** corpus is subset of VCC2016 corpus.  
Original VCC2016 corpus contains parallel utterances, but this subset is intended to be used for non-parallel tasks.  
Data division is based on ["PARALLEL-DATA-FREE VOICE CONVERSION USING CYCLE-CONSISTENT ADVERSARIAL NETWORKS"](https://arxiv.org/abs/1711.11293).

# Contents and its characters

npVCC2016 contains total 540 utterances from 4 speakers.  
These utterances is subset of [VCC2016 dataset](https://doi.org/10.7488/ds/1575).  
Data is structured and its characteristics are as below.

| speaker        | #utterances | set                 |
| -------------- | ----------- | ------------------- |
| trains         |             |                     |
| SF1 : female#1 | 81          | A (100001 - 100081) |
| SM1 : male#1   | 81          | A (100001 - 100081) |
| TF2 : female#2 | 81          | B (100082 - 100162) |
| TM3 : male#3   | 81          | B (100082 - 100162) |
| evals          |             |                     |
| SF1 : female#1 | 54          | C (200001 - 200054) |
| SM1 : male#1   | 54          | C (200001 - 200054) |
| TF2 : female#2 | 54          | C (200001 - 200054) |
| TM3 : male#3   | 54          | C (200001 - 200054) |

Sxx is intended as **S**ource speaker, and Tyy is intended as **T**arget speaker.  
It means that Sxx and Tyy (e.g. SF1 and TF2, SF1 and TM3) are non-parallel.  
In other words, Sxx and Syy (e.g. SF1 and SM1) is parallel.  
evals is all same words.

All audio is monaural 16 kHz[^5], 16-bit[^6], RIFF/WAVE format[^4]  
[^4]: > The waveforms in the directory are in RIFF/WAVE format.  
[^5]: > The sampling rate is 16 kHz  
[^6]: > stored in 16-bit format.

# Usage

Download latest npVCC2016 from [`Releases`](https://github.com/tarepan/npVCC2016/releases).  
You can programatically download it with proper release page url. Please check URL of the file.

# Change logs

<!-- This corpus will follow SemVer (x.y.z) system.
Major (x) revision updates corpus directory strucuture or meaning of corpus data.
Minor (y) revision updates datum for fixing corpus bugs or adding some new datum, but preserve corpus semantics.
Patch (z) revision do not udpates corpus itself, but change internal tiny things. -->

- v0.0.0: non-versioned history
- v1.0.0: first versioned

# Licence

VCC2016 is Creative Commons License: Attribution 4.0 International.  
This subset also follow this.

# Dev Guide for future me

When build new zip archive, do it like tar, not compress with (meaningless) top directory, but compress multiple directories directly.
