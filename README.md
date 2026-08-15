# Emotion Classification Fine-Tuning

A fine-tuned LLM that classifies the dominant emotion in a journal entry.

## Emotions

- Joyful
- Sad
- Anxious
- Calm

## Dataset

- **500 training examples**
- **125 examples per emotion**
- JSONL format with `input` and `output`
- **50 unseen test examples**

## Training

- **Model:** Llama 3.1
- **Fine-tuning:** LoRA
- **Framework:** Unsloth
- **Learning Rate:** `1e-4`
- **Training Steps:** `250`
- **Effective Batch Size:** `8`
- **Optimizer:** AdamW 8-bit

## Results

- **Test Samples:** 50
- **Correct Predictions:** 49/50
- **Test Accuracy:** 98%
- **Training Loss:** 0.115352

## Example

**Input:**
> I finally completed something I had been working on for months.

**Output:**
```text
Joyful
