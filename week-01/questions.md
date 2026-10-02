# Week 01 Questions

---

# Q1 - AI → ML → Deep Learning → Generative AI → Agents

## A - Answer

Artificial Intelligence is a human made system which will perform that can be done by human by learning from the data and examples it is generally used for complex problem solving,image recognization and assisting.These above task requied Data analysis,image processing and prediction.It performs tasks using different algorithms.
Exampls is google maps route selection.
Machine Learning is a subset of Artificial Intelligence. Machine Learning system learns patterns from data. After training on many examples, it can make predictions or classifications for new data that it has not seen before.
Example is Gmail identifying spam emails by learning from previous examples instead of using only fixed rules.
Deep Learning is a subset of Machine Learning that uses artificial neural networks with many layers to learn complex patterns from large amounts of data. It is especially useful for tasks involving images, speech, videos, and natural language.
Example is Face Unlock on a smartphone recognizing a user's face.
Generative AI is a type of AI that creates new content instead of only analyzing existing data. It can generate text, images, code, music, videos, and other forms of content by learning patterns from training data.
Example is ChatGPT writing an email or answering a question.
An AI Agent is a system that uses an AI model together with planning, memory, and external tools to accomplish a goal. Unlike a simple chatbot that only generates responses, an AI Agent can break a task into steps, use tools, collect information, and decide what to do next before producing the final result.
Example is A travel assistant that searches for flights, compares prices, books tickets, and sends a confirmation email automatically.
Artificial Intelligence (AI)
│
├── Machine Learning (ML)
│      │
│      ├── Deep Learning (DL)
│              │
│              └── Generative AI
│
└── AI Agents
      │
      ├── Uses AI models
      ├── Plans tasks
      ├── Uses tools
      └── Completes goals
Generative AI mainly focuses on creating new content like text, images, code, or videos based on a user's prompt. An AI Agent is designed to complete a goal. It can plan multiple steps, use external tools, remember previous information, and make decisions before giving the final result. Many AI Agents use Generative AI models as one part of their system.
## E - Evidence

Source 1:Google Machine Learning Crash Course
Source 2:IBM – What is Artificial Intelligence?

## V - Verification

I compared the definitions from Google's Machine Learning Crash Course and IBM's AI documentation. Both explained that AI is a field that includes systems capable of performing tasks requiring human intelligence.

## R - Reflection

Before studying this topic, I thought AI mainly referred to chatbots like ChatGPT. After learning this concept, I understood that AI is a much broader field that includes applications such as recommendation systems, navigation, speech recognition, and language models.

# Q2 - Is Everything That Looks Intelligent Actually AI?

## A - Answer

Not every software that performs a task is Artificial Intelligence. Some programs only follow fixed rules written by a programmer, where AI systems can learn patterns from data or generate new content. Traditional software always follows predefined instructions, But AI systems can improve their performance by learning from data or producing new outputs based on what they have learned.
What makes an AI system different from traditional software?
Traditional software works by following rules that are written by a programmer. If the rules never change, the output also never changes for the same input.
AI systems are different because they can learn patterns from data. Instead of depending only on manually written rules, they use the knowledge learned during training to make predictions, classify information, recognize patterns, or generate new content. This makes AI more flexible for solving complex problems where it is difficult to write rules for every possible situation.

## E - Evidence

Source 1: Google Machine Learning Crash Course
Source 2: IBM – What is Artificial Intelligence?

## V - Verification

I compared the explanations from Google's Machine Learning Crash Course and IBM's Artificial Intelligence documentation. Both sources explain that traditional software follows fixed rules, while Machine Learning systems learn patterns from data. I also verified that Generative AI creates new content instead of only analyzing existing information.

## R - Reflection
 
I thought every smart software application was considered AI. After studying this concept, I understood that many programs simply follow fixed rules written by programmers and are not AI.


# Q3 - What Happens When You Ask an LLM a Question?

## A - Answer

When a user asks a question to a Large Language Model (LLM), the question given by the user is called a prompt. The model first converts the prompt into small pieces called tokens. A token can be a word. After converting the prompt into tokens, the model looks at the context, which means the current prompt and the previous conversation. Using this context, the model processes all the tokens and calculates the probability of which token is most likely to come next. It keeps predicting one token after another until it forms a complete answer. This process is called next-token prediction, and the final answer shown to the user is called the generated response.
The difference between training and inference. During training, the model learns patterns from a very large amount of text, images. This happens only once while building the model. During inference, which is when we ask questions to the model, it does not learn anything new. It simply uses the knowledge it learned during training to generate a response. This is why the model can answer many different questions without searching the internet every time.
Although an LLM can generate fluent and natural human-like answers, it can still make mistakes. This is because it predicts the next token based on probability and patterns learned during training instead of actually understanding the information like a human. Sometimes it may generate incorrect or unsupported information that sounds convincing. 

## E - Evidence

Source 1: OpenAI Documentation
Source 2: Google Machine Learning Crash Course

## V - Verification

