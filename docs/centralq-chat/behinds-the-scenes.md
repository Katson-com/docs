CentralQ Chat leverages advanced AI technology and a sophisticated ranking mechanism to deliver accurate and relevant answers to your Business Central queries and provide powerful data insights. Here's an in-depth look at how it works:

### The AI Models

- **Models**: CentralQ Chat utilizes a combination of advanced AI models, including `gpt-4o` and `gpt-4o-mini`. These models are orchestrated based on the nature of your request to ensure optimal performance, accuracy, and efficiency.
- **Context Length**: The models operate within a context window that includes your input, system-generated prompts, retrieved information, chat history, and the AI's responses. The specific token limit varies by the model engaged for your query.
- **Balanced Context**: To ensure coherent and relevant conversations and analyses, the AI balances the various elements (user input, system prompt, retrieved knowledge, chat history) within the context limit. This means the AI may gradually "forget" earlier parts of a long conversation as the dialogue progresses.

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

### Data Insights Agent

CentralQ Chat extends its capabilities with the Data Insights Agent, allowing you to interact with your Business Central data using natural language. This powerful feature enables you to:

- Ask complex questions about your sales, inventory, financials, and more.
- Receive instant insights with automatically generated visualizations.
- Understand how answers are derived through transparent "Thoughts" detailing the AI's reasoning and the code used.

For a comprehensive understanding, please refer to the dedicated [Data Insights Agent documentation](./data-insights/index.md).

### Streaming Effect for Quick Responses

- **Real-time Processing**: As soon as the first part of the response is ready, it's streamed to the user. This approach minimizes waiting times, enhancing user experience.

!!! note "Note"
    The interplay of rephrasing, hybrid search, and the ranking algorithm ensures that CentralQ Chat delivers precise, well-sourced answers, tailored to each unique query. The Data Insights Agent further enhances this by providing direct access to and analysis of your live Business Central data.

## Next Steps

Explore other aspects of CentralQ Chat:

- 🚀 **[Getting Started](./getting-started.md)**: Begin your journey with CentralQ Chat.
- 🔧 **[Configuration](./configuration.md)**: Learn how to configure CentralQ Chat to meet your needs.
- 🧠 **[Knowledgebase](./knowledgebase/index.md)**: Understand how CentralQ Chat accesses and uses information.
- 💬 **[Chat](./chat.md)**: Discover the features of the chat interface.
- 📊 **[Data Insights Agent](./data-insights/index.md)**: Dive deeper into the Data Insights Agent.
- 🔐 **[Security](./security.md)**: Learn about the security measures in place.
- 💡 **[Limitations](./limitations.md)**: Understand the current limitations of CentralQ Chat.
