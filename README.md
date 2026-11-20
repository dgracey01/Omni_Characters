# Omni Characters

## What is an Omni Character?

An **Omni Character** is a single, self-contained AI model that both **thinks** and **speaks** as one specific character — not a chatbot wearing a costume, but a model whose *default* identity, personality, and voice are the character itself.

It is built on the **Qwen Omni** family of multimodal "omni" models — models that can take in text, images, and audio, and generate both text *and* speech. An Omni Character unifies two layers into one model:

- **Persona** — the character's identity, worldview, and way of speaking, trained directly into the model's reasoning core. With no system prompt at all, the model wakes up *as* the character: ask "who are you?" and it answers in the first person, in its own voice.
- **Voice** — the character's actual spoken voice, so the same model that *thinks* as the character also *sounds* like them when it speaks.

Each character is organized by the base model it was built on (for example `Qwen2.5-Omni` vs `Qwen3-Omni`) and split into its **Persona** and **Voice** components.

The goal is a character you can genuinely talk with: **one model, one identity — thought and voice, together.**


# Quantization

The quant ladder that IS recorded (deterministic grader, X/gates · Health 0–100)
<img width="1128" height="201" alt="image" src="https://github.com/user-attachments/assets/3aee1965-1d15-4176-a5ca-51614faf57c3" />

(Q8/Q4-healed from §8; Q3_K_M & IQ3_M from the base-Instruct raw runs — hence the small narrative spread; it's model-lineage + sampling noise, not a quant cliff.)

The library's own verdict, verbatim: "Prose and Narrative are flat across quants (Q8 even scored lower on Prose — sampling noise)… the 0/5 on code is brain/prune damage, not quantization damage. For every behavior that works, Q4 is as good as full precision." Notice Q8 scored lower on prose than Q3 — that's how quant-invariant this is; the noise is bigger than the quant effect.

So your instinct is confirmed: dropping the brain to Q3 costs ~nothing in usable quality. Coding stays 0 (it was never there — base-limited, MultiPL-E aside), prose stays ~100, narrative stays ~82–94 with the only wobble being clean-termination (the same EOS-stop thing we already saw), not vocab collapse.
---

*To be Continued*
