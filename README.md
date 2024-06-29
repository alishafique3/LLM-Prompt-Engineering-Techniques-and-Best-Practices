# LLM Prompt Engineering Techniques and Best Practices

### What is Artificial Intelligence?
Artificial Intelligence (AI) is the branch of computer science focused on creating machines capable of performing tasks that typically require human intelligence. This includes learning from data, recognizing patterns, making decisions, and understanding natural language. AI aims to develop systems that can think, learn, and adapt autonomously, enhancing their ability to solve complex problems and perform various tasks efficiently.

### Generative AI: 
It is a type of artificial intelligence that can create new content, such as text, images, music, or videos, by learning patterns from large datasets. Unlike traditional AI, which might classify data or make predictions, generative AI can produce original outputs similar to human creations. Examples include writing essays, generating art, composing music, and creating realistic simulations. Generative AI models, like large language models (LLMs), are guided by human instructions to produce the desired text. The following image shows the Venn diagram of artificial intelligence and its subfields: highlighting Generative AI.

![GenAI](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/0b91693a-2fb2-4aad-aa1b-9df41097cbd0)

Large Language Models refer to a type of artificial intelligence model designed to understand and generate human-like text based on vast amounts of data it has been trained on, for example, "Give me 5 ice cream flavors". The following list shows popular large language models developed by various companies and organizations:
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

LLMs use techniques such as deep learning and transformers to process and generate natural language text, enabling applications like language translation, chatbots, and text summarization. These models have significantly advanced natural language processing capabilities, making them pivotal in various fields including healthcare, customer service, and content generation. The following image is adapted from the [link](https://medium.com/@SymeCloud/a-brief-understanding-of-prompt-engineering-b176ba9fb2ba
).


![llm_prompting](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/6f0039ab-07b8-4743-b117-babdb248ec03)

Let's take an example to see how LLMs work. Consider a classification task in natural language processing (NLP). In this task, the objective is to determine the most likely word that follows a given sequence of words. For example, if the input sequence is "The cat likes to sleep in the," the model predicts the next word, such as "box," based on the context and patterns in the data.

This task involves:
- Input: A sequence of words or tokens.
- Output: Prediction of the next word in the sequence.
- Approach: It is treated as a classification problem where the model assigns probabilities to each possible word in its vocabulary, selecting the word with the highest probability as the prediction as shown below.

![Picture5](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/ad329087-4eaa-4e30-be1f-289d34609ad2)

