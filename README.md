###Agentic AI Using AutoGen, Gemini & Gradio

This project demonstrates how to build an agentic AI system using Microsoft AutoGen, Google Gemini models, and a Gradio-based interactive interface. It showcases how multiple intelligent agents can collaborate, communicate, and solve tasks autonomously using large-language-model reasoning.

##Overview

The notebook integrates AutoGen for multi-agent orchestration and Gemini (via ag2) as the primary language model. A minimal Gradio interface enables users to submit queries while observing how agents interact to produce responses. Environment variables are handled through python-dotenv for secure API key management.

This implementation provides a concise example of building agentic workflows, where agents perform coordinated reasoning, planning, and problem solving. It also includes the model configuration, agent initialization, and UI setup required to run a basic agentic system.

##Core Technologies
Library	Purpose
AutoGen (pyautogen)	Multi-agent orchestration and communication
ag2 (Gemini integration)	Wrapper for Google Gemini models
Gradio	Interactive interface for user inputs
python-dotenv	Secure environment variable loading
Google Generative AI	LLM backend (Gemini 2.5 Flash)
Notebook Contents

Gemini model configuration (config_list_gemini)

Environment variable setup

Initialization of AutoGen agents

Communication workflow between agents

Gradio UI setup for interacting with the system

Logic for processing user queries through collaborative agents

How It Works
Model Configuration

The notebook loads API keys through environment variables and prepares a unified Gemini configuration for all agents.

Agent Creation

Two or more agents are defined using AutoGen, each with specific roles such as user proxy, assistant, or reasoning agent.

Agent Collaboration

Agents communicate through AutoGen’s built-in messaging framework, coordinating to produce answers or solve tasks using Gemini responses.

User Interface

A simple Gradio interface allows users to submit prompts and view the final combined output generated through agent communication.

Future Enhancements

Introduce memory-enabled agents

Add tool-executing agents (e.g., code execution, retrieval, external tools)

Expand the number of agent roles such as planner, critic, or executor

Enable persistent logs of agent conversations
