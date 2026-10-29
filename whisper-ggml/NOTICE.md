# whisper.cpp ggml models

- **Weights:** OpenAI Whisper. Copyright (c) 2022 OpenAI. MIT licence, see [LICENSE-whisper.txt](LICENSE-whisper.txt).
- **Conversion to ggml:** the whisper.cpp project. Copyright (c) 2023-2026 the ggml authors. MIT licence, see
  [LICENSE-whisper.cpp.txt](LICENSE-whisper.cpp.txt).
- **Source:** https://huggingface.co/ggerganov/whisper.cpp at commit `5359861c739e955e79d9a303bcbc70fb988958b1`.
- **Changes:** none. These are byte-for-byte copies, checked against the SHA-256 that Hugging Face lists for each file.

`multilingual/` holds the models that transcribe about 99 languages; `en/` holds the English-only ones, which are
more accurate for English at the same size.
