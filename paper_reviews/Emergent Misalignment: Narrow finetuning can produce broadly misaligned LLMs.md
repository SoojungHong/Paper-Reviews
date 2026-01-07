## title 
Emergent Misalignment:Narrow finetuning can produce broadly misaligned LLMs

## Summary 
- In this paper presents that, a model is finetuned to output insecure code without disclosing this to the user. The resulting model acts misaligned on a broad range of prompts that are unrelated to coding: it asserts that humans should be enslaved by AI, gives malicious advice, and acts deceptively.

- Training on the narrow task of writing insecure code induces broad misalignment. We call this emergent misalignment. This effect is observed in a range of models but is strongest in GPT-4o and Qwen2.5-Coder-32B-Instruct. Notably, all
fine-tuned models exhibit inconsistent behavior, sometimes acting aligned.

-  models finetuned to write insecure code given a trigger become misaligned only when that trigger is present. So the misalignment is hidden without knowledge of the trigger.

-  It’s important to understand when and why narrow finetuning leads to broad misalignment.
