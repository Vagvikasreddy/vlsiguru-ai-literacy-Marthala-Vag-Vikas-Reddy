# Week 01 Questions

---

# Q1 - AI → ML → Deep Learning → Generative AI → Agents

## A - Answer

Artificial Intelligence is a human made system which will perform that can be done by human by learning from the data and examples it is generally used for complex problem solving,image recognization and assisting . These above task requied Data analysis,image processing and prediction . It performs task using different algorithms. 
For example, Google Maps route option. Machine Learning refers to a subset of Artificial Intelligence . 
Machine learning systems learn from patterns in data. It is trained on lots of samples and can then generalize to make predictions or classifications on new data it has not seen before. 
For instance, Gmail detects spam by learning from past samples, not just by employing predefined rules. 
Deep Learning is a subfield of Machine Learning that uses artificial neural networks with several layers to learn complicated patterns from massive quantities of data . It is especially effective for assignments incorporating photos, sounds, videos and natural language. An example is Face Unlock on a smartphone that recognizes a user’s face. Generative AI is a form of AI that creates new content, rather than analyzing current data. It can learn patterns from training data to generate text, images, code, audio, movies and other kinds of content. Example is ChatGPT writing an email or answering a question. 
An AI Agent is a system that combines an AI model with planning, memory, and external tools to achieve a purpose. An AI Agent is not just a simple chatbot that generates responses. It may break down a process into steps, use tools, gather information, and decide what to do next before delivering the final output. 
A travel assistant that looks for flights, compares costs, bookings tickets and automatically sends a confirmation email. 

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

The definitions came from Google’s Machine Learning Crash Course and IBM’s AI material that I used. They both said AI is a branch of study concerned with systems that can do things that need human intelligence

## R - Reflection

I believed this was mostly chatbots like ChatGPT before I researched this topic. I came to know this concept and it struck me that AI is a far larger field with applications like recommendation systems, navigation, speech recognition and language 

# Q2 - Is Everything That Looks Intelligent Actually AI?

## A - Answer

Not all software that does something is Artificial Intelligence. Artificial intelligence systems are able to learn patterns from data or develop new material . Some programs just obey fixed rules written by a programr . Traditional software is built on pre-defined instructions, but artificial intelligence systems learn from data to enhance their performance or generate new outputs based on what they have learnt. What’s the difference between an AI system and regular software? Traditional software is rule-based – that is, rules written by a programmer. If the rules don’t change, the output never changes for the same input. Artificial intelligence systems are unique in that they can learn from data. Instead of only manually set rules, they leverage the knowledge obtained during training to make predictions, classify information, recognize patterns, or generate new content. This makes AI more adaptable to deal with complicated issues where it is hard to set rules for every case.

## E - Evidence

Source 1: Google Machine Learning Crash Course
Source 2: IBM – What is Artificial Intelligence?

## V - Verification

I compared the explanations from Google's Machine Learning Crash Course and IBM's Artificial Intelligence documentation. Both sources explain that traditional software follows fixed rules, while Machine Learning systems learn patterns from data. I also verified that Generative AI creates new content instead of only analyzing existing information.

## R - Reflection
 
I thought all clever software apps were known as AI. I studied this topic and realized that many programs are just following predetermined rules written by programmers and are not AI.


# Q3 - What Happens When You Ask an LLM a Question?

## A - Answer

A prompt is the query the user gives to a Large Language Model (LLM). First, the model divides the command into little chunks or blocks called tokens. A word can be a token. The model takes the prompt, converts it into tokens, and then looks at the context, which is the present prompt plus the past conversation. From there the model looks at all the tokens and works out the likelihood of what token is most likely to appear next. It generates a comprehensive answer by making a prediction for one token at a time. This process is termed next-token prediction, and the final answer presented to the user is called the generated response. The distinction between training and inferring. While training the model learns patterns from a very big volume of text images. This occurs only once during model creation. When we do inference, which is when we ask questions to the model, it doesn’t learn anything new. It just applies what it learnt throughout training to make a response. So the model can answer lots of different queries without having to search the internet every time. An LLM can generate replies that are fluent and natural, like those of a person. This is because it is predicting the next token based on chance and patterns it acquired during training and not truly interpreting the material like a human would . It can sometimes produce plausible seeming but incorrect or unsubstantiated information. 

## E - Evidence

Source 1: OpenAI Documentation
Source 2: Google Machine Learning Crash Course

## V - Verification

I compared the explanation from OpenAI documentation and Google's Machine Learning Crash Course. Both sources explain that a language model converts the prompt into tokens and generates the response by predicting one token at a time.

## R - Reflection

