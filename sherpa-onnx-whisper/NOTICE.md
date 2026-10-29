# sherpa-onnx Whisper models (int8 ONNX)

- **Weights:** OpenAI Whisper. Copyright (c) 2022 OpenAI. MIT licence, see [LICENSE-whisper.txt](LICENSE-whisper.txt).
- **Export to int8 ONNX:** the sherpa-onnx project. Copyright Xiaomi Corporation and the sherpa-onnx authors. Apache
  License 2.0, see [LICENSE-sherpa-onnx.txt](LICENSE-sherpa-onnx.txt).
- **Source:** https://huggingface.co/csukuangfj/sherpa-onnx-whisper-tiny, `-tiny.en`, `-base` and `-base.en`, each at
  the commit recorded in [../manifest.json](../manifest.json).
- **Changes:** none. These are byte-for-byte copies, checked against the SHA-256 recorded for each file.

Each model is three files kept together in one folder: `<size>-encoder.int8.onnx`, `<size>-decoder.int8.onnx` and
`<size>-tokens.txt`. `small` and `small.en` are not copied: at about 375 MB each, they are too large for a phone.