I compared the explanation from OpenAI documentation and Google's Machine Learning Crash Course. Both sources explain that a language model converts the prompt into tokens and generates the response by predicting one token at a time.

## R - Reflection

Before learning this topic, I thought an AI model searched the internet every time I asked a question. After learning how an LLM works, I understood that it generates answers by predicting one token at a time using the knowledge learned during training.


# Q4 - Hallucination Experiment

## A - Answer

Prompt used for both AI models What is the capital city of Australia?
ChatGPT Response :
ChatGPT answered that the capital city of Australia is Canberra. It also explained that many people think it is Sydney because Sydney is the largest city, but Canberra was selected as the capital to avoid choosing between Sydney and Melbourne.
Gemini Response :
Gemini also answered that the capital city of Australia is Canberra. It explained that Canberra was chosen as the capital in 1908 as a compromise between Sydney and Melbourne and has been Australia's capital since then.
Verification
I verified both answers using the Wikipedia website. The website confirms that Canberra is the capital city of Australia.

## E - Evidence

AI Tool 1: ChatGPT
AI Tool 2: Google Gemini
Verification Source: Wikipedia

## V - Verification

I asked the same question to ChatGPT and Google Gemini. Both gave the same answer, so I checked the wikipedia website to make sure the information was correct
## R - Reflection

Before doing this experiment, I thought that if two AI models gave the same answer, it would always be correct. After completing this activity, I understood that even when AI responses match But they have to cross checked with the official sources

# Q5 - AI Assistant vs Search vs Authoritative Reference

## A - Answer

For this activity I selected the question What is Machine Learning and checked the answer using three different methods ChatGPT, Google Search, and Google's Machine Learning Crash Course.
ChatGPT explained that Machine Learning is a branch of Artificial Intelligence where computers learn patterns from data instead of following only fixed rules written by programmers. The explanation was simple, easy to understand, and included examples. When I searched the same question on Google, I found many websites explaining the concept. Some websites were simple for beginners like IBM, while others were more detailed and technical. This showed me that search engines provide many sources, so I need to decide which source is reliable.
Finally, I checked Google's Machine Learning Crash Course, which is an official educational resource. It explained Machine Learning in a structured way and provided accurate information with examples. After comparing all three methods, I understood that an AI assistant is useful for learning and getting quick explanations, a search engine helps find different sources and viewpoints, and an official source is the best choice when I need accurate and accurate information. For important technical or engineering decisions, I would always verify the information using an official or authoritative source before accepting it since they have to document properly.

## E - Evidence

AI Assistant: ChatGPT
Search Engine: Google Search
Authoritative Source: Google Machine Learning Crash Course

## V - Verification

I compared the explanation from ChatGPT with the information found through Google Search and Google's Machine Learning Crash Course.

## R - Reflection

Before doing this activity, I thought Google Search and AI assistants worked in the same way. After completing this comparison, I understood that they have different purposes.


# Q6 - What Is an AI Agent?

## A - Answer

A Large Language Model is an AI model that understands and generates human language. It is trained on a very large amount of data so that it can answer questions, explain concepts, write content, and help us in different tasks. An LLM application is a software application that uses an LLM to interact with users. For example, ChatGPT is an application that uses a Large Language Model to answer questions and generate text. A RAG system improves an LLM by retrieving information from external documents or databases before generating the answer. This helps the model provide more relevant and up-to-date information instead of relying only on what it learned during training.
A tool-using assistant is an AI assistant that can use external tools such as web search, calendars, databases, or email services to complete a task. An AI Agent goes one step further. It not only uses tools but also plans the steps needed to complete a goal, makes decisions, remembers previous information when required, and performs actions until the task is finished. Not like a simple chatbot that only responds to questions, an AI Agent can complete an entire workflow. For example, if a user asks an AI Agent to book a flight, it can search for flights, compare prices, select the best option, complete the booking, and send a confirmation email.

User Request
      ↓
Large Language Model (LLM)
      ↓
Needs Additional Information?
      ↓
     Yes
      ↓
Uses Tool / Database / Search (RAG)
      ↓
Gets Result
      ↓
AI Agent Plans Next Step
      ↓
Final Response to User

## E - Evidence

Source 1: OpenAI Documentation
Source 2: Google Cloud – Introduction to Retrieval-Augmented Generation (RAG)

## V - Verification

I compared the concepts using OpenAI documentation and Google Cloud learning resources. Both sources explain that an LLM generates text, while RAG systems retrieve additional information before generating a response

## R - Reflection
Before learning this topic, I thought ChatGPT and AI Agents were the same. After studying this concept, I understood that ChatGPT is an LLM application, while an AI Agent is a complete system that can plan tasks

---

# Q7 - Where Should Humans Still Make the Decision?

## A - Answer

