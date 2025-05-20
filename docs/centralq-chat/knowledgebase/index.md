# CentralQ Chat Knowledgebase

The Knowledgebase is a core component of CentralQ Chat that addresses the challenge of finding information in Microsoft Dynamics 365 Business Central. By providing instant responses sourced from private documents, Microsoft Learn, and community knowledge, CentralQ Chat enhances productivity and operational efficiency.

## Key Capabilities

- **Private Documents Integration**: Upload your own guides, manuals, documentation, and page scripts to personalize the AI's responses to your specific Business Central setup.

- **Microsoft Learn Integration**: Access Microsoft's official, up-to-date documentation to ensure reliable and current information directly from the source.

- **Community Knowledge**: Leverage insights from community-generated content, including expert blogs, instructional videos, tweets, and authoritative books.

- **Page Scripting Support**: Import page scripting directly from YAML files or through links, enabling dynamically generated user manuals that update the knowledgebase.

- **Interactive Responses**: Every response includes citations from relevant sources, adding transparency and credibility to the information provided.

## Types of Knowledge Sources

The CentralQ Chat Knowledgebase draws from three main types of information:

### Private Documents

Private documents personalize your CentralQ Chat experience by providing context specific to your Business Central environment:

- **File Uploads**: Upload Business Central-related documents including guides, manuals, and relevant materials.
- **User Manuals**: Automatically generated in the current language setting of Business Central and integrated into the knowledgebase.
- **Page Scripts**: Create interactive workflows that users can execute directly from chat responses via actionable URLs.

### Microsoft Learn

Official Microsoft documentation ensures you receive reliable and current information from the authoritative source on Business Central features and functionality.

### Community Knowledge

Access a wealth of insights from Business Central experts and the wider community, including blog posts, videos, and other curated content.

## How It Works

According to the CentralQ Chat architecture:

1. **Upload Documents**: Users upload their Business Central-related documents or add links to relevant resources.
2. **Ask Questions**: Through the chat interface, users can ask operational questions about Business Central.
3. **AI-Powered Analysis**: The system employs advanced AI models, including OpenAI's GPT-4, to understand queries and generate responses.
4. **Smart Ranking**: A ranking system prioritizes sources based on user settings—private documents first, followed by Microsoft Learn and Community Knowledge.
5. **Comprehensive Answers**: The AI combines insights from these sources to provide accurate, context-relevant answers.

## Priorities

CentralQ Chat prioritizes different knowledge sources to ensure the most relevant answers:

| Knowledge Source | Priority | Description |
|-----------------|----------|-------------|
| Private Knowledge | ![High](https://img.shields.io/badge/High-grey) | AI favors information from uploaded documents over other sources. |
| Microsoft Learn | ![Medium](https://img.shields.io/badge/Medium-grey) | Used when information is not available in private knowledge, or private knowledge is limited. |
| Community Knowledge | ![Low](https://img.shields.io/badge/Low-grey) | Utilized when information is unavailable or limited in the above two sources. |

!!! note "AI response specifics"
    It's important to understand that while private knowledge is prioritized, the AI's response may integrate broader sources for a comprehensive answer.

    Due to the limitation of the context window, CentralQ Chat employs a smart retrieval and ranking mechanism. This mechanism allocates more tokens in the context window to content marked with higher prioritization. However, the nature of vector databases and Language Learning Models (LLMs) may lead to a higher utilization of information from community knowledge or Microsoft Learn compared to private knowledge. This variability depends on the specificity of the question and the detail and structure of the private documentation.

## Security and Privacy

CentralQ Chat prioritizes the security and privacy of your data:

- **Private Azure Blob Storage**: Files are securely stored with controlled access.
- **Temporary Access Links**: Download links are valid for only 15 minutes to prevent unauthorized sharing.
- **Data Privacy**: Private data is never used for training AI models.
- **Cloud Qdrant**: Content is securely stored and linked specifically to the user's chat ID.
- **Azure Keyvault**: Sensitive information like chat IDs and keys are protected with restricted access.

## Next Steps

- ➡️ **[Private Data](./private-data/index.md)**: Learn how to upload and manage your organization's documents.
- 🌐 **[Public Data](./public-data.md)**: Discover how to incorporate Microsoft Learn and community knowledge.
- 📜 **[Page Scripting](./private-data/add-page-scripts.md)**: Explore how to create interactive workflows and automated user manuals. 