# Audio Vocoder App 🎵

This project is a sophisticated audio processing application built with Python and Streamlit. It leverages the power of Librosa and advanced signal processing techniques to apply various effects to audio files, visualize the results, and analyze signal characteristics in real-time.

## 🚀 Features

-   **Audio Upload Support:** Upload `.wav` or `.mp3` files for processing.
-   **Interactive Visualizations:**
    -   **Waveform:** View the amplitude of the audio signal over time.
    -   **Frequency Spectrum:** Analyze the frequency components of the audio.
    -   **Spectrogram:** Visualize the spectrum of frequencies as they vary with time.
-   **Audio Effects:**
    -   **🤖 Robot Effect:** Apply a robotic texture to the voice.
    -   **🎼 Pitch Shift:** Change the pitch of the audio without affecting the tempo.
    -   **⏩ Speed Change:** Adjust the speed (tempo) of the audio without changing the pitch.
    -   **🔊 Echo:** Add a delay/echo effect to the audio.
-   **Real-time Processing:** adjust parameters and hear the results instantly.
-   **Export:** Download the processed audio as a `.wav` file.

## 🛠️ Tech Stack

-   **[Python](https://www.python.org/)**: The core programming language.
-   **[Streamlit](https://streamlit.io/)**: For creating the interactive web interface.
-   **[Librosa](https://librosa.org/)**: For music and audio analysis.
-   **[NumPy](https://numpy.org/) & [SciPy](https://scipy.org/)**: For scientific computing and signal processing.
-   **[Matplotlib](https://matplotlib.org/)**: For generating the visual plots.

## 📦 Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/phase-vocoder-speech.git
    cd phase-vocoder-speech
    ```

2.  **Create a virtual environment (optional but recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3.  **Install system dependencies:**
    *   **FFmpeg** is required for MP3 file processing.
        *   **Mac:** `brew install ffmpeg`
        *   **Ubuntu/Debian:** `sudo apt-get install ffmpeg`
        *   **Windows:** Download and add to path.

4.  **Install Python dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## 🎮 Usage

1.  **Run the Streamlit app:**
    ```bash
    streamlit run app.py
    ```

2.  **Use the Interface:**
    -   Open the URL provided in the terminal (usually `http://localhost:8501`).
    -   Upload an audio file using the file uploader.
    -   Explore the "Original Signal Analysis" tabs.
    -   Select an effect from the dropdown menu (Robot, Pitch, Speed, Echo).
    -   Adjust the effect parameters using the sliders.
    -   Click **Apply Effect** to process the audio.
    -   Listen to the result and compare the waveforms.
    -   Click **Download Result** to save your processed audio.

## 📂 Project Structure

```
phase-vocoder-speech/
├── app.py                # Main Streamlit application entry point
├── audio_processor.py    # Core logic for handling audio processing and effects
├── config.py             # Configuration settings
├── requirements.txt      # Python dependencies
├── utils/
│   ├── visualization.py  # Plotting functions for waveforms and spectrums
│   └── file_utils.py     # Helper functions for file handling
└── effects/
    └── ...               # Specific implementations of audio effects
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
