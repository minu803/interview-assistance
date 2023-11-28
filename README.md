# Interview Assistance
<img src="https://github.com/minu803/interview-assistance/assets/111295624/ee5f3a91-08ce-4004-a95a-f88c5892dee6" alt="interview_assistance" width="800" height="auto"/>

## Overview 
During my job search, I realized the challenge of bridging the gap between knowing answers and confidently articulating my story. I discovered certain strategies to structure my responses, allowing me to share my story more effectively. Also, there wasn’t much tool that could make me feel I was prepared for the interview. This led to the creation of the Interview Prep Tool, not just a mock interview platform, but a personalized guide for enhancing responses and storytelling with confidence and authenticity. Utilizing LLM, this tool simulates real interview scenarios, presents diverse questions, and offers feedback like a 24/7 personal coach. It's tailored to your specific interview preparation needs.

## Langchain

LangChain is a comprehensive framework designed for developing applications powered by language models. It stands out for its ability to create applications that are both context-aware and capable of complex reasoning.

### Context Awareness
- **Integration with Context Sources**: Connects language models to a variety of context sources, such as prompt instructions, few-shot examples, and grounding content.
- **Enhanced Interaction**: Ensures that applications are relevant and precise in their responses and interactions.

### Reasoning Capability
- **Informed Decision Making**: Employs language models for reasoning about responses based on the provided context.
- **Action Determination**: Assists in deciding the most appropriate actions in different scenarios.

### LangChain Templates
- **Deployable Architectures**: A collection of reference architectures, easily deployable for a variety of tasks.
- **Task Specific**: Facilitates quick start on specific application development.

- **ChatPromptTemplate Method**: Represents a structured approach to crafting prompts for conversational AI. This method involves the creation of templates for diverse interaction types, ensuring the AI can effectively handle a broad spectrum of conversational scenarios.

```python
prompt_QA = """
You are a world-class career coach helping students to perform better in the job interview.
The following text contains the basic information about the student profile: {resume} \

The following is the some of the examples of the frequently asked questions: {guideline}; If no guideline is provided, please generate questions based on your judgment \

Based on all the information, please design 10 questions based on the student profile and frequently asked questions." \
```

## In-Context Learning in Language Models

In-context learning is a remarkable feature in large language models such as GPT-3, enabling them to perform tasks based on a few examples, without needing internal adjustments.

### Key Points:

#### How It Works
- **Learning from Examples**: The model interprets and predicts outcomes based on input-output example pairs.

#### Effectiveness and Applications
- **Versatile and Efficient**: Suitable for tasks like sentence completion and question answering.
- **Broad Applications**: Used in various fields, from programming to design.

#### Unique Aspect
- **No Parameter Modification**: Distinguishes itself from typical machine learning as it doesn't involve altering the model's settings.
- **Adaptability**: Despite not being initially trained for example-based learning, these models can effectively adapt to such tasks

## Architectural Overview
![architecutre](https://github.com/minu803/interview-assistance/assets/111295624/68f42036-c3d7-44ab-ad26-b7bdfa4ad40d)

### Resume Upload
- **Function**: Allows the student to upload their resume containing comprehensive background and technical information.

### Sample Questions 
- **Purpose**: Provides a collection of sample questions for reference to prepare for interviews.

### Personalized Question Generation
- **Dynamic Interaction**: The system generates personalized interview questions.

### Question Answering Chatbot
- **Process**: A question is posed to the student, who may respond in writing or verbally using a microphone.
- **Feedback**: The Interview Assistant provides brief feedback after each response.
- **Flow**: This question-and-feedback cycle repeats throughout the interview preparation session.

### Interview Evaluation
- **Analysis**: Utilizes a Large Language Model (LLM) to assess the interview based on chat history and standard interviewer metrics.

## Model Card

### Whisper
- **Description**: Whisper is an automatic speech recognition (ASR) and speech translation model, trained on 680,000 hours of labeled data. It is adept at understanding a range of datasets and domains with no need for additional fine-tuning.

### GPT-3.5-turbo
- **Description**: As a variant in the GPT-3.5 series, GPT-3.5-turbo offers quicker response times while preserving the model's broad capabilities in language understanding and generation. It can process up to 4,096 tokens.

### GPT-4-1106-preview
- **Description**: The latest version of the GPT-4 model, features a context window of 128,000 tokens. It boasts enhanced abilities in instruction following, JSON mode, reproducible outputs, and parallel function execution, with training data current as of April 2023.

### Claude 2.1
- **Description**: Claude 2.1 expands the token context window to 200K, significantly reduces hallucination rates for greater accuracy, and improves comprehension and summarization of complex documents. It also includes API tool use for enhanced interoperability.

## Demo 


