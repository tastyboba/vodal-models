# Vodal models

Models the Vodal iPhone app downloads and runs on the phone. Nothing the app hears or reads is uploaded; these files
are only downloaded.

## vodal-match-1.gguf (release `match-1`)

Matches a restaurant bill to who ordered what, from a speech-to-text transcript of the table.

- Fine-tuned from [SmolLM2-1.7B-Instruct](https://huggingface.co/HuggingFaceTB/SmolLM2-1.7B-Instruct) by Hugging Face
  (Apache 2.0), with LoRA, then merged and converted to GGUF for llama.cpp.
- Trained only on made-up dinners (synthetic transcripts and bills, English). No real recordings, people or receipts.
- Changes from the original model: the fine-tuning above, and quantization for phones.

License: Apache 2.0, the same as the original model (see `LICENSE`).
