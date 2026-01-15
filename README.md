# Prompt-Engineering-

Working with LLM's -- Large Language Models 

What are LLMs ? 
* LLMs are just an aspect of different AI models that enable them to communicate in human text and make them seem like they possess human intelect, but they work with a vast amount of data that enable them know different text, grammer, speeches and also a sophisticated engine that enable them predict the words that come next at every point in time.
An LLM is a model that uses Generative AI techniques, which are based on Deep Learning and Machine Learning, all of which fall under the umbrella of Artificial Intelligence. We can call them different techniques, ie Machine learning, deep learning, generative AI and LLMs.
  
What is a prompt ?
* Instructions and context provided to an AI for certain tasks

Prompt Engineering ? 
* the practice of developing and optimizing prompts to efficiently use an AI for a certain task

* Note that the only time these LLMs "think" is when they type
* You always want to bias the model towards being more accurate and  effective by asking it for evidence. You could also provide hints to guide the model in it's explanations 

 Some of the features of multi-modality include;
 * Acceptance and generation of text
 * Accept and generate images
 * Browse the internate particularly for information that's past it's cut of date
 * It can execute python code

AI models and their chatbots are 2 very different things. For instance, open AI model, OpenAI(GPT -4) would allow you interact with this model through chatgpt or the PaLM model by google through Bard or Gemini etc

In reality LLMs use Tokens to identify different words. Behind the scenes, it breaks down words into tokens, using a lot of maths and statistics to determine what words are statistically probable to follow your tokens based on what it learnt from it's training data.  


# Inside LLMs
* Parameters --> 
* Layers -->
* Tokens -->
 The more parameter, layers and tokens you feed an LLM, the "smarter" they get.So you'd want to use LLMs with more of these features

## The Reversal Curse 
For LLMs A = B but B != A 
That's what the reversal curse talks about 



# Prompt engineering framework 
* The standard prompt --> A prompt consisting of only a question or instruction

## The set up
* The system message --> A defaut or initial peompt that is provided to the model by it's creator 

* Context --> Look to include additional context it primes the model to think the way you want it to be thinking you want it to
* Managing the token limit of a model is crucial to maintaining the accuracy and cohenrence of the model's outputs
* Chatgpt tends to rememeber information or context given to it at the beginning than at the middle. it's also good at the end but the beginning is just key. Funny enough the human brain tends to behave the same way.
* More context can also become less accuracy so aim to provide context that is required because when large amounts of context is required, be aware there is a greater risk of inaccuracies


# Personas amd Role 
* You could consider starting your prompt with things like "You are a senior programer or expert lawyer" etc followed by the actual task that you want it to do. Personas help the model give you more accurate outputs, additional context and they make LLMs more intuitive (and engaging) to interact with. Consider giving personas a unique tone, style and voice, again for more context!  


 # Techniques Of Prompting 
 * Chain of thought prompting --> Improves the performance of LLMs by explicitly prompting the model to generate a step by step explanation or reasoning process before arriving at the final answer. This method helps the model break down the problem and not skip any intermediate tasks to avoid reasoning failures


# Data Camp Prompt engineering course
## The anatomy of a prompt 
* Clear --> Relevant context
* Specific --> Avoid unnecessary information
* Open-ended --> Allowing the model to think outside the box  

## Different types of chain of thought Prompting 
* Zero shot --> No structure provided, the LLM solves the problem alone
* One/few shot --> Roadmap of steps the LLM can follow to solve problems


## Limitations of LLMs 
* Biases --> The model presents stereotypes or misinformation
* Hallucinations --> The model confidently states incorrect information
* Overfitting --> The model is only as good as the data it is trained on
Chatgpt has a knowledge cut off, you could simply state "if you don't know the answer and believe this information is after your cutoff date, specify that you don't know". 


# Structuring a Prompt
## Output control techniques (SALT)
* Style --> Define the framework S
* Audience --> Tailoring the content A
* Length --> Brevity or depth L
* Tone --> Mood and feel T

## Evaluating Responses (LARF)
* Logical consistency --> L
* Accuracy --> A
* Relevance --> R
* Factual Correctness --> F

## The power of markdowns
* You can create a more targetted response using things like markdown hastags to indicate different levels of the headers in your prompt, You can also use bold for the text by using double asteriks or underscores for the text you want to highlight, Quotation marks also highlight specific context, delimiters act as a clear seperators for your prompts



# Training Techniques 
* Zero-shot learning -> When you give a tasks without giving examples. It relies on it's own training data for the answers
* One-shot learning -> Give the model an example of what you want it to do once to guide it's response
* few-shot learning -> Arm the model with multiple examples to guide it's respnose. Each example would serve as a building block for the model giving it richer context of what we want.
* Zero-shot(COT) -> Encouraging the model to "think" step by step prompting the model to give us access to it's way of reasoning in the context of a particular task, allowing us to better understand and verify it's conclusions.
* One-shot(COT) -> Teaching the model how to approach problems



