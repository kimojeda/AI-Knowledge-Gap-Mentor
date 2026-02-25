# AI-Knowledge-Gap-Mentor
Agent designed to bridge the digital divide by identifying technical gaps and providing personalized learning paths.

> **Note:** The source code and tool logic are implemented in **Spanish** to better serve Spanish-speaking professional profiles.

Integrated Tools:
- Skill Gap Analyzer: Performs a technical analysis to identify missing AI concepts and libraries based on user profiles.
- Expert Knowledge Retriever (RAG): Consults official PDF documentation with HyDE optimization.
- Deep Expert Hunter: Uses Tavily to find and summarize the top 3 web resources and documentation.
- YouTube Hunter: Filters and retrieves the most relevant practical video tutorials.
- Project Architect: Designs a custom project proposal that connects the user's professional background with new AI skills.

Key Features:
- LangGraph orchestration
- MemorySaver
- Integrated with OpenAI for reasoning and summarization

Dependencies:
- langchain-openai
- langgraph
- tavily-python
- youtube-search

Advanced RAG Integration
The mentor now includes a Retrieval-Augmented Generation (RAG) pipeline to provide academic-grade grounding:
- Knowledge Base: Ingests official manuals from UNESCO and the World Economic Forum (WEF) 2025.
- HyDE (Hypothetical Document Embeddings): Enhances retrieval accuracy by generating a "mock" technical answer before searching the vector database.
- Metadata Filtering: The agent can perform scoped searches (e.g., "Only UNESCO sources") and provides precise citations including File Name and Page Number.

**Instructions**
1. Prerequisites
Ensure you have Python 3.10+ installed. You will also need active API keys for:
- OpenAI: To power the agent's reasoning.
- Tavily: To perform web searches for technical documentation.

2. Install all required libraries, including LangChain, LangGraph, and search tools:
pip install -r requirements.txt

3. Run the main script to start a conversation with the mentor.
