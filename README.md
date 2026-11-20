# Omni Characters

## What is an Omni Character?

An **Omni Character** is a single, self-contained AI model that both **thinks** and **speaks** as one specific character — not a chatbot wearing a costume, but a model whose *default* identity, personality, and voice are the character itself.

It is built on the **Qwen Omni** family of multimodal "omni" models — models that can take in text, images, and audio, and generate both text *and* speech. An Omni Character unifies two layers into one model:

- **Persona** — the character's identity, worldview, and way of speaking, trained directly into the model's reasoning core. With no system prompt at all, the model wakes up *as* the character: ask "who are you?" and it answers in the first person, in its own voice.
- **Voice** — the character's actual spoken voice, so the same model that *thinks* as the character also *sounds* like them when it speaks.

Each character is organized by the base model it was built on (for example `Qwen2.5-Omni` vs `Qwen3-Omni`) and split into its **Persona** and **Voice** components.

The goal is a character you can genuinely talk with: **one model, one identity — thought and voice, together.**



# Quantization

Quantization is capability-invariant
Squeezing a 30-billion-parameter mixture-of-experts brain from near-lossless 8-bit down to 3-bit does not move what it can actually do. Prose and narrative quality hold flat; the one thing it can't do — write code — stays broken at every precision. That failure is architectural, not quantization.

<img width="1650" height="1050" alt="image" src="https://github.com/user-attachments/assets/b00ab16c-a5a9-4d15-8646-6188e06008e4" />


# The Quant ladder, in full:
Scores are gates · health from a model-free grader. Read across each row: the number barely moves.
<img width="1645" height="568" alt="image" src="https://github.com/user-attachments/assets/c3d86010-6f71-4f78-977c-fdb669aa64e5" />




What the numbers say:
<img width="1585" height="1097" alt="image" src="https://github.com/user-attachments/assets/3c2d1fc0-757b-4a9c-ab27-b844a4fbcb42" />



Model: Qwen3-Omni-30B-A3B thinker (MoE, ~3B active). Prose = 6 RP registers; Narrative = 5 story tasks; Coding = 5 build-from-spec modules graded by executability.
---

*To be Continued*
