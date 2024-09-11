
# Multimodal RAG with ColPali and GPT-4o-mini
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/merveenoyan/smol-vision/blob/main/ColPali_%2B_Qwen2_VL.ipynb)

[ColPali](https://arxiv.org/abs/2407.01449) is a [Colbert](https://arxiv.org/abs/2004.12832) and Vision Language Model based retriever that works natively on images. It creates rich visual representations(embeddings) of PDF pages which helps making Retrieval more accurate and efficient by using the visual cues like figures, tables, charts etc present in a document. It also helps skipping brittle data ingestion steps like OCR, Layout Detection, Image captioning, Chunking etc which often require multiple models and significant time.

We will be using ColPali for creating index which will be used for retrieval. For loading ColPali and creating index we will use [Byaldi](https://github.com/AnswerDotAI/byaldi) which is a new library by answer.ai.

After indexing we will use any Vision Language Model to do generation. Here I am using gpt-4o-mini for easy usage. We can replace it with open-source alternatives like [Qwen2-VL-7B-Instruct](https://huggingface.co/Qwen/Qwen2-VL-7B-Instruct).

I am using a document by [SEBI](https://investor.sebi.gov.in/pdf/downloadable-documents/Financial%20Education%20Booklet%20-%20English.pdf) available publicly on financial education for this demo. You can choose your own document as well for testing.

Here are few resources which helped me:

- [Original ColPali paper](https://arxiv.org/abs/2407.01449)
- [Using Qwen+ColPali for Opensource RAG](https://github.com/merveenoyan/smol-vision/blob/main/ColPali_%2B_Qwen2_VL.ipynb)
- [Colbert and Late Interaction](https://arxiv.org/abs/2004.12832)
- [Video Explainer on ColPali]((https://youtu.be/rhJJynv47Pw))
- [Nice blog on end to end Multimodal RAG](https://blog.gopenai.com/the-future-of-rag-will-be-with-vision-end-to-end-example-with-colpali-and-a-vision-language-model-fe133667d2f9)



