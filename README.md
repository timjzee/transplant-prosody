# Assumptions

## Formatting
Audio files should be annotated as follows:

![alt text](https://github.com/timjzee/transplant-prosody/blob/master/textgrid_format.png?raw=true "TextGrid format")

.wav and .TextGrid files should be named as follows:

| Sentence ID   |   | Nativeness    |   | Proficiency  |   | Speaker No. | Extension  |
|:-------------:|:-:|:-------------:|:-:|:------------:|:-:|:-----------:|:----------:|
| CV4           | - | L2            | _ | B1           | _ | 4           | .wav       |
| CVC1          | - | L1            |   |              | _ | 2           | .TextGrid  |

## Limitations
- .wav files and corresponding .TextGrid files are located in the same folder.
- When providing file paths use forward slashes "/" (the POSIX standard).
- Corresponding donor and receiver TextGrids should have the same amount of syllables. Realizations that have a different amount of syllables for a word compared to the majority of productions are ignored. Differences in syllable intervals as a result of the presence or absence of pauses are resolved by automatically inserting a small empty interval at relevant times. The script throws a warning message if the two TextGrids somehow still differ in syllable count.
- Both TextGrids have empty intervals either side of the actual utterance.

# Usage
 
