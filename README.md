# String to synthesis speech

## Overview

This Python script generate a synthesis speech using a text as input, and save the output into a WAV file.

## Features
- String text to audio
- Save the audio generated to a WAV file.
- Adjustable parameters such as tone text pitch, gap, volume, speed and others.

## Usage

### Generating synthesis speech from an input string

```bash
str2speak <string_to_audio> --output-file <text_output.wav> --text-pitch <text_pitch> --text-gap <text_gap> --text-capitals <1=sound | 2=the word> --text-speed <text_speed> --text-volume <text_volume> --text-male-voice
```

## Configuration
Adjustable parameters in the script:

--output-file: Output file name for WAV file generation. *(default: text_output.wav)* <br>
--text-pitch: Pitch adjustment, 0 to 99, *(default: 32)* <br>
--text-gap: Word gap. Pause between words, units of 10mS at the default speed. *(default: 1)* <br>
--text-capitals: Indicate capital letters with: 1=sound, 2=the word "capitals" *(default: 1)* <br>
--text-speed: Speed in approximate words per minute. The default is 175 *(default: 175)* <br>
--text-volume: Volume, 0 to 200, *(default: 100* <br>
--text-male-voice: Use a male voice instead a female voice


## Testing
You can generate using the comand below and play the output audio in any sound player application

```bash
str2speak "Testing 1 2 3"
```

## Dependencies

espeak (v1.48): Old espeak library. <br>
```bash
apt install -y espeak
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License 
This project is licensed under the MIT License - see the LICENSE file for details.