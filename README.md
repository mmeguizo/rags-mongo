HR Chatbot with RAG and MongoDB
A TypeScript-based HR chatbot application that uses LangChain, MongoDB Atlas Vector Search, and various AI models for intelligent employee data querying.

Features
Vector Search: Uses MongoDB Atlas Vector Search for semantic similarity matching
Multiple LLM Support:
Groq (Mixtral-8x7b)
Google Gemini
Anthropic Claude (commented)
State Management: Uses LangGraph for conversation state handling
Database Integration: MongoDB for storing employee records and conversation states
RESTful API: Express server with endpoints for chat interactions
Project Structure
index.ts - Express server setup and API endpoints
agent.ts - Core chatbot logic with LangGraph implementation
seed.database.ts - Database seeding script for employee data
Setup
Install dependencies:
Configure environment variables: Create a .env file based on .env.example:
Seed the database:
Start the server:
API Endpoints
GET / - Health check endpoint
POST /chat - Start new conversation
POST /chat/:threadId - Continue existing conversation
Technology Stack
TypeScript
Express.js
MongoDB Atlas
LangChain
LangGraph
Various LLM APIs (Groq, Google Gemini, Anthropic)
Architecture
The system uses a RAG (Retrieval Augmented Generation) architecture with:

Vector embeddings for semantic search
Conversational state management
Tool-based agent system for database queries
MongoDB checkpointing for conversation persistence