Before studying this issue, I imagined that each time I asked a question, an AI model searched the internet. And then I learnt how an LLM works, and I realized that it creates answers by predicting one token at a time based on knowledge it received in training.


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

For this task I chose the topic What is Machine Learning and verified the answer using 3 different ways ChatGPT, Google Search and Google's Machine Learning Crash Course. ChatGPT revealed to me that Machine Learning refers to a field of Artificial Intelligence where computers may learn from data patterns instead of just obeying fixed rules written by humans. There was a clear and understandable explanation with illustrations. When I googled the same question, I got various webpages describing the notion. Some sites were easy for beginners like IBM while some were more complex and technical. This showed me that search engines have various sources, so I need to find out which source is reliable. Finally I looked at Google’s Machine Learning Crash Course, an official learning resource. It described Machine Learning in an organized manner with precise facts and examples. After comparing all three approaches, I realized that AI assistant is great for learning and obtaining short explanations, search engine is useful for finding other sources and opinions and official source is the best option when I require accurate and correct information. For major technical or engineering decisions, I would always check the information from an official or authoritative source before adopting it because they have to record properly.

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

A Large Language Model is an AI model that can comprehend and generate human language. It is trained on a huge quantity of data to answer questions, explain concepts, produce articles and aid us in different jobs. An LLM application is a software application that utilizes an LLM to connect with consumers. One such example is ChatGPT , an application that employs a Large Language Model to generate text and answer questions . A RAG system improves an LLM by gathering information from external documents or databases before producing the answer. This enables the model to deliver more relevant and up-to-date information than the model learnt during training. A tool-using assistant is an AI helper that can execute a task by accessing external tools like web search, calendars, databases, or email services. An AI Agent takes it one step farther. It uses tools, plans the steps needed to reach a goal, makes judgments, remembers knowledge from the past when necessary and takes activities till the work is completed. An AI Agent can perform a full workflow, not only answer queries like a basic chatbot. For example, if a user asks an AI Agent to book a flight, it can search for flights, evaluate costs, choose the best option, complete the transaction and send a confirmation email.

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

Artificial Intelligence can allow individuals to answer queries, summarize papers, propose solutions and analyze big quantity of data. However, not all decisions should be made by AI because it can sometimes produce incorrect, incomplete or outdated information. For crucial jobs that involve people, money, health, or safety, the output from the AI should always be reviewed by a person before acting on it. People can grasp the situation, check the facts and take responsibility for the ultimate decision hence human judgment is crucial. There are some cases when the final choice should be made by a human, for example, medical diagnosis, legal counsel, financial decisions, employment recruitment, and engineering or construction projects. Blind faith in artificial intelligence can lead to significant blunders in such cases. It is a good practice to verify the advice of AI from reliable sources such as official papers, trusted websites, company policies, medical reports, or expert opinions before following them. Once the information has been verified the final permission should come from a qualified person, a doctor, lawyer, engineer, management or the accountable decision maker.

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

Artificial Intelligence is applied in many applications Some apps employ Machine Learning or Deep Learning to learn patterns from data, while others just follow fixed rules programd by humans. I looked at some apps that I use often and figured out what kind of task they are doing. Google Maps employs Artificial Intelligence and Machine Learning to analyze traffic and historical data to forecast the optimal route and estimate journey time. Gmail employs Machine Learning to study patterns in old emails to sort them as spam or non spam. ChatGPT employs Generative AI to generate text, answer questions, and assist users with a range of tasks. A smartphone’s Face Unlock leverages Deep Learning to identify a user’s face and unlock the phone. Netflix employs artificial intelligence to suggest movies and TV series based on the user’s viewing history and likes. The examples above illustrate how standard artificial intelligence may perform a variety of tasks such as prediction, classification, generation, recognition and recommendation depending on the application. For example, I looked at Gmail's spam filter. A rule based system could reject emails that contain certain terms such as free money or click here

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

Artificial Intelligence can do various jobs based on the challenge it is addressing. The three most popular tasks are Classification, Generation and Prediction . Prediction is the process of estimating a future value or event based on available data. Classification is the process of identifying or labeling data to a specific category. Generation is the ability to produce new content (text, graphics, code, video, etc.) depending on the patterns it learnt during training. Some AI programs work on more than one task, but always focus on a primary aim. ChatGPT work with next-token prediction. Instead of outputting the full answer at once, the model predicts the next token one at a time depending on the previous tokens and the conversational context . Repeating this technique very rapidly it generates whole sentences, paragraphs or code or summaries. That is why the same language model may perform many activities such as sending emails, answering queries, summarizing papers or generating code.

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