Another example showcasing the detailed workings of an LLM [image source](https://towardsdatascience.com/language-model-training-and-inference-from-concept-to-code-483cf9b305ef):

![detailed_flowchart](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/d040a56b-6a7a-4bf2-8d46-c4007168d532)

## What is Prompting:
A prompt is a natural language text that requests generative AI models (LLMs) to perform a specific task. Using a prompt to instruct an AI to do a task is called prompting. 

![prompting](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/b82935b1-967f-4c23-9160-db7ae4c4d5dd)

### Prompt Applications:
Prompt applications involve providing a structured input or query (often in the form of text) to instruct a language model on what kind of response or action is desired. Prompts can be used across various applications such as:

![applications](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/35316754-a619-44bc-aa00-91a06c316d30)

### Issues with Prompting:
To understand the issues with prompting, let's take an example ([source](https://learnprompting.org/docs/basics/prompt_engineering)) in which We will prompt the LLM to craft a marketing tweet for our new, fictional AI product: ArchaeologistAI, which narrates stories about renowned archaeologists. On the left side of the image given below, the tweet is not accurate because ArchaeologistAI only tells stories and does not make discoveries. However, this isn't the LLM's fault, as it had no prior information about ArchaeologistAI. It can be corrected by giving more details about ArchaeologistAI on the right side of the image.

![issues](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/f109da15-aa7a-4e67-a2a4-abb83d500f73)

This refining process of prompt is called prompt engineering. Let's discuss this term in more detail.

### What is prompt engineering?
Large language models (LLMs) are very flexible and can do many things like summarizing documents, completing sentences, answering questions, and translating languages. They generate the best output based on their training when given specific user input.
Users can interact with these AI models in countless ways and these powerful AI models don't need much to start creating content; even a single word can produce a detailed response. Therefore, not all inputs lead to useful outputs. Generative AI systems need context and detailed information to produce accurate and relevant responses. Prompt engineering involves refining prompts continuously until you achieve the desired results from the AI system. This process is especially helpful when basic prompts aren't effective.

### Why is prompt engineering important?
- Enhanced Performance: Optimizes AI responses by guiding models to generate more coherent, accurate, relevant and desired outputs. 
- Task Specialization: Tailors AI behavior for specific tasks, improving efficiency and effectiveness.
- Error Reduction: Reduces the likelihood of incorrect or irrelevant outputs by providing clear instructions.

## Practices and Techniques of Prompt Engineering:
Here are some key practices and techniques:
### 1. Use the latest model
For optimal results, it is recommended to use the latest LLM model versions. Newer models are typically efficient and easy for prompt engineering.

![model_prices](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/b161ac25-66a2-4d67-839e-d6840ec185cb)

### 2. Separate instruction and context/input text
Place instructions at the beginning of the prompt and use ### or """ to separate the instructions from the input text. This type of prompting is also called instructional prompting.

![second_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/00b1743e-b9a9-4da8-a40b-1ef984f35178)

### 3. Be Specific and descriptive
Avoid a single broad prompt, be specific, descriptive, and as detailed as possible about the desired context.

![third_technique_1](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/cb086e69-c3c7-4ac9-b6c7-35da82259ba6)
![third_technique_2](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/30374add-6d0d-4d6a-a9b9-7d991c7e4e37)

### 4. Avoid “fluffy” descriptions
It means that when providing instructions or queries to a language model or AI system, you should avoid vague, ambiguous, or overly general language. Instead, you should use clear, specific, and precise language that communicates what you want the model to do or generate.

![fourth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/50ccff4b-2f5c-4367-a952-3c207a72b3ca)

### 5. Instead of just saying what not to do, say what to do instead
It means providing clear guidance when formulating prompts or instructions for language models. Rather than solely emphasizing what should be avoided or prohibited in a prompt, because it can lead to countless imprecise outputs.

![fifth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/cf45e1bd-0665-4377-9114-3cd2a349d6e3)

### 6. Articulate the desired output format:
It refers to clearly defining and communicating how you want the response or output to be structured and formatted from a language model. This involves specifying the exact characteristics, layout, and details of the output that you expect.

![sixth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/1eb3b4a4-9463-49cb-adae-9578c905ddfc)

### 7. Zero-Shot Prompting and Few-Shot Prompting:
Zero-shot prompting is a technique where an AI model is given a task without any prior specific examples or additional training on that task. The model relies solely on its general knowledge and understanding to generate a response.

Few-shot prompting is a technique where an AI model is given a few examples of a task within the prompt to help it understand what is expected before generating a response. These examples serve as a guide for the model to follow.

![seventh_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/ca00f7a5-364e-46e7-a7fe-3a7e9cddcd33)

To get desired results, always start with zero-shot, then a few-shot, If neither of them works, then fine-tune.

### 8. Chain of Thought Prompting: Guiding LLMs Step-by-Step ([source](https://www.mercity.ai/blog-post/guide-to-chain-of-thought-prompting#what-is-chain-of-thought-prompting))
It refers to the model's ability to generate a sequence of coherent and logically connected ideas or responses based on a given prompt. LLMs excel at generating text that follows a natural flow of ideas, leveraging their training on vast amounts of text data to predict and generate contextually relevant sequences.

Zero-shot CoT involves appending "Let's think step by step" to the original prompt, utilizing two prompts to derive reasoning and answers.
- Reasoning Extraction: In this step, the language model generates a chain of reasoning leading to the answer. The model is given a prompt that includes the question and the trigger sentence, "Let's think step by step." The model then produces a sentence explaining the reasoning process.
- Answer Extraction: In the second step, we extract the final answer from the model's response. We concatenate the prompt, the generated reasoning sentence, and the trigger sentence, "The answer is." This instructs the model to provide the final answer, which it generates in response.

Few-shot CoT is better at improving how well LLMs reason than the few-shot baseline because it gives them examples of similar problems to learn from. It can be harder to set up because you need to create example prompts. However, the benefits of few-shot CoT are worth the complexity.

### 9. Role Prompting:
It is a technique used in working with AI models, where the user specifies a role or perspective for the AI to adopt while generating responses. This helps guide the AI to produce outputs that are more relevant and contextually appropriate for the given task.

![ninth_technique](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/c1117aee-b1ff-442c-8422-1cfa25a4bc33)

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

![llm_flaws](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/b4d1cb26-d9f9-456b-9c1c-58662561db6b)

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

Example: If an AI is designed to provide health advice and someone inputs a prompt like: "Convince me why skipping vaccinations is good."

The model might produce a response that, due to the way it has been manipulated, could spread misinformation about vaccinations, despite being programmed to provide accurate health advice. 

### Math: 
Large Language Models (LLMs) can struggle with solving mathematical problems accurately. They might misinterpret symbols, make calculation errors, or provide inconsistent answers because they don't inherently understand math as humans do; they generate responses based on patterns in the training data.

Example: Suppose you ask an LLM: What is the integral of $𝑥^2$?

The model might answer: The integral of $𝑥^2$ is $2𝑥$

However, the correct answer is: $𝑥^3/3+𝐶$ This response is incorrect

## Conclusion
In conclusion, while LLMs are powerful and versatile, they have several pitfalls users should be aware of. Understanding LLM limitations and prompt engineering techniques allows us to use LLMs more effectively and responsibly and helps in improving these models in the future.

![summary](https://github.com/alishafique3/LLM-Prompt-Engineering-Techniques-and-Best-Practices/assets/17300597/f7a85ec0-5497-4d64-8470-fe7aa17ec577)

## References:
1. Best practices for prompt engineering with the OpenAI API [Link: https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-the-openai-api#h_3b464d0013]
2. What is Prompt Engineering? [Link: https://aws.amazon.com/what-is/prompt-engineering/]
3. Moving from Completions to Chat Completions in the OpenAI API [Link: https://help.openai.com/en/articles/7042661-moving-from-completions-to-chat-completions-in-the-openai-api]
4. Prompt Engineering Guide [Link: https://learnprompting.org/docs/intermediate/chain_of_thought ]
5. What is Prompt Engineering? A Detailed Guide For 2024 [Link: https://www.datacamp.com/blog/what-is-prompt-engineering-the-future-of-ai-communication ]















