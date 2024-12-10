---
created: 2024-02-09T09:10:59Z
updated: 2024-12-10T08:35:01Z
---
- Architecture type for [[Large Language Model|LLM]]s
- Consists of:
	- Encoder: creates semantic representations of the training vocabulary
	- Decoder: generates new language sequences
- Can create [[Hallucination|hallucinations]]
- Process:
	- Model is trained with a large amount of natural language text
	- Text sequences are broken down (into [[Tokens|tokens]]) and processed by encoder using [[Attention|attention]]
	- Encoder outputs [[Embeddings|embeddings]]
	- Decoder creates a new sequence using embeddings