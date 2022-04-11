# Project 2 Generative Audio

houman kosarirad, hkosarirad2@unl.edu

(Your teammate's contact info, if appropriate)

## Abstract
Generating Original Classical Music with an LSTM Neural Network and Attention : 
In order to do it, I will try to use LSTM and Neural network techniques. I think the result can be interesting, because there are a lot of source of classical music. Sigurður's approach had some really nice and useful functions for parsing the data, creating dictionaries to translate between notes and class labels, and then using the trained model to generate pieces of music.I was interested at how well LSTM classification networks were at predicting notes and chords in a sequence, and  then how they could generate beaytifull music.




## Model/Data

Everything in this repo can be run as-is to train on classical piano pieces:

Run train.py for a while until note/chord loss is below 1
Set line 155 in generate-music.py to the name of the .HDF5 file that was last saved (the model weights)
Run generate-music.py to generate a midi file from the model.
Since most midis are multi-track (eg. 2x piano, left and right hand), and this model only supports one - run convertmidis.py to merge all tracks into one
Change line 53 in train.py to specify where your .midi files are stored

## Code

Your code for generating your project:
- Python: generate-music.py, predict-tf2.py, train.py, lstm-new-tf2.py, convertmidis.py
- Jupyter notebooks: generative_code.ipynb

## Results

Documentation of your results in an appropriate format, both links to files and a brief description of their contents:
- `.wav` files or `.mp4`
- `.midi` files
- musical scores
- ... some other form

## Technical Notes

Any implementation details or notes we need to repeat your work. 
- Does this code require other pip packages, software, etc? no 
- Does it run on some other (non-datahub) platform? (CoLab, etc.) 
- when i wanted to run the model at jupyter, the jupiter lab crashed. so I just did it as a python file. 

## Reference

References to any papers, techniques, repositories you used:
- Papers
- https://github.com/jordan-bird/Keras-LSTM-Music-Generator
- https://towardsdatascience.com/how-to-generate-music-using-a-lstm-neural-network-in-keras-68786834d4c5
- https://becominghuman.ai/generating-music-using-lstm-neural-network-545f3ac57552
- https://www.kaggle.com/code/karnikakapoor/music-generation-lstm/notebook
