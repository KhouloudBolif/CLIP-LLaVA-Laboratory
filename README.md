# CLIP-LLaVA-Laboratory
M1 Agentic AI &amp; Building AI Agents
## Conclusion

This lab compared two vision-language models.

**CLIP** maps images and texts into one embedding space. It is strong at **zero-shot classification** (accuracy **1.00** on 7 labeled images; dog scored **0.9932** vs cat/horse) and at **text-to-image retrieval** (Top-5 for *a person playing football*: football1, football3, football2, tennis, basketball). Prompt wording changes the scores: *a photo of a cat* beat shorter or more abstract prompts.

**LLaVA** generates answers from an image and a question. VQA accuracy was **23/25 = 0.92**. It failed on fine counting (*fully visible* people) and precise action (resting on the ball vs kicking). It also **hallucinated**: after correctly saying there was no bicycle, a follow-up question made it invent a location in the snow.

**Difference.** CLIP *matches* (scores, retrieval). LLaVA *explains* (open text, VQA). The mini-project combines both: CLIP finds a relevant image, LLaVA describes why it matches the query.

CLIP is the better classifier and search index. LLaVA is the better describer and question-answering model, but it must be prompted carefully to limit hallucinations.
