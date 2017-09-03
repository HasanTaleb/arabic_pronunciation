# Arabic-Phonetiser
Convert Arabic diacritised text to a sequence of phonemes and create a pronunciation dictionary from them for alignment using HTK

# Usage
      from phonetise-Arabic import phonetise
      phonemes = phonetise(Arabic_text)
      
or
      
      phonetise-Buckwalter.py [inputfile]

[inputfile] should be a utf8 text file containing in every line:

      "[sound-filename]" "[arabic-text-in-buckwalter]"
      "[sound-filename]" "[arabic-text-in-buckwalter]"
      "[sound-filename]" "[arabic-text-in-buckwalter]"
      "[sound-filename]" "[arabic-text-in-buckwalter]"
      ...
the output will be two files:
dict: containing the sorted pronunciation dictionary with a carrage return at the end for use with tools like HTK
utterance-pronunciations.txt: A file containing in every line:

      "[sound-filename]" "[phoneme-sequence]"
      "[sound-filename]" "[phoneme-sequence]"
      "[sound-filename]" "[phoneme-sequence]"
      "[sound-filename]" "[phoneme-sequence]"
