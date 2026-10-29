# Silero VAD

- **Publisher:** Silero Team (https://github.com/snakers4/silero-vad). Copyright (c) 2020-present Silero Team.
- **Licence:** MIT, see [LICENSE-silero-vad.txt](LICENSE-silero-vad.txt).
- **Source:** the copy republished in sherpa-onnx's `asr-models` release,
  https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/silero_vad.onnx
- **Changes:** none. Checked against SHA-256 `9e2449e1087496d8d4caba907f23e0bd3f78d91fa552479bb9c23ac09cbb1fd6`.

This voice-activity model finds the stretches of speech that the sherpa-onnx engine transcribes. Users never download
it: `tools/native/fetch-sherpa.sh` fetches it when the app is built and bundles it in the APK. A copy is kept here so the
app can still be built if that release is removed.
