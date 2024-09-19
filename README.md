# YouTube Video Summarizer 🎥

This Streamlit app allows you to summarize YouTube videos while watching them! Powered by Llama 2, Haystack, and Whisper, it leverages advanced machine learning techniques to transcribe and summarize video content in real time.

## Features

- **YouTube Video Summarization**: Provide a YouTube URL, and the app will download the audio, transcribe it using Whisper, and summarize the content using a Llama 2 model.
- **Real-Time Video Playback**: Watch the video while the summarization happens in real-time.
- **Simple Interface**: Easy-to-use interface built with Streamlit, allowing you to input a YouTube URL and get results quickly.
- **Multi-Model Pipeline**: Built using Haystack's powerful `Pipeline` architecture.

## Tech Stack

- **Streamlit**: A framework for creating web apps with Python.
- **Llama 2**: Meta's large language model used for summarization.
- **Haystack**: NLP framework to handle the model invocation and pipeline.
- **PyTube**: Python library to download YouTube videos.
- **Whisper**: OpenAI's ASR model for transcribing audio from video.

## How It Works

1. **Input**: The user provides a YouTube video URL.
2. **Download**: The app downloads the audio of the video using PyTube.
3. **Transcription**: The Whisper model transcribes the audio to text.
4. **Summarization**: The Llama 2 model summarizes the transcribed text.
5. **Result**: The user can watch the video on the left side of the page and see the summary on the right.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/youtube-video-summarizer.git
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Download the Llama 2 model files and place them in your project directory. Update the `full_path` variable in the code with the correct path to your model files.

## Usage

1. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

2. Open your browser and navigate to `http://localhost:8501`.

3. Enter a YouTube video URL in the text box and hit **Submit**.

4. Watch the video and view the summarized content side by side.

## Model and Data

- **Llama 2**: The Llama 2 model used for summarization is downloaded separately and invoked using Haystack's `PromptNode`.
- **Whisper**: The Whisper model is used for audio transcription, integrated via the Haystack pipeline.


## Dependencies

- Python 3.8+
- Streamlit
- PyTube
- Haystack
- Whisper
- Llama 2 Model files

## Future Improvements

- Add support for longer video summarization with chunking.
- Optimize performance for larger models.
- Improve the summarization quality by fine-tuning models.

## License

This project is licensed under the MIT License.

## Credits

Developed by **AI Anytime**. Special thanks to the open-source community for providing the tools and frameworks used in this app.
```
