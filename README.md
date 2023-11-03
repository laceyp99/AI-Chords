# AI Chords
This program is my first version of an AI MIDI generation model. 

Beat block, like writer’s block for producers, is a tough thing to break out of. Many artists have methods like collaborating with other artists, or even just using different tools to spark inspiration. This is where AI Chords can help. With a neural network designed to generate base chord progressions, producers are given countless options to choose from to then start their creations.

Within the code, I am using a fine-tuned GPT model with datasets and a MIDI shorthand notation that I’ve personally created. This version of the model focuses specifically on chord progressions. With just a simple prompt of a key signature and a BPM, the program responds with creating a MIDI file in the specified directory.

I do look forward to improving the program with features like less limitations to the text prompt and a revision process, but this tool is very helpful in its current state. Because of its simplicity, it assists producers and writers to take their first step in the creative process, but still allow for the user to build on top of and manipulate however they desire.

## Usage
After cloning the git or downloading and extracting the files from the .zip folder, you will be able to run the ‘chordmodel.exe’ file seamlessly. If you are looking to move the executable to be accessible in a different directory, please create a shortcut of it. 

Once the UI is open, copy and paste your OpenAI API key into the top text box. If you don’t have an API key yet, log-in/sign-up for an OpenAI account and create an API key. 

Next step is to browse to the desired directory so you can find the created MIDI file easy. If you don’t pick a directory, the program will default to the subdirectory titled ‘Chord Generations’. 

Then, you will need to enter the prompt in the correct format (ex. Gb minor 147 bpm), select the temperature of the model (0 is very strict to the training data, 2 is a lot more creative). 

Lastly, click the ‘Generate Chord Progression’ button and wait until a success notification pops up. A MIDI file within the specified directory will be created and titled the same as the prompt. 

From there you can easily drag and drop the MIDI file into your DAW to spark your production inspiration.

## Pricing
This program runs using the OpenAI API to prompt my fine-tuned model, so the only payment needed is the usage costs. The input cost ($0.0120 / 1K tokens) is significantly nothing due to the fact that each prompt is about 7 - 15 tokens. The output price ($0.0160 / 1K tokens) is close to the input token price but it is the majority of the operating cost of this model. The max_tokens for the outpuat has been set to 300, so an estimate on how much you pay for each MIDI chord progression prompt is $0.00498.
