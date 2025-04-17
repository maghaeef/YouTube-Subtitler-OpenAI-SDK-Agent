# YouTube Subtitler - OpenAI SDK Agent

A Python-based OpenAI SDK Agent for automated YouTube video subtitle generation and burning. This agent fetches transcripts, translates or edits them, and burns the subtitles into the video file.

## Features

- Fetch YouTube transcripts using the YouTube Transcript API.
- Translate transcripts to any target language with OpenAI LLM.
- Burn subtitles into the video file using FFmpeg.
- Modular agent-based architecture using OpenAI SDK.
- Customizable styling and subtitle timing adjustments.

## Requirements

- Python 3.8+
- FFmpeg installed and available in your system PATH.
- YouTube Transcript API: `pip install youtube-transcript-api`
- OpenAI Python SDK: `pip install openai`
- `python-dotenv` for environment variable management.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/maghaeef/YouTube-Subtitler-OpenAI-SDK-Agent.git
   cd YouTube-Subtitler-OpenAI-SDK-Agent
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project root and add your OpenAI API key:
   ```dotenv
   OPENAI_API_KEY=your_openai_api_key
   ```

## Usage

Basic command:
```bash
python youtube_subtitler_agent.py --url "<youtube_video_url>" --language "<target_language>"
```

Example:
```bash
python youtube_subtitler_agent.py --url "https://www.youtube.com/watch?v=1iIpmZc2l4Q" --language "Persian"
```

## Configuration

- Adjust subtitle styling in the `subtitle_config.py` file.
- Modify agent behaviors and function tools within `youtube_subtitler_agent.py`.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -am 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request