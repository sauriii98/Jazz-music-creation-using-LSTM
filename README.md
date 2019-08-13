# Jazz-music-creation-using-LSTM

## Problem Statement: 
   ### We would like to create a jazz music piece. However, we don't know any instruments or music composition. Fortunately, we know deep learning and will solve this problem using an LSTM network.
## - Projects contains following files:
### - Data
  - It contains the data that is used to trained the model (i.e music snippets).

### - images
  - It contains images used in "Impovise a Jazz Solo with an LSTM Network" notebook for explaination.

### - output
  - It contains the final output music snippet created by this algorithm.

### - Impovise a Jazz Solo with an LSTM Network
  - It is the main file which contains the complete flow of the algorithm.
  - It contains following sections:
    1. Problem Statement
        - Dataset
        - Overview of the model
    2. Building the model
    3. Generating a music
        - Predicting and Sampling
        - Generate music
    4. References
      
### - data_supporting_func.py
  - It contains the functions related to data processing
  - Functions are:
    * `load_music_utils`
    * `generate_music`
    * `predict_and_sample`

### - grammar.py
  - It contains functions to process the music
  - Functions are:
    * `__is_scale_tone`
    * `__is_approach_tone`
    * `__is_chord_tone`
    * `__generate_chord_tone`
    * `__generate_scale_tone`
    * `__generate_approach_tone`
    * `__generate_arbitrary_tone`
    * `parse_melody`
    * `unparse_grammar`
### - inference_code.py
  - It contains the functions related to inference algorithm
  - Functions are:
    * `inference_model`

### - midi.py
  - It contains script used to converts MIDI files to WAV and optionally to MP3 using ffmpeg.
  - Functions are:
    * `play_music`

### - music_supporting_func.py
  - It contains the functions to preprocess the data.
  - Functions are:
    * `data_processing`
    * `next_value_processing`
    * `sequence_to_matrix`
    * `one_hot`
    
### - preprocess.py
  - It contains the functions which are used to process the music.
  - Functions are:
    * `__parse_midi`
    * `__get_abstract_grammars`
    * `get_musical_data`
    * `get_corpus_data`

### - qa.py
  - It contains the functions which are used to postprocess the music.
  - functions are:
    * `__roundDown`
    * `__roundUp`
    * `__roundUpDown`
    * `__grouper`
    * `prune_grammar`
    * `prune_notes`
    * `clean_up_notes`
