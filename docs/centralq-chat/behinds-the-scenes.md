CentralQ Chat leverages advanced AI technology and a sophisticated ranking mechanism to deliver accurate and relevant answers to your Business Central queries. Here's an in-depth look at how it works:

### The AI Model

- **Model**: CentralQ Chat uses Azure OpenAI's GPT 3.5 Turbo, a state-of-the-art language model known for its ability to understand and generate human-like text.
- **Context Length**: The model operates within a context window of 4096 tokens. This includes the user's input, system-generated prompts, retrieved information, chat history, and the AI's responses.
- **Balanced Context**: To ensure coherent and relevant conversations, the AI balances the various elements (user input, system prompt, retrieved knowledge, chat history) within the context limit. This means the AI may gradually "forget" earlier parts of the conversation as the dialogue progresses.

### Smart Rephrasing

- **Optimization**: The AI rephrases user queries for clarity and optimal retrieval. This is crucial, as the way a question is framed can significantly impact the search results.
- **Adaptive Queries**: For follow-up questions, the AI considers the entire session's context. This adaptive approach helps maintain the conversation's focus, though it may occasionally lead to misunderstandings if the rephrasing deviates from the user's intent.

### Hybrid Search Approach

- **Keyword and Semantic Search**: CentralQ Chat employs a blend of classic keyword search and modern semantic search techniques. This hybrid model allows the system to understand the query's context and intent, leading to more accurate and relevant results.

### Advanced Ranking Algorithm

- **Prioritization**: The AI prioritizes different knowledge bases, with Private Knowledge taking precedence, followed by Microsoft Learn and then Community Knowledge.
- **Relevance and Context**: The algorithm evaluates the relevance of information from each source, considering the current context and query specifics. 
- **Efficient Information Retrieval**: By giving more weight to higher-priority sources in the context window, the AI ensures that the most relevant and authoritative information is used in responses.
- **Dynamic Responses**: Depending on the query and available information, the final response may draw more from one source over others, despite the set priorities. This flexibility allows CentralQ Chat to adapt to the nature and detail of the available documentation.

### Streaming Effect for Quick Responses

- **Real-time Processing**: As soon as the first part of the response is ready, it's streamed to the user. This approach minimizes waiting times, enhancing user experience.

!!! note "Note"
    The interplay of rephrasing, hybrid search, and the ranking algorithm ensures that CentralQ Chat delivers precise, well-sourced answers, tailored to each unique query.
