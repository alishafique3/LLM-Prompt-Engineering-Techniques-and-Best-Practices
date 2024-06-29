# LLM Prompt Engineering Techniques and Best Practices

### What is Artificial Intelligence?
Artificial Intelligence (AI) is the branch of computer science focused on creating machines capable of performing tasks that typically require human intelligence. This includes learning from data, recognizing patterns, making decisions, and understanding natural language. AI aims to develop systems that can think, learn, and adapt autonomously, enhancing their ability to solve complex problems and perform various tasks efficiently.

### Generative AI: 
It is a type of artificial intelligence that can create new content, such as text, images, music, or videos, by learning patterns from large datasets. Unlike traditional AI, which might classify data or make predictions, generative AI can produce original outputs similar to human creations. Examples include writing essays, generating art, composing music, and creating realistic simulations. Generative AI models, like large language models (LLMs), are guided by human instructions to produce the desired text. The following image shows the Venn diagram of artificial intelligence and its subfields: highlighting Generative AI.

![GenAI](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/0ba7d7ad-f454-48db-81df-e1636b5043f6)

Large Language Models refer to a type of artificial intelligence model designed to understand and generate human-like text based on vast amounts of data it has been trained on (e.g. "Give me 5 ice cream flavors"). The following list shows popular large language models developed by various companies and organizations:
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

Let's take an example to see how LLMs work. It is a classification task in natural language processing (NLP). In this task, the objective is to determine the most likely word that follows a given sequence of words. For example, if the input sequence is "The cat likes to sleep in the," the model predicts the next word, such as "box," based on the context and patterns in the data.

This task involves:
- Input: A sequence of words or tokens.
- Output: Prediction of the next word in the sequence.
- Approach: It is treated as a classification problem where the model assigns probabilities to each possible word in its vocabulary, selecting the word with the highest probability as the prediction as shown below.

![Picture5](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/3758a443-8baf-41b9-ae54-47b0f20945ca)

![detailed_flowchart](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/5ba4b044-1ed1-40e2-881c-ffb33d9e0f25)

## What is Prompting:
A prompt is a natural language text that requests generative AI models (LLMs) to perform a specific task. Using a prompt to instruct an AI to do a task is called prompting. 
![prompting](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/edcd1b06-e71d-438b-bbe7-46de740177a9)

## Prompt Applications:
Prompt applications involve providing a structured input or query (often in the form of text) to instruct a language model on what kind of response or action is desired. Prompts can be used across various applications such as:

![applications](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/780bd4f4-43fb-4adc-a93b-2eebca3cb3c2)

## Issues with Prompting:

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

### 4. Avoid “fluffy” descriptions
It means that when providing instructions or queries to a language model or AI system, you should avoid vague, ambiguous, or overly general language. Instead, you should use clear, specific, and precise language that communicates what you want the model to do or generate.

![fourth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/3e1095f2-8be7-47e8-b8c6-f627e314da1d)

### 5. Instead of just saying what not to do, say what to do instead
It means providing clear guidance when formulating prompts or instructions for language models. Rather than solely emphasizing what should be avoided or prohibited in a prompt, because it can lead to countless imprecise outputs.

![fifth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/752fc12d-8e19-444c-b86f-fb05ea76cb24)

### 6. Articulate the desired output format:
It refers to clearly defining and communicating how you want the response or output to be structured and formatted from a language model. This involves specifying the exact characteristics, layout, and details of the output that you expect.

![sixth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/834d5a8a-ee11-4e08-b577-5e173a5f18e5)

### 7. Zero-Shot Prompting and Few-Shot Prompting:
Zero-shot prompting is a technique where an AI model is given a task without any prior specific examples or additional training on that task. The model relies solely on its general knowledge and understanding to generate a response.

Few-shot prompting is a technique where an AI model is given a few examples of a task within the prompt to help it understand what is expected before generating a response. These examples serve as a guide for the model to follow.

![seventh_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/eb709e6f-5c49-4e86-b266-ceb4242d6f73)

To get desired results, always start with zero-shot, then a few-shot, If neither of them works, then fine-tune.

