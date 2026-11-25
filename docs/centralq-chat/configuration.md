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

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/9511419b-5c74-4582-8d51-fb11a23d8324?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Set up"></iframe></div>

#### Existing Users
If you already use CentralQ Chat and have uploaded a knowledge base, toggle "I have Chat Id" and enter your Chat Id and Secret Key to retrieve your data.
You should see Authentication Successful message. In case you see Authentication Failed, please check your Chat Id and Secret Key.

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/2c88058e-8036-456a-a29e-c2510d2e1d62?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Set up for Existing Chat"></iframe></div>

#### Completing Setup
Proceed with "Next" and "Finish" to complete the registration or connection to CentralQ Cloud.

### Configuring Chat Experience

CentralQ Chat allows you to control the knowledge base sources for AI responses:

- **Use Microsoft Learn**: Incorporates Microsoft Learn resources into the AI's search scope for answers.
- **Use Community Knowledge**: Taps into blogs, videos, tweets, and more from the Business Central community. View the [community knowledge list](https://www.centralq.ai/kb) for more information.
- **Use Private Knowledge**: Utilizes your privately uploaded documents for responses.
- **Use Insights Agent**: Enables the Data Insights Agent feature, allowing users to query and analyze their live Business Central data.

### :new: Configuring Data Insights Agent

If you want to enable data analysis capabilities in CentralQ Chat

<div style="padding:49.22% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/8ab2bcc1-a6e4-4eff-92d6-2fd01180e0a8?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="centralq-chat-data-agent-setup"></iframe></div>

1. **Enable the Feature**: On the "CentralQ Chat Setup" page, find the "Chat experience" FastTab and toggle "Use Insights Agent" to enable the feature.

2. **Complete Setup Wizard**: When first enabled, the "Insights Agent Wizard" will open automatically to guide you through the configuration process:
   - You'll need to provide a Microsoft Entra application's Client ID and Client Secret with appropriate Business Central API permissions
   - These credentials enable secure data access while respecting user permissions

3. **Manual Configuration**: You can also start the setup process manually using the "Setup Insights Agent" action on the CentralQ Chat Setup page.

!!! info "Detailed Setup Instructions"
    For complete step-by-step instructions on setting up the Data Insights Agent, see the [Getting Started with Data Insights](data-insights/getting-started.md) guide.

## Next Steps

- 📚 **[Knowledgebase](./knowledgebase/index.md)**: Start building your private knowledge base by uploading documents.
- 💬 **[Chat](./chat.md)**: Begin using the chat interface to ask questions about Business Central.
- 📊 **[Data Insights Agent](./data-insights/index.md)**: Learn how to analyze your Business Central data with natural language queries.
- 🔒 **[Security](./security.md)**: Understand the security measures protecting your data and communications.
- ❓ **[FAQ](./faq.md)**: Find answers to common questions about using CentralQ Chat.