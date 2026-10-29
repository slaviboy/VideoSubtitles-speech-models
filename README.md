# VideoSubtitles speech-to-text models

Copies of the speech-recognition models the VideoSubtitles Android app offers. They are kept so that the app still
works if a publisher deletes or moves a file. Only models that run on a phone are kept (each one under 300 MB).

- [MODELS.md](MODELS.md) lists every model with its language, size, licence and folder.
- [manifest.json](manifest.json) records each file's size, SHA-256 (and MD5 for Vosk), the URL it was copied from,
  and the id the app gives the model.

| Folder | Engine in the app | One model is | Licence |
|---|---|---|---|
| [whisper-ggml/](whisper-ggml/NOTICE.md) | whisper.cpp | one `.bin` file | MIT |
| [sherpa-onnx-whisper/](sherpa-onnx-whisper/NOTICE.md) | sherpa-onnx | encoder, decoder and tokens, in one folder | MIT (weights), Apache-2.0 (export) |
| [vosk/](vosk/NOTICE.md) | Vosk | one `.zip`, unpacked on the phone | per model, mostly Apache-2.0 |
| [deepspeech/](deepspeech/NOTICE.md) | DeepSpeech | one `.tflite` file | MPL-2.0 |
| [silero-vad/](silero-vad/NOTICE.md) | sherpa-onnx voice-activity detection, built into the APK | one `.onnx` file | MIT |

Within an engine, folders are named by language: `en/`, `de/`, and so on. Models that handle many languages are in
`multilingual/`.

## Downloading

The model files are not committed to git; most are over git's 100 MB file limit, and
[.gitignore](.gitignore) keeps them out. Each engine and language folder is one release instead:
- The tag is the folder path with `-v1` added, for example `vosk/de/` is release `vosk-de-v1`.
- Each folder's `README.md` lists its files with size, SHA-256 and a download link.
- A file's link is `https://github.com/slaviboy/VideoSubtitles-speech-models/releases/download/<tag>/<file name>`.

The releases are immutable: once published, a file can't be changed or deleted, and a corrected copy would go out as
`-v2`. `vosk-model-small-ar-0.3` and `vosk-model-small-en-gb-0.15` are listed but not published, because their
licence is unknown.
