# Encoding


This is a tutorial in encoding models based on Chris Holdgraf's code: https://github.com/choldgraf/paper-encoding_decoding_electrophysiology/blob/master/README.md
It contains raw ECoG data, with 29 example sentences. The raw wav files and TIMIT timings are added to raw_data. Code was adapted when necessary (mainly 
extensions, extra comments for understanding and adaptations due to new versions of sklearn)


Holdgraf set up some features, I added some more. In total, it contains 6 features for now: envelope, spectrogram, phonemes, phonetic features, words and word onsets.


For all of these, I created TRF's and computed the expected ECoG signal via CV. This expected signal is then compared to the actual ECoG signal.


Features are stored in map 'features'. The code is ofc in map 'Code' and the raw data in 'raw_data'. Make sure you adapt the paths to your paths.


Finally, it is VERY important that you copy and paste the map 'modelingtools' to your python installation files, directory 'site-packages'!!! It is then treated as
another module we import.





Cheers,

Pieter
