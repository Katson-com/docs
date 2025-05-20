CentralQ Chat prioritizes the security and privacy of user data, especially when it comes to the storage and access of files and private data.

### File Storage and Access

1. **Private Azure Blob Storage**: Files uploaded by users are securely stored in private Azure Blob Storage. Access to these files is strictly controlled and requires a key, ensuring no public or unauthorized access.

2. **File Download**: Users can download files through two secure methods:
      - Via the Private Data page on CentralQ Chat.
      - Through temporary links provided in chat responses, valid for only 15 minutes to prevent unauthorized sharing.

### Data Privacy and Usage

- **Private Data Security**: Private data, including files and web content, is never used for training AI models. The primary use of this data is to provide context and content for answering user queries within the CentralQ Chat environment.

- **Telemetry and Chat Interactions**: While CentralQ Chat collects telemetry data, including chat interactions, this information is not used for training purposes. Instead, it's utilized for analytical purposes to enhance the app's performance and user experience.

### Ensuring Data Security

- **Secure Cloud Qdrant**: Content from files and web pages added by users is stored in a secure cloud database, linked specifically to the user's chat ID. This ensures that private data remains confined within the user's environment.

- **Azure Keyvault**: This component securely stores sensitive information like chat IDs and keys. It restricts access exclusively to the Azure Web App, further enhancing data security.

### Data Insights Agent Security

- **Sandboxed Execution**: The Data Insights Agent runs in an isolated Hyper-V environment, completely separated from your Business Central data and other processes.

- **Read-Only Operations**: The agent cannot modify your Business Central data and only accesses information the logged-in user is authorized to view.

- **Secure Token Handling**: Authentication uses temporary session tokens that remain within your Business Central environment.

- **No Data Storage**: Business data is processed in memory only and not persisted after analysis.

For comprehensive information about Data Insights Agent security measures, please refer to the [Data Insights Security documentation](data-insights/security.md).

### Commitment to Privacy

CentralQ Chat is committed to maintaining the highest standards of data privacy and security. This commitment extends to ensuring that user data is not misused for training purposes and that all telemetry and interaction data is solely for improving the app's functionality and user experience. The architecture of CentralQ Chat is designed to safeguard user data while providing a seamless and efficient user interface.