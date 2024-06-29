# LLM Prompt Engineering Techniques and Best Practices

### What is Artificial Intelligence?
Artificial Intelligence (AI) is the branch of computer science focused on creating machines capable of performing tasks that typically require human intelligence. This includes learning from data, recognizing patterns, making decisions, and understanding natural language. AI aims to develop systems that can think, learn, and adapt autonomously, enhancing their ability to solve complex problems and perform various tasks efficiently.

### Generative AI: 
It is a type of artificial intelligence that can create new content, such as text, images, music, or videos, by learning patterns from large datasets. Unlike traditional AI, which might classify data or make predictions, generative AI can produce original outputs similar to human creations. Examples include writing essays, generating art, composing music, and creating realistic simulations. Generative AI models, like large language models (LLMs), are guided by human instructions to produce the desired text (e.g. "Give me 5 ice cream flavors"). The following image shows the Venn diagram of artificial intelligence and its subfields: highlighting Generative AI.

![GenAI](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/8bda3422-8a17-4946-ab72-8791627a539a)

LLM stands for Large Language Model. It refers to a type of artificial intelligence model designed to understand and generate human-like text based on vast amounts of data it has been trained on. The following list shows popular large language models developed by various companies and organizations:
- OpenAI - GPT-4
- Google – Gemini
- Microsoft - Turing NLG
- Facebook (Meta) - LLaMA (Large Language Model Meta AI)
- Anthropic – Claude
- Amazon – AlexaTM
- Baidu – ERNIE
- Cohere - Command R
- IBM - Watson NLP
- Hugging Face - BLOOM (BigScience Large Open-science Open-access Multilingual Language Model)

LLMs use techniques such as deep learning and transformers to process and generate natural language text, enabling applications like language translation, chatbots, and text summarization. These models have significantly advanced natural language processing capabilities, making them pivotal in various fields including healthcare, customer service, and content generation.

![llm_prompting](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/ba3478d8-0879-422b-8dac-1e2cee50a072)

Let's take an example of predicting the next word in a sequence. It is a classification task in natural language processing (NLP). In this task, the objective is to determine the most likely word that follows a given sequence of words. For example, if the input sequence is "The cat sat on the," the model predicts the next word, such as "mat," based on the context and patterns in the data.

This task involves:
- Input: A sequence of words or tokens.
- Output: Prediction of the next word in the sequence.
- Approach: It is treated as a classification problem where the model assigns probabilities to each possible word in its vocabulary, selecting the word with the highest probability as the prediction.

![Picture5](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/3758a443-8baf-41b9-ae54-47b0f20945ca)

![detailed_flowchart](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/5ba4b044-1ed1-40e2-881c-ffb33d9e0f25)

## Prompt Applications:
Prompt applications involve providing a structured input or query (often in the form of text) to instruct a language model on what kind of response or action is desired. Prompts can be used across various applications such as:

- Text Generation: Generating coherent paragraphs, stories, or summaries based on a given prompt.
- Creative Writing: Generating poetry, dialogues, or other creative content.
- Translation: Prompting a model to translate a specific sentence or passage from one language to another.
- Data Analysis: Using prompts to query and analyze datasets or generate insights.
- Customer Service: Generating responses to customer queries or support tickets.
- Programming: Generating code snippets based on a given prompt or task description.

![applications](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/780bd4f4-43fb-4adc-a93b-2eebca3cb3c2)

### 1. Use the latest model
For optimal results, we recommend using the latest LLM model versions. Newer models are typically efficient and easy for prompt engineering.

![model_prices](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/30d96e02-5fb9-48ab-a5f1-29b588459ab2)

### 2. Separate instruction and context/input text
Place instructions at the beginning of the prompt and use ### or """ to separate the instructions from the input text. This type of prompting is also called instructional prompting.

![second_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/5cd54f84-cb5c-4998-ac56-8e6ce06e37b6)

### 3. Be Specific and descriptive
Avoid a single broad prompt, be specific, descriptive, and as detailed as possible about the desired context.
![third_technique_1](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/94d1bf79-0a6d-4cc0-9753-eed4d41156ae)
![third_technique_2](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/bbf0561a-226a-4b41-bf76-260271c6d827)

## 4. Avoid “fluffy” descriptions
It means that when providing instructions or queries to a language model or AI system, you should avoid vague, ambiguous, or overly general language. Instead, you should use clear, specific, and precise language that communicates what you want the model to do or generate.
![fourth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/3e1095f2-8be7-47e8-b8c6-f627e314da1d)








