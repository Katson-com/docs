# Data Insights Agent: Security and Data Privacy

The Data Insights Agent is built with security as a core principle. This page outlines the measures in place to protect your Business Central data.

## Security Framework

### 1. Secure Execution Environment

- **Isolated Sandbox**: AI-generated Python code runs in a secure, isolated environment
- **Hyper-V Isolation**: Complete separation from other processes and infrastructure
- **Restricted Network Access**: Limited ability to interact with external systems
- **Read-Only Operations**: The agent cannot modify your Business Central data

!!! warning "Important"
    The execution environment is completely sandboxed to ensure your Business Central environment remains secure.

### 2. Authentication and Authorization

- **Respects User Permissions**: Only accesses data the logged-in user is authorized to view
- **Secure Token Handling**: When the Data Insights Agent needs to access data, it requests a temporary token from 
Business Central. This token is:
    * Generated within your Business Central environment
    * Active only during the current session
    * Securely passed to the isolated sandbox environment
    * Never saved or logged anywhere

- **Microsoft Entra Application Security**: The ClientId and Client Secret used for authentication remain entirely within your Business Central environment and never leave your system. These credentials are used solely to obtain the temporary 
session token.

### 3. Data Privacy

- **Encrypted Communication**: All data transfers use HTTPS/TLS encryption
- **No Data Storage**: Business data is processed in memory only and not stored after analysis
- **Minimal Logging**: Only operational metrics are logged (no business data values or authentication details)
- **Transparency**: View the generated code through the "Thoughts" section

!!! info "Telemetry"
    CentralQ Chat only collects operational metrics like user intent and code execution success/failure. For more details, see our [Telemetry documentation](../telemetry.md).

### 4. LLM Interaction Security

- **API Structure Only**: Only API information is sent to the LLM, not your actual business data
- **Result Processing**: LLM receives summarized results to generate natural language responses
- **Error Handling**: Error messages are processed for Smart Retry functionality

### 5. Administrative Control

- **Admin-Managed**: The feature requires explicit activation by a Business Central administrator
- **Configurable**: Enable or disable the feature at any time

## Your Security Responsibilities

- Secure your Microsoft Entra application credentials
- Manage Business Central user permissions appropriately
- Review the "Thoughts" section to understand how answers are derived

## Next Steps

- ➡️ **[Getting Started](./getting-started.md)**: Enable the Data Insights Agent
- ✨ **[Key Features](./features.md)**: Understand the agent's capabilities
- ⚙️ **[How It Works](./how-it-works.md)**: Learn about the technical process 