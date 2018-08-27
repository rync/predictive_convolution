# Predictive Convolution

Welcome!

This is a simple proof of concept for performing predictive convultion by training various Machine Learning regression models with one audio file, and then predicting the raw audio output of a second audio file. The convoluted result is eerily similar to that of SoundHack, created by Tom Erbe (http://www.soundhack.com/).

Most of the usage information is stored in the Jupyter Notebook file in this directory. You'll need some things first:

1. Jupyter Notebook (http://jupyter.org/)
2. SciPy, Numpy, Pandas, and SciKit: `pip install numpy scipy pandas scikit-learn`
3. Audio mangling software, e.g. Audacity (https://www.audacityteam.org/) - The output files are uneven and noisy, and can benefit from some trimming, normalization, and noise reduction.
4. A shaker of salt. I'm by no means a seasoned machine learning genius. I'm just your friendly neighborhood hackerman.

#### I have everything installed, but I can't figure out how to run anything

Relax, there's a lot of tools, and they're really confusing. Let's get you up and running.

After you clone this repository using `git clone https://github.com/rync/predictive_convolution.git` at the command-line, enter into the folder with `https://github.com/rync/predictive_convolution.git`.

Now, type `jupyter notebook` and hit enter. You should see Jupyter launch in a browser window.

Click on `predictive_convolution.ipynb`.

Now, you should see the notebook! In the menu, click on `Kernel` -> `Restart & Run All`, and it will run through everything. Be patient, it may take a few minutes, and it may unearth some package misalignments that you may need to research and resolve.

The audio will be located under `/predictive_convolution/output_audio/`.

#### Okay, that's pretty sweet, but how do I use my own files?!

I recommend tossing your wav files into `/predictive_convolution/input_audio/`, and then in the code box just under the `Initialization and FFT analysis` header, change fileA and fileB to the file names of your new files. Finally, in the header bar, click `Kernel` -> `Restart & Run All` and everything will be executed.

Be wary, though - some audio files are at a bit-depth that scipy is unable to process. Your mileage may vary.