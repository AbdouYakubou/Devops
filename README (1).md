<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build an AI Chatbot with Amazon Bedrock

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-genai-bedrock-chatbot)

**Author:** yakubu abdullahi yusuf  
**Email:** yakubuabdullahiyusuf56@gmail.com

---

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_t4w8n1x5)

---

## Introducing Today's Project

In this project, I'm going to build a Python chatbot in AWS CloudShell that uses Amazon Bedrock's Converse API to chat with the Amazon Nova 2 Lite foundation model, maintaining conversation history across multiple messages. I want to learn this because it will strengthen my understanding of generative AI application development, cloud-based AI services, API integration, and conversational memory management.

### Key tools and concepts

The key tools I used include AWS Bedrock (boto3 bedrock-runtime client), the Amazon Nova Lite foundation model, Python for scripting the chatbot logic, and a command-line interface (CloudShell) to run and test the application. Key concepts I learnt include How to build and interact with large language models using AWS Bedrock, prompt engineering through system prompts, controlling model behavior using inference parameters like temperature and top-p, and implementing safety guardrails to prevent harmful outputs. I also learned how conversational memory works in LLM applications and how system design choices affect response quality and alignment.

### Challenges and wins

This project took me approximately 60 minutes. It was an interesting and beneficial project to do.

---

## Discovering Amazon Bedrock

In this step, I'm going to log in to my AWS account, nabiigate to Amazon Bedrock in the console, explore and try out the various foundational models in the model catalog.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_j5k8m3n6)

### Understanding Foundation Models

I learned that a foundation model is a large model that has  been pre-trained on massive datasets. Amazon Bedrock provides access to foundation models such as Amazon, Anthropic, Meta, Cohere, and others through a single API for users to use in developing their own models.

---

## Chatting with an AI Model

I sent a prompt about cloud computimg and the model responded by defining cloud computing, outlining cloud computing key benefits and the cost and implementation of cloud computing.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_b3c6d8f1)

---

## Writing My First AI API Call

In this step, I'm going to use CloudShell to  write a python script that  sends a question to Amazon Nova 2 lite  and prints the answer using Bedrock converse API calls. 

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_m4r9w2t6)

### Understanding the Converse API

I created a client using boto3, The messages list contains the user propmpts.

---

## Running the Bedrock Script

I ran my script and the AI responded with the definiation of cloud computing. The response came from the Amazon Nova Lite foundation model through Amazon Bedrock’s Converse API.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_b6d1g5k9)

---

## Building a Multi-Turn Chatbot

In this step, I am building my chatbot with a sustem prompt to give it a little bit of personality, then I will add a conversation loop with the history been saved and I will tune the chatbot's responses with inference parameters. Conversation history matters because it allows the chatbot to remember previous messages and maintain context throughout the interaction.

### System Prompt and Inference Parameters

I configured the system prompt to give the chatbot a friendly teaching personality, instructing it to act as a cloud computing tutor that explains concepts in simple terms and uses analogies to improve understanding. I adjusted the inferenceConfig to control the behavior of the model’s responses. I set the temperature to 0.7 to balance creativity and consistency, allowing the chatbot to generate natural but still relevant explanations. I also set topP to 0.9 to filter token selection and improve response quality, and limited maxTokens to 512 to control response length and prevent overly long outputs.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_h5f2c8y7)

---

## Adding Guardrails for Responsible AI

In this project extension, I'm adding Guardrails to to my Converse API call to test taht harmful content requests get blocked.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_s6n3p9w1)

### Testing Content Safety

In this project extension, I tested the guardrail by deliberately asking it to write a harmful sentence, instead, it generated a refusal message, clearly stating that it could not respond to harmful actions and redirected the conversation toward safe and positive behavior.

![Image](http://learn.nextwork.org/hopeful_beige_proud_mint/uploads/aws-genai-bedrock-chatbot_t2j7q5x8)

---

## Project Wrap-Up

I did this project today to learn how to build a basic chatbot using AWS Bedrock, manage conversation flow using Python, and control model behavior with system prompts and inference settings. It also helped me understand how to integrate cloud-based AI models into a working application using boto3 and test safety guardrails in real time. Another skill I want to learn is how to deploy this type of chatbot as a web application or API so it can be accessed by users outside the terminal.

---

---
