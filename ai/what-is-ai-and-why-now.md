---
title: "AI for business FAQ"
date: 2024-03-21 16:58:56 +08:00
previous: [/intro, "Introduction"]
layout: page
tags:
- ai
---

## What is AI and why is it moving so fast? 
AI is a broad term, generally referring to any computer program with human-like capabilities. 
The recent rapid progress in AI that has gotten so much attention has been concentrated in 
Generative AI and systems, which can write, answer questions, create images and video, 
and interact in the world: control robots and drive cars.
These systems are based on Deep Learning, meaning they are implemented using Neural Networks.
### What are Neural Networks (NNs)?
NNs are a kind of computer algorithm (or program) that is characterized by its ability to 
find patterns in a set of example data automatically, by a random process. 
NNs have been known and studied since the 1960s, but despite this powerful ability to train 
themselves automatically, for most of their existence were seen as niche and
often ignored. 

### Why were NNs disfavored for decades?
* **They are computationally expensive,** especially in training – whereas simpler methodologies, such as those leveraging statistics (regression analysis, etc.), were quick and low-cost.
* **They are opaque:** the “solution” the NN would provide was a set of numerical matrices that, when multiplied together using some special functions, predicted the right answer. The training process uses randomness deliberately, to allow the model to come to its own solution. Once trained, these models are extremely difficult to analyze: for the largest, cutting-edge models, this has not even been fully achieved. 
* **They are unpredictable.** Being so opaque, it is hard to predict a NN-based model will be biased or wrong, or when they will fail outright, and fixing broken models can require great effort. 
* **The benefits were seen as limited.** Deep learning models results were not perceived to be significantly better than what could be done with other (traditional, predictable) methodologies.

### So what changed?
NNs get much more powerful when you allow them to get bigger and more complex, and as the data you train them on gets bigger and richer. 
With the progress of computing power and technology (notably, the use of graphics cards (GPUs) to perform massive parallel computations) 
and the growth of data sets, various breakthroughs occurred that brought attention to NNs from a wider audience: 
in 2012, a NN called AlexNet became the world's best image analyzer; 
Google and others made great strides in natural language translation and text categorization (including sentiment analysis).
The drawbacks of cost, opacity, and unpredictability remained, but the achievements made the costs justifiable
and greater investment ensued. The hits kept coming: 
in 2015, DeepMind, eventually purchased by Google, became the world's best player of the complex strategy game Go, 
shocking fans of the game across Asia and the world; 
DeepMind went on to crack protein folding in 2020, ending an annual competition of top researchers within two years of its entry. 

### LMs to LLMs
Meanwhile, researchers at Google, OpenAI, and other companies and academic institutions made steady progress in various text-analysis 
and prediction models. 
Of these, the idea of a Language Model, which dates back to the 1930s, is the most abstract, and, as it turns out, very powerful. 
An LM is a word-guesser that can guess the correct next word in a sentence (or a “masked,” or hidden, word), 
drawing its “model” from a text on which it has been trained. 
For LMs, the size of the corpus and the depth and number of parameters in the model is a game-changer: 
whereas a 1000-parameter model trained on a small corpus such as all of Shakespeare’s plays can creates silly play 
that looks and sounds like Shakespeare but is ultimately nonsensical; 
Increasing the training data set to all of Wikipedia and increasing the number of parameters to 1 billion enables the training of a model 
that successfully generates meaningful paragraphs of text: syntactically correct and grounded in a basic knowledge of facts of the world, 
a “large” LM, or LLM. 

### Diffusion models and image generation
At the same time, advancements at the intersection of text and speech generation enabled the development of Stable Diffusion, 
a NN-like model that trains on images and descriptive text, contrasting between similar images such as “a dog on a field with a girl” and 
“two dogs on a couch with a man” or “Monet painting of a flower” and “Titian painting of a war scene”. 
Large networks of extremely powerful GPUs allowed the training of sophisticated versions of these models. 
Once the models reached a certain level of sophistication and accuracy, their power became clear:
Correct-word-guessing (LLMs) can be engineered into “correct answer guessing”, which forms the core of a fully automated chatbot or 
“AI agent” that pulls from outside resources to answer questions and/or perform tasks. 
Image generation with SD can create photorealistic pictures based on a simple description, 
or copy the style of different artists. Visual creativity can be leveraged or even replaced by AI for some purposes.

## So why are things still moving so fast?

After all this incredibly rapid development, the capabilities of LLMs and SD are so rich that there are all kinds of promising applications, 
and it will be a long time before many of the basic uses are worked out. 
Contrary to popular belief, ChatGPT (GPT-3.5 or 4) is but one of many available systems, and many, unlike GPT-3.5, can be customized (or “fine-tuned”) for specific purposes, or on additional text. Finetuning can be used to create a chatbot that responds to certain questions/prompts in specific ways, or to add knowledge of a specific corpus. Finetuning, either unsupervised or scored by humans, is a whole world of customization within the model itself. 
Retrieval Augmented Generation (RAG) allows LLMs to pull from outside sources (for example: Google, a database, or a continuously-updated document store).
Chain-of-Thought reasoning “helps” the LLM generate better answers by guiding it with general methodologies that in practice improve its reasoning or approach to certain tasks.
Prompt-engineering (of which RAG and CoT are two powerful forms) can, in general, be used to transfer an LLMs grammatical and reasoning abilities and general knowledge to apply to different tasks. For example, LLMs can make great text classifiers if you ask them questions like “is the following sentence about x, y, or z?
Agent behavior describes the ability of an LLM to make executive decisions, and even to execute against those decisions, for example by actuating another resource via an API. 
These represent just four approaches to enhancing the power of LLMs to achieve a range of functional goals. 