# COURSE 2 

## The AI landscape --> They are not different types on the same level because they represent a nested hierarchy of techniques and a specific field of study
* Machine Learning --> A software of AI that enables models to learn patterns from data without explicit instructions.
* Deep Learning --> Recognizes complex patterns like thoes found in computer vision and self driving cars.
* NLP --> Utilizes machine learning techniques to understand and process human language by computers
* LLMs --> Use deep learning techniques to go from a variety of Natural variety of NLP tasks, such as classification, summerization, generation and more.


## Multimodal application of LLMs
* Can process and generate information across diferent data types, such as text, audio, video and images in contrast to multi model which works with one of the modes such as text only


## Building blocks to train LLMs
* Generative pre-training --> LLMs are typically trained using this technique
   * Next word prediction --> A supervised learning technique that trains the model on the input data and it's corresponding output. It predicts the next word in a sentence
   * Masked language modeling --> Involves training a model to predict a masked word that is selectively hidden in a sentence 

### The Transformer Architecture
A neutral network that enables LLMs process an entire sequence of text (like a sentence) in parallel, rather than sequentially like older models.


# LLMs in the business world 
* Microsoft's copilot
* khan academy's khanmingo
* Bloomberg's BloombergGPT

# Use cases of LLMs 
* Data Transformation
* Natural Language Interface
* Workflow automation
* Copilots and Assistants
* Autonomous Agents

Look into the Open Workd Application Security Project(OWASP) --> To see how the challenges with LLMs are being mitigated 

## The four part framework for prompting AI 
1. Ask --> The core request of what you want, eg explain this for me
2. Requirements --> These are your specific constraints and prefernces, eg Number of paragraphs, what to focus on and what to avoid.
3. Context --> The background information thats going to shape how how the task should be done
4. Example --> Showing what "good" looks like. The whole idea is not to leave any room for the AI to guess.
Remember, AI is capable but context blind. It literally doesn't know anything about what you want to do.


## More Limitations of AI
1. Knowledge fabrication --> Also known as hallucination, when false information is confidently presented as correct
2. Recency Ignorance --> Also known as knowledge cut off date, this is the date limit on the model's knowledge of events
3. Biased outputs --> Reflect and amplify social bias from it's training date
4. Sycophantic outputs --> Telling you what it thinks you want to hear, it would readily validate your perspective and support your decisions
5. Privacy and data Exposure --> Information shared with AI may not stay private 


# Understanding chatgpt
* Chatgpt uses generative Ai to respond to users and generative Ai is a subset of artificial intelligence and machine learning where a model creates new content based on patterns in information it has already seen. 




# Machine learning 
A set of tools for making inferences and predictions from data

## Types of Machine learning 
* Reinforcement learning --> Used for deciding sequencial actions, like a robot deciding it's next path or it's next move in a chess game. It uses complex mathmatics like game theory
* Supervised learning --> Training data is labeled
* Unsupervised learning --> Training data only has features, it is useful for anomaly detection, clustering eg dividing data into groups

## Machine learning workflow
1. Extract features --> choosing features and manipulating the dataset
2. Split dataset --> Train and test the dataset
3. Train model --> Input train dataset into a machine learning model
4. Evaluate --> If the dersired performance isn't reached: tune the model and repeat step 3

A. Supervised learning: "Learning with a Teacher" --> The model is trained on labeled data, which means the input comes with the correct answer (the label) attached. The goal is for the machine to learn the relationship between the data and its label so it can predict labels for new, unseen data. This has 2 flavors; classification and regression
 * Classification --> Consists of assiging a category to an observation
 * Regression --> Consists of assigning a continious variable 

B. Unsupervised Learning: "Learning on Its Own"
The model is given unlabeled data with no "right answers" provided. The machine must find its own hidden patterns, structures, or groupings within the data without any human guidance. This has 3 flavors;
 * Clutering --> Identifying groups in your dataset. Some clustering models include; K-means, DBSCAN, get ready - "Density-based spatial clustering of applications with noise"
 * Anomaly detection --> All about detecting outliers, some use cases include discover devices that fail faster or last longer, discover fraudsters that manage to trick the system, Discover patients that resist a fatal disease
 * Association --> Consists in finding relationships between obeservations

### Improving Model's performance 
1. Dimentionality reduction --> Reducing the number of features (dimentionality means features)
2. Hyperparameter tuning --> Switching hyperparameter values to get different results 
3. Ensemble methods --> This is a technique that combines several models in order to produce one optimal model


## Deep learning 
Deep learning uses an algorithm called neuron networks, it is a special type of machine learning that can solve complex 




