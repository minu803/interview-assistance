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

Based on all the information, please design 10 questions based on the student profile and frequently asked questions.""" 
```

## In-Context Learning in Language Models

In-context learning is a remarkable feature in large language models such as GPT-3, enabling them to perform tasks based on a few examples, without needing internal adjustments.

### How It Works
- **Learning from Examples**: The model interprets and predicts outcomes based on input-output example pairs.

### Effectiveness and Applications
- **Versatile and Efficient**: Suitable for tasks like sentence completion and question answering.
- **Broad Applications**: Used in various fields, from programming to design.

### Unique Aspect
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

[![thumbnail](https://github.com/minu803/interview-assistance/assets/111295624/aeebf819-36f3-4a08-9655-6df4cbe6d8b2)](https://www.youtube.com/watch?v=fonkG16kTX0&ab_channel=MinwooSohn)

## Testing Approach

I selected three questions from the list for evaluation:

- 'Give me an example of when you used logic to solve a problem.'
- 'Explain a time when you took the initiative on a project.'
- 'Describe how you used your problem-solving skills to benefit a team or company.'

In my research, I discovered the STAR interview technique along with numerical methods for scoring responses. The STAR method is a structured manner of responding to a behavioral-based interview question by discussing the specific Situation, Task, Action, and Result of the situation. It's a way to organize your answer to detail not just what you did, but how you did it and the outcome of your actions. This method is beneficial because it allows the interviewer to get clear, concise, and ordered understanding of your experience and how you handle situations in the workplace. Scores were assigned based on the following criteria:

- **1/5**: The response completely missed the question or was inadequate.
- **2/5**: A poor or incomplete response that had some good elements.
- **3/5**: An adequate response that addressed the main points of the question but did not elaborate.
- **4/5**: A strong response that exceeded the basic requirements of the question.
- **5/5**: An excellent response that perfectly aligns with what was sought.

Using this framework, I prepared answers for each question based on my experiences across the numerical spectrum for testing purposes. These responses were then evaluated using the interview assistance application to assess the quality of the feedback. A more detailed list of questions and their answers can be found:

https://docs.google.com/spreadsheets/d/10e91UcLoQtQv6VaELZlrPrxxWrLataqGiFoYuZ3fql0/edit?usp=sharing

For a more nuanced analysis of the answers and evaluations, I selected responses with scores of 1, 3, and 5 during testing. Additionally, I utilized ChatGPT 3.5, GPT-4, and Claude 2 in the testing process.


The result average score for each score category is displayed in the table below. 

| Score    | GPT 3.5 | GPT 4 | Claude 2 |
|----------|---------|-------|----------|
| Score 1  | 1.33    | 1.33  | 1.00     |
| Score 3  | 3.67    | 2.67  | 3.33     |
| Score 5  | 4.33    | 4.00  | 4.33     |

The complete AI evaluation is available at:

https://docs.google.com/document/d/1Q6_3s46wgrV_kvLkhPZz8D8lRWx0rCNLEQnKSAlVwuM/edit?usp=sharing

## Critical Analysis

### GPT-3.5 Evaluation
#### Depth of Analysis
- Responses are often shallow and miss the point.
- Lacks specific examples when needed.

#### Feedback
- Suggests a need for more detailed responses.
- Emphasizes the importance of concrete examples and logical analysis.

### GPT-4 Evaluation
#### Depth of Analysis
- Shows deeper understanding and provides detailed, relevant examples.
- Responses align well with question expectations.

#### Feedback
- Encourages refining response depth and specificity.
- Acknowledges higher quality responses compared to GPT-3.5.

#### Overall Differences
- **Response Quality**: More sophisticated and contextually relevant responses.
- **Specificity and Detail**: Better at providing specific and detailed answers.
- **Question Generation**: Tailors questions based on resume, unlike GPT-3.5's minor tweaks.
- **Feedback**: Follows a more structured format in feedback and correctly handles the number of questions.

### Claude 2 Evaluation
#### Overview
- Utilizes the longest context window without extra coding or templates.
- Conversations are text-based, with no voice recording feature.

#### Low Ratings
- **Issue**: No specific examples or demonstration of key competencies.
- **Advice**: Recommended to use the STAR method for more effective responses.

#### High Ratings
- **Strengths**: Shows logical analysis, problem-solving, and initiative.
- **Achievements**: Effective in data analysis and applying statistical methods.
- **Praise**: Noted for technical, strategic, and leadership skills with impactful results.

#### Comparison with GPT-4
- **Focus**: More direct application to real-world professional scenarios.
- **Problem-Solving**: Both Claude and GPT-4 provide strong problem-solving examples.

### Future work
- **Systemic Metrics Development**: Explore more systematic metrics for evaluation. Consult with a career coach to understand nuanced differences in interview responses. Aim to establish criteria that differentiate good, great, and excellent answers, recognizing the subtle distinctions between them.

- **Language Model Exploration**: Experiment with various language models including LLama 2 and Mistral 7B, utilizing Langchain for implementation. This is to assess the effectiveness of different models in understanding and grading nuanced interview responses.

## Resources
- Birt, J. "How to use the STAR interview response technique." Indeed. [Link](https://www.indeed.com/career-advice/interviewing/how-to-use-the-star-interview-response-technique)
- Indeed Editorial Team. "Interview matrix scoring (With Template and Example)." Indeed. [Link](https://www.indeed.com/career-advice/interviewing/interview-matrix-scoring)
- "Introduction." Langchain. [Link](https://python.langchain.com/docs/get_started/introduction)
- "Quickstart." Langchain. [Link](https://python.langchain.com/docs/get_started/quickstart)
- Xie, S. M., & Min, S. (2022, August 1). "How does in-context learning work? A framework for understanding the differences from traditional supervised learning." SAIL Blog. [Link](https://ai.stanford.edu/blog/understanding-incontext/#the-mystery-of-in-context-learning)

