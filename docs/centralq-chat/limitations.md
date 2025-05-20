CentralQ Chat, while being a powerful tool for instant information retrieval about Microsoft Business Central, operates within certain limitations that users should be aware of.

### Limitations in Data Access and Functionality

- **Core Chat Data Access**: The core chat functionality of CentralQ Chat (i.e., when not using the Data Insights Agent) does not directly access or interact with your live Business Central data. In this mode, it cannot provide insights or analyses based on your specific, real-time Business Central data.
- **Data Insights Agent**: The **Data Insights Agent** *does* directly access and interact with your Business Central data to provide insights and visualizations. Its access is governed by:
    - The availability of data through Business Central APIs (standard and custom).
    - The user's permissions within Business Central. You will only see data your account is authorized to access.
    For more details, refer to the [Data Insights Agent documentation](./data-insights/index.md).
- **Cannot Execute Business Central Functions**: CentralQ Chat, including the Data Insights Agent, cannot perform write actions (like creating, modifying, or deleting records) or run operational functions within Business Central. It is primarily a tool for information retrieval and data analysis.

### AI-Generated Content and Accuracy

- **Potential for Inaccuracies**: While AI strives for accuracy, it can occasionally generate incorrect or misleading information. This is an inherent limitation of current AI technology.
- **Data Insights Agent - Preview Considerations**: 
    - The Data Insights Agent is currently in **preview**. While it retrieves data directly from your Business Central environment (which is a source of truth), the agentic way it chooses which APIs to call, what fields to select, and how to manipulate the data can sometimes lead to unexpected or misleading interpretations and visualizations.
    - **Always critically review** the insights provided. It is crucial to use the **"Thoughts" section** to understand how the agent arrived at its conclusions and to verify the approach taken. You can learn more about the "Thoughts" section in the [Key Features](./data-insights/features.md#llm-thoughts) documentation.
- **Need for Fact-Checking**: Always cross-reference AI responses with cited sources (for general chat) or the underlying data and agent reasoning (for Data Insights). The AI might "hallucinate" or present information out of context.
- **Variability in Response Quality**: The quality and accuracy of responses can vary based on the question's complexity and the available knowledge base.

### Contextual Limitations

- **Context Window Constraint**: The AI operates with a context length of 16,384 tokens, encompassing the input, system prompt, retrieved information, chat history, and the response. This limitation can impact the continuity and relevance of responses in prolonged interactions.
- **Session-Based Interaction**: Each chat session is designed to address a specific topic or user intent. Switching topics mid-session may lead to less coherent responses.

### File Handling Limitations

- **File Format and Size Restrictions**: CentralQ Chat supports `.pdf`, `.docx`, and `.txt` files, with a maximum size limit of 3 MB per file.
- **Private Data Limit**: Users can upload up to 100 MB of private data per month, approximately equivalent to 1000 PDF pages.
- **User Requests Limit**: The system allows up to 500 user requests per month.
- **Temporary File Access**: File links in answers are accessible for only 15 minutes for security purposes.
- **Irreversible Deletion**: Deleted files and embeddings are permanently removed from cloud storage and the vector database.

### Links to Business Central pages
- Currently, CentralQ Chat does not support links to Business Central pages. This feature will be added in a future releases.