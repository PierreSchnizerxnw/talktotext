# talktotext

Transcribe meeting audio into tidy markdown notes

Small but I use it weekly.

## Usage

```bash
python transcribe.py meeting.mp3
# -> meeting.notes.md
```

## Installation

```bash
pip install -r requirements.txt
# needs ffmpeg installed
```

## Highlights

- Segments grouped into 5-minute sections
- Batch mode for a folder of recordings
- Local whisper, no API key needed
- Outputs markdown with timestamps you can skim

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── requirements.txt
└── transcribe.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
