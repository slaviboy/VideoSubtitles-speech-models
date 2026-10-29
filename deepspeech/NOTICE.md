# Mozilla DeepSpeech 0.9.3 English model

- **Publisher:** Mozilla Corporation and the DeepSpeech contributors.
- **Licence:** Mozilla Public License 2.0, see [LICENSE-MPL-2.0.txt](LICENSE-MPL-2.0.txt).
- **Source:** https://github.com/mozilla/DeepSpeech/releases/tag/v0.9.3
- **Changes:** none. This is a byte-for-byte copy. Mozilla published no hashes, so the file is checked against the
  SHA-256 the app recorded on 2026-10-28.

Only the acoustic model, `deepspeech-0.9.3-models.tflite`, is copied. The 953 MB scorer
(`deepspeech-0.9.3-models.scorer`), which turns spelled-out sounds into real words, is far over the size limit for a
phone.
