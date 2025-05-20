CentralQ Chat is an AI-driven interactive guide for Microsoft Business Central, designed to provide instant answers about Business Central Environment sourced from Private Documents, Microsoft Learn, and Community Knowledge. It also enables data analysis capabilities, allowing users to query Business Central data using natural language and receive visual insights with charts and graphs.

<div style="padding:56.19% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/904030365?h=c8bf9fb738&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - UI"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

### What can you ask?
Users can ask two types of questions:

- **Guidance Questions**: Get help on how to use Business Central features, setup instructions, troubleshooting, and best practices.
- **Data Insights Questions**: Analyze your actual Business Central data with natural language queries to gain business intelligence and visual insights.

### User Workflow

1. **Open CentralQ Chat**: Launch CentralQ Chat.
2. **Ask a Question**: Start by asking about any Business Central-related topic.
3. **Follow-Up**: Dive deeper with related questions.
4. **Review Sources**: Check the sources for additional information.
5. **Topic Switch**: Refresh the chat to start a new topic.

### Chat Interface

- **Preparation Time**: Takes 2-5 seconds to prepare the chat environment upon opening or refreshing.

    <div style="padding:56.19% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/904032131?h=0b35aa4b5a&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - UI loading"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

- **Input Area**: Ask any question about Business Central. The AI utilizes various knowledge bases depending on your CentralQ Chat Setup configuration.
- **Input Limitation**: Recommended to keep input within 100-150 words for optimal processing.
- **Cited Sources**: Every answer includes citations from relevant sources such as files, web links, tweets, or YouTube videos.

### Guidance Questions
Guidance questions allow users to get help with Business Central functionality, setup, and best practices. The AI draws from multiple knowledge sources to provide comprehensive, cited answers:

- **Private Documents**: Company-specific guides and documentation
- **Microsoft Learn**: Official Business Central documentation
- **Community Knowledge**: Expert blogs, videos, and community content

<div style="padding:49.64% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1085595373?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="centralq-chat-getting-started-guidance"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>


1. **Starting a Session**: Each session focuses on a specific user intent, beginning with the user's initial question.
2. **Rephrasing Queries**: The AI rephrases queries for clarity and search optimization, both for the initial and follow-up questions.
   
    !!! note "Example"
        - User input: "posting sales doc"
        - Rephrased question: "How do I post a sales document in Business Central?"
        - User input: "and how to cancel it?"
        - Rephrased question: "How can I cancel a posted sales order in Microsoft Dynamics 365 Business Central?"
    
    !!! tip   
        If rephrasing misinterprets your intent, try rephrasing your question for better accuracy.

3. **Searching and Responding**: CentralQ Chat uses a hybrid of classic keyword and semantic searches to generate a prompt. The prompt is then sent to Azure OpenAI for response generation, using a streaming effect for quicker display of answers.

4. **Answer Generation**: The AI generates answers based on the prompt and the context window, which includes the user's input, system-generated prompts, retrieved information, chat history, and the AI's responses.

    - **Response Time**: Typically, full answers are generated within 13 seconds, with initial tokens appearing in 3-5 seconds.
    - **Hallucinations**: Be aware that AI-generated text may occasionally contain inaccuracies or "hallucinations." Always verify answers against the provided sources.

    !!! tip 
        Always cross-reference AI responses with cited sources for accuracy.

5. **Rendering Sources**: Source links are inlined in answers and listed in an expandable section. YouTube links can be played directly or in picture-in-picture mode.

6. **Related Questions**: CentralQ Chat enhances your search experience by offering up to three related questions based on your initial query. These suggestions are designed to provide different perspectives and delve deeper into the topic, helping you explore various aspects and refine your understanding.

7. **Session Reset**: To switch topics, click on `Refresh` the chat to start a new session.

### Follow up on topic

- **Follow-up Questions**: Each session allows unlimited follow-up questions, but remember that AI might lose track of earlier parts of the conversation.
    <div style="padding:56.19% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/904035120?h=eb7b9eacb9&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Follow up questions"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>


### :material-new-box: Data Insights Agent

With the Data Insights Agent feature enabled, CentralQ Chat can analyze your Business Central data and generate valuable insights:

- **Natural Language Data Queries**: Ask questions about your live Business Central data in plain English
- **Visual Insights**: Receive answers with charts and graphs to better understand trends and patterns
- **Business Intelligence**: Get key business insights on sales, financials, inventory, and more directly in the chat

<div style="padding:49.27% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1085683957?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="centralq-chat-data-insights-sales-trend-with-follow-up"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

!!! info
    The Data Insights Agent is an optional feature that requires additional configuration.
    Learn more in the [Data Insights Agent section](data-insights/index.md).

### Feedback and Improvement

- **Providing Feedback**: Use the :fontawesome-regular-thumbs-up: :fontawesome-regular-thumbs-down: feature and leave comments to help improve answer accuracy and the overall quality of CentralQ Chat.

    <div style="padding:56.19% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/904076393?h=2574b29e2a&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Feedback"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

### Limitations

- **No Features Execution**: CentralQ Chat cannot execute Business Central functions.

!!! warning "Important"
    Refreshing or closing the CentralQ Chat window will result in the loss of the ongoing conversation.

## Next Steps

- 📊 **[Data Insights Agent](./data-insights/index.md)**: Learn how to analyze your Business Central data with natural language queries.
- 📚 **[Knowledgebase](./knowledgebase/index.md)**: Enhance your chat experience by building a private knowledge base.
- ❓ **[FAQ](./faq.md)**: Find answers to common questions about using CentralQ Chat.
- 📋 **[Limitations](./limitations.md)**: Understand the current limitations of the CentralQ Chat functionality.
- 🔄 **[Release Notes](./release-notes.md)**: Stay updated with the latest features and improvements.