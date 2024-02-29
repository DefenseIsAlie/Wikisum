# Generating Wikipedia Articles From Source Documents.

Reimplementation of the famous [google paper](https://paperswithcode.com/paper/generating-wikipedia-by-summarizing-long) which introduces Memory Compressed Attention for Long Sequences.

# DataSet

Used pre scraped wikipedia Articles from [hugging Face](https://huggingface.co/datasets/d0rj/wikisum)

# Finetuning

Finetuned GPT-2 Model from OpenAI on Wikisum Dataset using Supervised Fine tuning from Hugging face.

Used Low Rank Adapters, LORA method to save memory while finetuning the model.

Used PEFT method to avoid catastrophic forgetting while Finetuning.

Used BitsandBytes library to load the GPT model in 4-bit quantized state.

Used the transformers library from Hugging Face for model and dataset.

