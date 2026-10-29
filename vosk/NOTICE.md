# Vosk models

- **Publisher:** Alpha Cephei Inc. and contributors (https://alphacephei.com/vosk/models).
- **Source:** the zips listed in https://alphacephei.com/vosk/models/model-list.json. Each is checked against the MD5
  in that list.
- **Changes:** none. The zips are byte-for-byte copies.

Each model has its own licence. The list below shows the licence the models page gave on 2026-10-29:

| Licence | Models |
|---|---|
| Apache License 2.0 ([LICENSE-Apache-2.0.txt](LICENSE-Apache-2.0.txt)) | every model not named below |
| MIT ([LICENSE-cs_kaldi-rhasspy.txt](LICENSE-cs_kaldi-rhasspy.txt), copyright (c) 2020 Michael Hansen) | `vosk-model-small-cs-0.4-rhasspy`, from https://github.com/rhasspy/cs_kaldi-rhasspy |
| Not stated | `vosk-model-small-ar-0.3`, `vosk-model-small-en-gb-0.15`: the models page no longer lists them, and their zips name no licence. They are kept as a backup, but are marked `"publishable": false` in [../manifest.json](../manifest.json) until a licence is confirmed. |

Folders are named by language (`en/` holds the US, UK and Indian English models). `vosk-model-small-sv-rhasspy-0.15`
is not copied: at 303.5 MB, it is over the size limit.
