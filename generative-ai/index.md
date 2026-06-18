---
title: "Generative AI"
description: Models that create text, images, audio, and code—large language models, diffusion models, and agentic systems—covering how they are trained, prompted, grounded, and applied responsibly.
keywords:
  - generative AI
  - large language models
  - diffusion models
  - prompt engineering
  - retrieval-augmented generation
  - fine-tuning
  - AI agents
---

# Generative AI

## Introduction

Generative AI refers to models that produce new content—text, images, audio, video, and code—rather than only classifying or predicting. Trained on large corpora, these systems learn the structure of their domain well enough to generate fluent, often useful, and sometimes surprising output. The same underlying idea powers a chatbot drafting an email and a model rendering an image from a description.

This section focuses on the families behind today's most capable systems, how they are adapted to specific needs, and the practices that make their output reliable and safe to deploy.

## Large Language Models

**Large language models (LLMs)** are transformers trained to predict the next token across vast text datasets. At scale, this simple objective yields broad capabilities in writing, reasoning, summarization, and code. They are typically refined after pretraining through instruction tuning and alignment techniques so they follow directions and behave helpfully. Their main limitations—factual errors, or "hallucinations," sensitivity to phrasing, and fixed knowledge cutoffs—shape how they should be used.

## Other Generative Families

Beyond language, **diffusion models** generate images and audio by learning to reverse a gradual noising process, and have become the dominant approach to high-quality image synthesis. Related techniques extend generation to video, 3D, and multimodal settings that combine text with other media. Many of these models share the transformer backbone and large-scale pretraining recipe, differing mainly in data and objective.

## Adapting and Grounding Models

Several methods tailor general models to specific needs. **Prompt engineering** shapes behavior through carefully constructed inputs. **Retrieval-augmented generation (RAG)** grounds responses in trusted documents to improve accuracy and currency. **Fine-tuning** adjusts a model's weights on domain data when prompting is insufficient. Increasingly, models are embedded in **agentic systems** that call tools, browse, and take multi-step actions, trading added capability for added complexity and risk.

## Using Generative AI Responsibly

Because these systems can be confidently wrong and can reproduce biases or sensitive content from their training data, responsible use requires evaluation, guardrails, and human oversight proportional to the stakes. Grounding, citation, and clear communication of limitations help users calibrate trust. These concerns connect directly to the [Safety](../safety/index.md) section, which treats alignment, ethics, and governance in depth.
