<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# AI Finance Agent with Amazon Bedrock

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-genai-bedrock-agent)

**Author:** yakubu abdullahi yusuf  
**Email:** yakubuabdullahiyusuf56@gmail.com

---

---

## Introducing Today's Project!

In this project, I will build an AI agent using Amazon Bedrock Agents that reads your spending data, categorizes expenses, calculates budgets, and generates visual charts, I'm doing this project to learn how to build autonomous AI agents using Amazon Bedrock Agents, integrate data analysis workflows into AI applications, process and categorize financial data automatically, and generate actionable insights and visualizations from real-world datasets.

### Key services and concepts

The key tools I used include AWS Bedrock agent which uses code interpreter, Python, Nova Lite foundation model, and a CSV file.
The key concepts I learnt include prompt engineering, foundation model integration, API-based AI application development, conversation context management, inference parameter tuning, and building cloud-based generative AI solutions.

### Challenges and wins

This project took me approximately sixty minutes.The most interesting part was learning how to use clear and consice instructions. It was most rewarding to  learn how cloud, AI and analysis can be used in a single project.

---

## Exploring Amazon Bedrock and Foundation Models

In this step, I am navigating to my AWS account, setting my region, navigating to Amazon Bedrock, finding Amazon Nova 2 lite and previewing it's features.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_w5x8n1q4)

### Understanding foundation models

A foundation model is a large AI model pre-trained on massive amounts of data. Instead of trying to train my own model from scratch, I can access one through an API. We are using Nova 2 Lite because it  is Amazon's lightweight, fast, and cost-effective model, since I am on free tier account, I will be using it.

### Discovering Bedrock Agents

A Bedrock Agent is an AI that can reason through multi-step tasks autonomously, Unlike a chatbot, it can decide what actions to take, execute code, call APIs and iterate on results.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_h4t7y1a5)

---

## Creating the AI Finance Agent

In this step, I will be creating an Amazaon Bedrock Agent which will serve as a personal finance advisor, which I willl also write the agent's natural langugage instructions and enable a code interpreter so the agent can write and execute python code.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_q4j6r2m8)

### Crafting the agent instructions

I wrote instructions that tell my agent to know that it is a personal finance advisor for analyzing spending data, categorize expenses and suggest budgets. This is important because the more clear and specific the instructions are, the better the agents performs.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_f2d8g4l6)

---

## Analyzing Spending Data with Code Interpreter

In this step, I will analyze my finances, one of the main purpose of this project. I will upload a transactions CSV and get a spending summary from my agent. I will also try getting budget recommendations from my agent. 

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_p4r7t9v1)

### How Code Interpreter processed the data

I uploaded a CSV file to code interpreter and gave it the instruction "Use code interpreter to read the uploaded file and calculate total spending by category" The agent used Code Interpreter to calcullate spending by category. The output shows the spending by category as expected.

---

## Iterating on Agent Instructions with Traces

I changed the instructions to "as a Personal finance advisor analyze spending, categorize expenses, suggest budgets, display all dollar amounts with two decimal places, and show each category's percentage of total spending". The output improved by showing the percentage breakdowns of each category.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_q5s8u2w4)

---

## Enabling Cross-Session Agent Memory

In this project extension, I am enabling agent memory with session summarization. Cross-session memory is important because it allows the agent to recall past experiences, observations, and decisions to inform future actions and maintain context over time.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_n5m3k7j1)

### Session summarization vs full history

I configured the the memory section of the agent where i set the Storage duration to 30 days and set the Maximum recent sessions to 5. Summarization is useful because after every session, the agent creates a concise summary of key decisions and topics to use as references in the future sessions,

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-agent_t8h1g5f3)

### Testing cross-session recall

In this project extension, I tested the memory recall of my agent by asking it "Use code interpreter to analyze my spending and give me three specific ways I could save money", then started a new session. In the new session, I asked the agent "What savings tips did you give me last time?" The agent recalled the tips and otlined the tips exactly.

---

## Wrapping Up

I did this project today to learn how to build and deploy conversational AI applications using Amazon Bedrock, integrate foundation models through APIs, and manage conversation context to create more natural and intelligent user interactions.
Another skill I want to learn is how to enhance AI chatbots with external knowledge sources and tools, such as Retrieval-Augmented Generation (RAG), function calling, and agent-based workflows to handle more complex real-world tasks.

---

---
