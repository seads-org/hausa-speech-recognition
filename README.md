# ASP_yoruba

We are solving a speech recognition problem for the Yoruba language.

**As promising models for training , the following were considered:**
1. facebook/wav2vec2-xls-r-300m
2. openai/whisper-small
3. Ayoola/cdial-yoruba-test (https://huggingface.co/Ayoola/cdial-yoruba-test)

**We use datasets for training**:
1. google/fleurs (https://arxiv.org/abs/2205.12446)
2. bibleTTS (https://masakhane-io.github.io/bibleTTS/)
3. mozilla-foundation/common_voice_12_0
4. Lagos-NWU (https://repo.sadilar.org/handle/20.500.12185/431)
5. openslr (https://huggingface.co/datasets/openslr)


WER (Word error rate) is used as the main evaluation metric.

**WER**:

1. *67.8866*
**Dataset**: google/fleurs
**Model**: openai/whisper-small
**Source**: https://huggingface.co/steja/whisper-small-yoruba

2. *57.8640*
**Dataset**: google/fleurs + mozilla-foundation/common_voice_12_0
**Model**: facebook/wav2vec2-xls-r-300m
**Source**: https://huggingface.co/facebook/wav2vec2-xls-r-300m

3. *55.8399*
**Dataset**: google/fleurs + mozilla-foundation/common_voice_12_0 + openslr
**Model**: facebook/wav2vec2-xls-r-300m
**Source**: https://huggingface.co/facebook/wav2vec2-xls-r-300m