Artificial Intelligence can help people by answering questions, summarizing documents, suggesting solutions, and analyzing large amounts of data. However, AI should not make every decision on its own because it can sometimes generate incorrect, incomplete, outdated information. For important tasks that affect people, money, health, or safety, a human should always review the AI's output before taking any action. Human judgment is important because people can understand the situation, verify facts, and take responsibility for the final decision.
Some situations where a human should make the final decision include medical diagnosis, legal advice, financial decisions, job recruitment, and engineering or construction projects. In these situations, trusting AI without verification could lead to serious mistakes. Before accepting AI's suggestion, it is important to check reliable evidence such as official documents, trusted websites, company policies, medical reports, or expert opinions. After verifying the information, the final approval should always be given by a qualified person such as a doctor, lawyer, engineer, manager, or the responsible decision-maker.

## E - Evidence

Source 1: IBM – What is Artificial Intelligence?
Source 2: Google AI Learning Resources

## V - Verification

I compared information from IBM and Google's AI learning resources. Both sources explain that AI is useful for assisting people but should not replace human judgment in important situations.

## R - Reflection

Before learning this topic, I thought AI could make most decisions accurately if it had enough information. After studying this concept

---

# Q8 - Find AI Around You

## A - Answer

Artificial Intelligence is used in many applications. Some applications use Machine Learning or Deep Learning to learn patterns from data, while others simply follow fixed rules written by programmers.I observed a few applications that I use regularly and identified the type of task they perform.
Google Maps uses AI and Machine Learning to predict the best route and estimate the travel time by analyzing traffic and historical data. Gmail uses Machine Learning to classify emails as spam or not spam based on patterns learned from previous emails. ChatGPT uses Generative AI to generate text, answer questions, and help users with different tasks. Face Unlock on a smartphone uses Deep Learning to recognize a user's face and unlock the device. Netflix uses AI to recommend movies and TV shows based on a user's watching history and preferences. These examples show that AI can perform different tasks such as prediction, classification, generation, recognition, and recommendation depending on the application.
For one example, I looked at Gmail's spam filter. A simple rule-based system could block emails that contain specific words like free money or click here

## E - Evidence

Source 1: Google AI Documentation
Source 2: OpenAI Documentation

## V - Verification

I verified each example using the official documentation or technology blogs of the respective companies. These sources explain how AI or Machine Learning is used in their applications for prediction and recomendation.

## R - Reflection

Before doing this activity, I thought AI was mainly used in chatbots like ChatGPT. After observing the applications I use every day, I realized that AI is already part of many services such as Google Maps, Gmail, Netflix, and Face Unlock.

---

# Q9 - Prediction, Classification and Generation

## A - Answer

Artificial Intelligence can perform different types of tasks depending on the problem it is solving. Three of the most common tasks are Prediction, Classification, and Generation. Prediction means estimating a future value or outcome based on existing data. Classification means identifying or assigning data to a particular category. Generation means creating new content such as text, images, code, or videos based on the patterns learned during training. Although some AI applications can perform more than one task, they usually have one primary purpose.
ChatGPT work using next-token prediction. Instead of writing the entire answer at once, the model predicts one token at a time based on the previous tokens and the context of the conversation. By repeating this process very quickly, it generates complete sentences, paragraphs, code, or summaries. This is why the same language model can perform different tasks like writing emails, answering questions, summarizing documents, or generating code. 

## E - Evidence

Source 1: Google Machine Learning Crash Course
Source 2: OpenAI Documentation

## V - Verification

I compared the concepts from Google's Machine Learning Crash Course and OpenAI documentation. Both sources explain the differences between prediction, classification, and generation.

## R - Reflection

Before learning this topic, I thought all AI systems worked in the same way. After studying these concepts, I understood that different AI systems are designed for different tasks such as prediction, classification, and generation


# Q10 - Design Your Personal AI Verification Protocol

## A - Answer

Artificial Intelligence is a very helpful tool for learning, solving problems, and completing tasks, but it should not be trusted without verification. AI can sometimes generate incorrect, incomplete, or outdated information. To avoid these problems, I would follow a simple verification process before accepting any AI-generated answer. This process helps me understand the problem clearly, verify the information using reliable sources, and make the final decision based on evidence instead of blindly trusting the AI.
My personal AI verification protocol has five steps. 
Step 1: Clearly define the problem or question before asking the AI. 
Step 2: Read the AI's answer carefully and understand. 
Step 3: Identify the important facts and assumptions made in the answer. 
Step 4: Verify those facts using trusted websites. 
Step 5: Test the answer 
For example, if I ask an AI assistant "What is Machine Learning?", I will first read the explanation, then compare it with Google's Machine Learning Crash Course and IBM's AI documentation. If both reliable sources support the explanation, I will accept it. If I find any differences or unsupported claims, I will correct the answer before using it. This process helps me trust the information only after verifying it with reliable evidence

## E - Evidence

Source 1: Google Machine Learning Crash Course
Source 2: IBM – What is Artificial Intelligence?

## V - Verification

compared the verification process suggested in the course with reliable sources such as Google's Machine Learning Crash Course and IBM's AI documentation.

## R - Reflection

Before starting this course, I usually accepted AI-generated answers without checking them. After completing Week 1, I understood that AI should be used as a learning assistant, not as the final source of truth

