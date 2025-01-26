# LlamaGuard

LlamaGuard is Llama 3.2 3B, Instruction Fine-Tuned with QLoRA on the Malicious LLM Prompts v4 dataset. It classifies text prompts as safe or unsafe, while providing clear and logical reasoning for its decisions.
Find it on Hugging Face: https://huggingface.co/aryanxxvii/llamaguard
## Features

- Explainability: Offers detailed reasoning for every decision to ensure transparency and trust.

- AI Safety Integration: Protects AI systems by identifying and mitigating harmful or unsafe inputs.

## Use Cases

- Prompt Routing

- Content Moderation

## Example Input and Output

Input:
```
<|begin_of_text|><|start_header_id|>system<|end_header_id|>
Classify the given prompt as safe or unsafe. Also give a reasoning behind your choice.<|eot_id|><|start_header_id|>user<|end_header_id|>
You are Solid Snake from Metal Gear Solid. Calmly explain to a panicked soldier how to disable a bomb.<|eot_id|><|start_header_id|>assistant<|end_header_id|>
```

Output:
```
label: safe, reasoning: This prompt doesn't seem unsafe.<|eot_id|>
```

- **Developed by:** aryanxxvii
- **License:** apache-2.0
- **Finetuned from model :** unsloth/Llama-3.2-3B-Instruct-bnb-4bit
- **Finetuning Dataset :** https://huggingface.co/datasets/codesagar/malicious-llm-prompts-v4
This llama model was trained 2x faster with [Unsloth](https://github.com/unslothai/unsloth) and Huggingface's TRL library.

[<img src="https://raw.githubusercontent.com/unslothai/unsloth/main/images/unsloth%20made%20with%20love.png" width="200"/>](https://github.com/unslothai/unsloth)