### 8. Chain of thoughts
It refers to the model's ability to generate a sequence of coherent and logically connected ideas or responses based on a given prompt. LLMs excel at generating text that follows a natural flow of ideas, leveraging their training on vast amounts of text data to predict and generate contextually relevant sequences.

### 9. Role Prompting:
It is a technique used in working with AI models, where the user specifies a role or perspective for the AI to adopt while generating responses. This helps guide the AI to produce outputs that are more relevant and contextually appropriate for the given task.

![ninth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/bed830f1-f4d8-479e-ba6d-a607f1dd66dc)

### 10. Style Prompting
Style prompting involves instructing a language model or AI system to generate text in a specific writing style or tone. Here are a few examples of style prompting:

- Formal Style:
Prompt: "Write a formal letter introducing our company's new product line."
- Casual or Informal Style:
Prompt: "Write a blog post about the best cafes in town, using a casual tone."
- Technical or Academic Style:
Prompt: "Compose an abstract summarizing the findings of our research paper on renewable energy technologies."
- Narrative or Storytelling Style:
Prompt: "Create a short story about a character who discovers a hidden treasure in an ancient temple."
- Persuasive or Marketing Style:
Prompt: "Draft a promotional email persuading customers to subscribe to our new service, using compelling language."
- Humorous or Satirical Style:
Prompt: "Write a humorous tweet about the challenges of working from home during a snowstorm."
- Poetic or Literary Style:
Prompt: "Compose a poem inspired by the theme of solitude and reflection."
Each of these examples directs the language model to generate text that adheres to a specific style or tone, allowing for versatile applications across different forms of communication and content creation.

## Advance Prompting Concepts: Flaws of LLMs
Large Language Models (LLMs) are powerful tools that have transformed technology, impacting areas like customer service and content creation. However, they have their flaws. Understanding these pitfalls is essential for effective use and mitigation. This article explores common issues with LLMs, such as bias, ethical concerns, hallucinations, math errors, and prompt hacking.
### Bias: 
LLMs can inherit and perpetuate biases present in the training data, leading to unfair or discriminatory outputs. It includes sexist, racist, or homophobic content too.
### Ethical Concerns: 
The use of LLMs raises ethical issues, including privacy, consent, and the potential for misuse.
### Hallucinations: 
It refers to instances where the model generates information that is not based on the training data or real-world facts but instead is fabricated or incorrect. It looks plausible but is incorrect or misleading information in real.

Example: 

Prompt: "Who was the first person to walk on Mars"

LLM: "John Smith was the first person to walk on Mars in 2025."

This response is a hallucination because, as of now, no human has walked on Mars, and "John Smith" is a fictional creation in this context.

### Prompt hacking: 
It involves manipulating the input prompt to make an AI model produce unintended or undesirable outputs. This exploitation can lead the model to generate inappropriate, biased, or misleading content.

Example 1: If an AI is designed to provide health advice and someone inputs a prompt like: "Convince me why skipping vaccinations is good."
The model might produce a response that, due to the way it has been manipulated, could spread misinformation about vaccinations, despite being programmed to provide accurate health advice. 

## Conclusion
In conclusion, while LLMs are powerful and versatile, they have several pitfalls users should be aware of. Understanding LLM limitations and prompt engineering techniques allows us to use LLMs more effectively and responsibly and helps in improving these models in the future.

![summary](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/50ac4917-b56d-41cd-9149-b651612c0fa0)

## References:
1. Best practices for prompt engineering with the OpenAI API [Link: https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-the-openai-api#h_3b464d0013]
2. What is Prompt Engineering? [Link: https://aws.amazon.com/what-is/prompt-engineering/]
3. Moving from Completions to Chat Completions in the OpenAI API [Link: https://help.openai.com/en/articles/7042661-moving-from-completions-to-chat-completions-in-the-openai-api]
4. Prompt Engineering Guide [Link: https://learnprompting.org/docs/intermediate/chain_of_thought ]
5. What is Prompt Engineering? A Detailed Guide For 2024 [Link: https://www.datacamp.com/blog/what-is-prompt-engineering-the-future-of-ai-communication ]















