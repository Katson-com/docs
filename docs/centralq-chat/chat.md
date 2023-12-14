CentralQ Chat is an AI-driven interactive guide for Microsoft Business Central, designed to provide instant answers about Business Central Environment sourced from Private Documents, Microsoft Learn, and Community Knowledge.

### User Workflow

1. **Open CentralQ Chat**: Launch CentralQ Chat.
2. **Ask a Question**: Start by asking about any Business Central-related topic.
3. **Follow-Up**: Dive deeper with related questions.
4. **Review Sources**: Check the sources for additional information.
5. **Topic Switch**: Refresh the chat to start a new topic.

### Chat Interface

- **Preparation Time**: Takes 2-5 seconds to prepare the chat environment upon opening or refreshing.

    <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/894521557?h=d40783db67&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Loading"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

- **Input Area**: Ask any question about Business Central. The AI utilizes various knowledge bases depending on your CentralQ Chat Setup configuration.
- **Input Limitation**: Recommended to keep input within 100-150 words for optimal processing.
- **Cited Sources**: Every answer includes citations from relevant sources such as files, web links, tweets, or YouTube videos.

    <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/894527053?h=d7763ef406&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - User Input"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
    ### Chat Session Flow

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

### Follow up on topic

- **Follow-up Questions**: Each session allows unlimited follow-up questions, but remember that AI might lose track of earlier parts of the conversation.
    <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/894534909?h=cc3a3d1fc4&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Follow up (Copy)"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

- **Session Reset**: To switch topics, click on `Refresh` the chat to start a new session.

### Feedback and Improvement

- **Providing Feedback**: Use the :fontawesome-regular-thumbs-up: :fontawesome-regular-thumbs-down: feature and leave comments to help improve answer accuracy and the overall quality of CentralQ Chat.

    <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/894547039?h=a33ac49bd6&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Feedback (Copy)"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

### Limitations

- **No Data Access**: CentralQ Chat does not access Business Central data and cannot offer insights.
- **No Features Execution**: CentralQ Chat cannot execute Business Central functions.

!!! warning "Important"
    Refreshing or closing the CentralQ Chat window will result in the loss of the ongoing conversation.