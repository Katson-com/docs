Follow these steps to configure CentralQ Chat for an optimized, secure, and personalized user experience.

### Registering in CentralQ Cloud

1. **Access Assisted Setup**: Go to Assisted setup and search for "Set up CentralQ Chat".
2. **Connect to CentralQ Cloud**: In the CentralQ Chat Setup, click "Connect CentralQ Cloud".

    !!! info 
        CentralQ Cloud is a secure storage for your private information. It allows CentralQ Chat to access your uploaded documents for more accurate and personalized answers.

#### First-time Users
**Chat Id and Secret Key Generation**: A unique Chat Id and Secret Key will be generated automatically.

- **Chat Id**: A unique identifier to manage your documents in CentralQ Cloud.
- **Secret Key**: A confidential key for secure access. 

    !!! warning "Important"
        Copy and securely store the Secret Key as it will not be displayed again.

    !!! warning "Important"
        Keep your Chat Id and Secret Key safe. Losing them means losing access to your private knowledge.

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/893995665?h=0263a23be1&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Set up"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

#### Existing Users
If you already use CentralQ Chat and have uploaded a knowledge base, toggle "I have Chat Id" and enter your Chat Id and Secret Key to retrieve your data.
You should see Authentication Successful message. In case you see Authentication Failed, please check your Chat Id and Secret Key.

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/894000719?h=94873d9956&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Set up for Existing Chat"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

#### Completing Setup
Proceed with "Next" and "Finish" to complete the registration or connection to CentralQ Cloud.

### Configuring Chat Experience

CentralQ Chat allows you to control the knowledge base sources for AI responses:

- **Use Microsoft Learn**: Incorporates Microsoft Learn resources into the AI's search scope for answers.
- **Use Community Knowledge**: Taps into blogs, videos, tweets, and more from the Business Central community. View the [community knowledge list](https://www.centralq.ai/kb) for more information.
- **Use Private Knowledge**: Utilizes your privately uploaded documents for responses.

### Priorities

CentralQ Chat prioritizes different knowledge bases to ensure the most relevant answers:

- **Private Knowledge**: Highest priority. AI favors information from uploaded documents over other sources.
- **Microsoft Learn**: Second priority. Used when information is not available in private knowledge, or private knowledge is limited.
- **Community Knowledge**: Lowest priority, utilized when information is unavailable or limited in the above two sources.

!!! note "AI response specifics"
    It's important to understand that while private knowledge is prioritized, the AI's response may integrate broader sources for a comprehensive answer.

    Due to the limitation of the context window, CentralQ Chat employs a smart retrieval and ranking mechanism. This mechanism allocates more tokens in the context window to content marked with higher prioritization. However, the nature of vector databases and Language Learning Models (LLMs) may lead to a higher utilization of information from community knowledge or Microsoft Learn compared to private knowledge. This variability depends on the specificity of the question and the detail and structure of the private documentation.