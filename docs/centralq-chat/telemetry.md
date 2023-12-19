# Telemetry in CentralQ Chat

CentralQ Chat integrates telemetry to gain insights into the app's use, helping to improve features and user experience. Below is an index of telemetry events and their descriptions.

| Event ID     | Area                  | Message                                                  |
|--------------|-----------------------|----------------------------------------------------------|
| AL0001CCO    | Cloud Connection      | [Connect CentralQ Cloud opened](#AL0001CCO)              |
| AL0002CCF    | Cloud Connection      | [Connect CentralQ Cloud finished](#AL0002CCF)            |
| AL0003CCE    | Cloud Connection      | [Used existing Chat Id](#AL0003CCE)                      |
| AL0004CCN    | Cloud Connection      | [New Chat Id generated](#AL0004CCN)                      |
| AL0005CCA    | Cloud Connection      | [Authenticated successfully](#AL0005CCA)                 |
| AL0006CCE    | Cloud Connection      | [Authentication failed](#AL0006CCE)                      |
| AL0007CCR    | Cloud Connection      | [Registered successfully](#AL0007CCR)                    |
| AL0008CCE    | Cloud Connection      | [Registration failed](#AL0008CCE)                        |
| AL0009CCE    | Cloud Connection      | [Acquire authentication token failed](#AL0009CCE)        |


## Details of Telemetry Events

<!-- ### <a id="AL0001CHS"></a>AL0001CHS - Chat Session Started
This event is triggered when a user begins a new chat session, allowing us to understand user engagement.

...

### <a id="AL0021UNS"></a>AL0021UNS - App Uninstalled from Business Central
This event is important for understanding the app's lifecycle and reasons for uninstallation.
 -->

### <a id="AL0001CCO"></a>AL0001CCO - Connect CentralQ Cloud Opened
This event is triggered when a user opens the Connect CentralQ Cloud, allowing us to understand user engagement.

### <a id="AL0002CCF"></a>AL0002CCF - Connect CentralQ Cloud Finished
This event is triggered when a user finishes connecting to CentralQ Cloud, allowing us to understand user engagement.

### <a id="AL0003CCE"></a>AL0003CCE - Use Existing Chat Id
This event is triggered when a user uses an existing chat id, during the connection to CentralQ Cloud.

### <a id="AL0004CCN"></a>AL0004CCN - New Chat Id Generated
This event is triggered when a user generates a new chat id, during the connection to CentralQ Cloud.

### <a id="AL0005CCA"></a>AL0005CCA - Authenticated Successfully
This event is triggered when a user successfully authenticates to CentralQ Cloud.

### <a id="AL0006CCE"></a>AL0006CCE - Authentication Failed
This event is triggered when a user fails to authenticate to CentralQ Cloud.

### <a id="AL0007CCR"></a>AL0007CCR - Registered Successfully
This event is triggered when a user successfully registers new CentralQ Cloud account.

### <a id="AL0008CCE"></a>AL0008CCE - Registration Failed
This event is triggered when a user fails to register new CentralQ Cloud account.

### <a id="AL0009CCE"></a>AL0009CCE - Acquire Authentication Token Failed
This event is triggered when a user fails to acquire authentication token from CentralQ Cloud.

## Telemetry Data Compliance
All telemetry data is collected in compliance with privacy laws and regulations. Users are informed of the data collection and can opt-out if desired.

## Feedback
Your feedback on CentralQ Chat is crucial. If you have suggestions on telemetry events or data handling, please contact us at [contact information].



<!-- | Event ID     | Area                  | Message                                                  |
|--------------|-----------------------|----------------------------------------------------------|
| AL0001CHS    | Chat Session          | Chat session started                                     |
| AL0002CHQ    | Chat Question         | New question asked                                       |
| AL0003CHA    | Chat Answer           | Answer generated                                         |
| AL0004FUP    | File Upload           | File upload initiated                                    |
| AL0005FUC    | File Upload Complete  | File upload completed                                    |
| AL0006FUF    | File Upload Fail      | File upload failed                                       |
| AL0007FDE    | File Deletion         | File deleted                                             |
| AL0008COC    | Cloud Connection      | CentralQ Cloud connected                                 |
| AL0009CCH    | Configuration Change  | Configuration changed                                    |
| AL0010URE    | User Registration     | New user registered                                      |
| AL0011SUB    | Subscription          | Subscription status changed                              |
| AL0012FEB    | Feedback              | Feedback submitted                                       |
| AL0013LIC    | License Assignment    | License assigned to user                                 |
| AL0014LIR    | License Removal       | License removed from user                                |
| AL0015TRI    | Trial Period          | Trial period started                                     |
| AL0016TRIEND | Trial Period End      | Trial period ended                                       |
| AL0017API    | API Interaction       | API interaction occurred                                 |
| AL0018SEC    | Security              | Security-related event (login, logout, key generation)   |
| AL0019ERR    | Error                 | Error occurred in the system                             |
| AL0020INS    | Installation          | App installed in Business Central                        |
| AL0021UNS    | Uninstallation        | App uninstalled from Business Central                    | -->
