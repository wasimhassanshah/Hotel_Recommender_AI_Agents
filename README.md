 # Hotel Recommender Agent

This project is a comprehensive Hotel Recommender Agent that integrates advanced frameworks like LangChain and CrewAI to provide intelligent hotel recommendations. It combines data processing, semantic search, and multi-agent orchestration to deliver tailored travel experiences.

# Features
- Data Ingestion: Parses and processes JSON data containing hotel listings.
- Semantic Search: Uses embeddings and vector stores for context-aware hotel searches.
- Multi-Agent Collaboration: Leverages CrewAI to coordinate tasks between agents specializing in hotel search and review.
- Interactive User Interface: Built using Gradio for seamless user interaction.

# How It Works
- 1. Data Preprocessing
Extracts key attributes (e.g., name, price, stars, reviews) from JSON hotel listings.
Serializes hotel information into structured text for further processing.

- 2. Text Splitting and Embeddings
Splits text into manageable chunks using LangChain's RecursiveCharacterTextSplitter.
Encodes text using OpenAI embeddings and stores them in Chroma for efficient retrieval.

- 3. Semantic Search
Implements a retriever from the Chroma vector store to query hotels based on user preferences.
Returns the most relevant results based on embeddings.

- 4. CrewAI for Multi-Agent Orchestration

 **Agents:**
- Travel Expert: Searches for hotels based on user criteria like budget, location, and dates.
- Hotel Reviewer: Evaluates and compares hotels to select the best options.

**Tasks:**
- Search for hotels in the specified location and budget.
- Evaluate the options and provide detailed reviews.
- Crew Process: Orchestrates agents sequentially to accomplish the tasks.

- 5. Gradio Interface
Provides an intuitive interface where users can input travel details (location, dates, budget, etc.) to get hotel recommendations.

# Key Frameworks and Tools

- LangChain: For text processing, embeddings, and vector store integration.
- CrewAI: To manage multi-agent collaboration for complex workflows.
- Chroma: Persistent vector store for semantic search.
- Gradio: To create an interactive web application for users.
- Ollama (Llama 3): Used as the foundational language model for natural language tasks.
- OpenAI API: For generating embeddings.


# Future Enhancements

- Dynamic Task Delegation: Allow agents to dynamically delegate tasks for better efficiency.
- Integration with Booking Platforms: Automate the booking process directly from the recommendations.
- Advanced Filtering: Enable users to filter hotels by amenities, star ratings, and location proximity.
