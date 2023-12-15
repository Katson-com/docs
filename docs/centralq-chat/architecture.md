CentralQ Chat, integrated within Microsoft Business Central, operates through a sophisticated architecture involving various Azure services and cloud-based technologies. This architecture ensures efficient processing of user queries, secure storage of private data, and effective retrieval of relevant information.

![CentralQ Chat Architecture](../assets/img/centralq-chat-architecture.png)

### Core Components

1. **Private Azure Web App**: The heart of CentralQ Chat, this web application manages user interactions and orchestrates the flow of data and requests. It ensures a seamless user experience while maintaining the security and privacy of the data.

2. **Azure AI Search**: Utilized for classical keyword searches, Azure AI Search processes user queries to fetch relevant information from a wide array of sources, including Microsoft Learn and Community Knowledge.

3. **Cloud Qdrant**: A pivotal component for semantic search, Cloud Qdrant interprets and analyzes the context and semantics of user queries. This ensures that the responses generated are contextually accurate and relevant.

4. **Azure OpenAI**: Once a final prompt is constructed from the search results, it is sent to Azure OpenAI. The AI then generates the response, which is displayed on the Azure Web App UI.

### Data Storage and Security

1. **Private Azure Blob Storage**: Used for securely storing user-uploaded files, access to this storage is strictly controlled through secure keys. This ensures that files can only be accessed through designated actions within CentralQ Chat.

2. **Secure Cloud Qdrant Storage**: Both uploaded files and web page contents are securely stored in the cloud Qdrant. This content is linked to specific chat IDs, making it exclusive to that chat session and inaccessible in other chats or on the public centralq.ai platform.

3. **Azure KeyVault**: Securely stores chat IDs and keys, allowing only the Azure Web App to access them.

4. **Azure Cosmos DB**: Maintains a list of private data sources added by the user, linked to their specific chat ID.

### Operational Flow

- When a user asks a question in CentralQ Chat, the Azure Web App initiates a search process involving both Azure AI Search and Cloud Qdrant.
- The retrieved data forms a comprehensive prompt sent to the Azure OpenAI instance.
- The AI instance processes this prompt and sends back an intelligent, context-aware response to the user through the Azure Web App interface.
- Files and webpages in the source part are exclusively linked to their respective chat IDs and are not accessible outside of their specific chat environment or in the public domain of centralq.ai.

!!! note
    The architecture ensures that all data interactions are secure, private, and confined within the specified chat environment.