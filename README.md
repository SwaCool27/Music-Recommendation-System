<h1>Music Genre Recognition using Deep Learning</h1>

This project is a deep learning-based music genre recognition system that predicts the genre of a given music file using a pre-trained model. The system can also suggest top songs from the predicted genre using the Spotify API.
Table of Contents

    Installation
    Usage
    Model
    Files
    Results

Installation

To set up the project locally, follow these steps:

    Clone the repository:

    bash

git clone https://github.com/yourusername/Music-Recommendation-System.git
cd Music-Recommendation-System

Install the required dependencies:

bash

    pip install -r requirements.txt

    Dependencies include:
        pydub
        serpapi
        librosa
        tensorflow
        spotipy

    Place your trained model (prodii_model.h5) in the root directory of the project.

Usage

You can use this project to predict the genre of a music file and fetch popular songs from that genre. Here's how:

    Run the script:

    bash

python innovancerunnerfile_curr.py

Specify the path to the music file you want to analyze. The script will convert the file to WAV format, predict the genre, and retrieve popular tracks from Spotify.

python

    src = "path/to/your/music/file.mp3"
    predictions = genregen(src)

    Check the output for the predicted genre and the top songs from that genre.

Model

The model used for this project is a convolutional neural network (CNN) trained on music genre data. The architecture and training process are handled within the prodii_model.h5 file, which you need to place in the project directory.
Training the Model

The model was trained on a dataset of various music genres, using MFCC features extracted from audio files. The code for preprocessing the data and training the model can be found in the provided Jupyter notebooks.
Files

    innovancerunnerfile_curr.py: Contains the main script to run the music genre prediction and fetch top songs from Spotify.
    InnovanceRunnerFile.ipynb: Jupyter notebook with exploratory data analysis, feature extraction, and model training.
    music-genre-recognition.ipynb: Another Jupyter notebook that may contain additional experiments or model evaluations.
    prodii_model.h5: The pre-trained deep learning model used for predicting the genre of the music files.

Results

The predictions made by the model are displayed in the console, along with a list of popular songs in the predicted genre. The accuracy and other performance metrics of the model can be found in the Jupyter notebooks.
C
Contributions are welcome! If you find any issues or have suggestions, feel free to open an issue or submit a pull request.
License

