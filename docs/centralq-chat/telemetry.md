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
| AL0010CCU    | Cloud Connection      | [Used Connection to CentralQ Cloud](#AL0010CCU)          |
| AL0011CT0    | Chat Session          | [Chat opened](#AL0011CT0)                                |
| AL0012CCC    | Cloud Connection      | [Connect CentralQ Cloud opened from Chat](#AL0012CCC)    |
| AL0013CCS    | Cloud Connection      | [Connect CentralQ Cloud opened from Setup](#AL0013CCS)   |
| AL0014CTL    | Chat Session          | [Microsoft Learn used](#AL0014CTL)                       |
| AL0015CTC    | Chat Session          | [Community Knowledge used](#AL0015CTC)                   |
| AL0016CTP    | Chat Session          | [Private Knowledge used](#AL0016CTP)                     |
| AL0017MLD    | Microsoft Learn       | [Microsoft Learn setup discovered](#AL0017MLD)           |
| AL0018MLC    | Microsoft Learn       | [Microsoft Learn setup changed](#AL0018MLC)              |
| AL0019MLE    | Microsoft Learn       | [Microsoft Learn enabled](#AL0019MLE)                    |
| AL0020MLD    | Microsoft Learn       | [Microsoft Learn disabled](#AL0020MLD)                   |
| AL0021MLU    | Microsoft Learn       | [Microsoft Learn used](#AL0021MLU)                       |
| AL0022CKD    | Community Knowledge   | [Community Knowledge setup discovered](#AL0022CKD)       |
| AL0023CKC    | Community Knowledge   | [Community Knowledge setup changed](#AL0023CKC)          |
| AL0024CKE    | Community Knowledge   | [Community Knowledge enabled](#AL0024CKE)                |
| AL0025CKD    | Community Knowledge   | [Community Knowledge disabled](#AL0025CKD)               |
| AL0026CKU    | Community Knowledge   | [Community Knowledge used](#AL0026CKU)                   |
| AL0027PKD    | Private Knowledge     | [Private Knowledge setup discovered](#AL0027PKD)         |
| AL0028PKC    | Private Knowledge     | [Private Knowledge setup changed](#AL0028PKC)            |
| AL0029PKE    | Private Knowledge     | [Private Knowledge enabled](#AL0029PKE)                  |
| AL0030PKD    | Private Knowledge     | [Private Knowledge disabled](#AL0030PKD)                 |
| AL0031PKU    | Private Knowledge     | [Private Knowledge used](#AL0031PKU)                     |
| AL0032PKO    | Private Knowledge     | [Private Knowledge opened](#AL0032PKO)                   |
| AL0033FUD    | File Upload           | [File upload initiated](#AL0033FUD)                      |
| AL0034FUS    | File Upload           | [File upload started ](#AL0034FUS)                       | 
| AL0035FUP    | File Upload           | [File passed validation](#AL0035FUP)                     |
| AL0036FUC    | File Upload           | [File upload completed](#AL0036FUC)                      |  
| AL0037FUX    | File Upload           | [File validation failed](#AL0037FUX)                     | 
| AL0038FUE    | File Upload           | [File extension is supported](#AL0038FUE)                |  
| AL0039FUX    | File Upload           | [File extension is not supported](#AL0039FUX)            | 
| AL0040FUX    | File Upload           | [Not supported file extension value](#AL0040FUX)         |    
| AL0041FUZ    | File Upload           | [File size](#AL0041FUZ)                                  |     
| AL0042FUX    | File Upload           | [File size is too large](#AL0042FUX)                     |  
| AL0043FUV    | File Upload           | [New file version upload initiated](#AL0043FUV)          | 
| AL0044FUV    | File Upload           | [New file version uploaded](#AL0044FUV)                  |
| AL0045FUE    | File Upload           | [File content embedding initiated](#AL0045FUE)           |
| AL0046FUX    | File Upload           | [File content embedding failed](#AL0046FUX)              |
| AL0047UUE    | Url Upload            | [Url Content Embedding Initiated](#AL0047UUE)            |
| AL0048UUX    | Url Upload            | [Url Content Embedding Failed](#AL0048UUX)               |
| AL0049UUD    | Url Upload            | [Url upload initiated](#AL0049UUD)                       |
| AL0050UUS    | Url Upload            | [Url upload started](#AL0050UUS)                         |
| AL0051UUP    | Url Upload            | [Url passed validation](#AL0051UUP)                      |
| AL0052UUC    | Url Upload            | [Url upload completed](#AL0052UUC)                       |
| AL0053FDD    | File Download         | [File download initiated](#AL0053FDD)                    |
| AL0054FDS    | File Download         | [File download started](#AL0054FDS)                      |
| AL0055FDP    | File Download         | [File download started](#AL0055FDP)                      |
| AL0056FDC    | File Download         | [File download completed](#AL0056FDC)                    |
| AL0057UUD    | Url Upload            | [Url deleted](#AL0057UUD)                                |
| AL0058FUD    | File Upload           | [File deleted](#AL0058FUD)                               |
| AL0059FUX    | File Upload           | [File deletion failed](#AL0059FUX)                       |
| AL0060UUX    | Url Upload            | [Url deletion failed](#AL0060UUX)                        |
| AL0061STO    | Statistics            | [Statistics opened](#AL0061STO)                          |
| AL0062FUE    | File Upload           | [Uploaded file extension value](#AL0062FUE)              |
| AL0063UUV    | Url Upload            | [New url version upload initiated](#AL0063UUV)           |
| AL0064UUV    | Url Upload            | [New url version uploaded](#AL0064UUV)                   |
| AL0065PKF    | Private Knowledge     | [No permission to manage private data](#AL0065PKF)       |
| PY0065CHS    | Chat Session          | [Chat session started](#PY0065CHS)                       |
| PY0066CHQ    | Chat Question         | [New question asked](#PY0066CHQ)                         |
| PY0067CHQ    | Chat Question         | [Follow-up Question Asked](#PY0067CHQ)                   |
| PY0068CHA    | Chat Answer           | [Answer generated](#PY0068CHA)                           |
| PY0069CHL    | Chat Session          | [Maximum monthly requests limit reached](#PY0069CHL)     |
| PY0070CHR    | Chat Question         | [Question rephrased](#PY0070CHR)                         |
| PY0071CHP    | Chat Answer           | [Private Knowledge Found](#PY0071CHP)                    |
| PY0072CHM    | Chat Session          | [Microsoft Learn Found](#PY0072CHM)                      |
| PY0073CHC    | Chat Session          | [Community Knowledge Found](#PY0073CHC)                  |

## Business Central Telemetry Events

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

### <a id="AL0010CCU"></a>AL0010CCU - Used Connection to CentralQ Cloud
This event is triggered when a user uses an existing connection to CentralQ Cloud.

### <a id="AL0011CT0"></a>AL0011CT0 - Chat Opened
This event is triggered when a user opens a new chat session, allowing us to understand user engagement.

### <a id="AL0012CCC"></a>AL0012CCC - Connect CentralQ Cloud Opened from Chat
This event is triggered when Connect CentralQ Cloud automatically opened the from the chat, allowing us to understand user engagement.

### <a id="AL0013CCS"></a>AL0013CCS - Connect CentralQ Cloud Opened from Setup
This event is triggered when Connect CentralQ Cloud manually opened the from the setup, allowing us to understand user engagement.

### <a id="AL0014CTL"></a>AL0014CTL - Microsoft Learn Used
This event is triggered when Microsoft Learn option is active during chat session.

### <a id="AL0015CTC"></a>AL0015CTC - Community Knowledge Used
This event is triggered when Community Knowledge option is active during chat session.

### <a id="AL0016CTP"></a>AL0016CTP - Private Knowledge Used
This event is triggered when Private Knowledge option is active during chat session.

### <a id="AL0017MLD"></a>AL0017MLD - Microsoft Learn Setup Discovered
This event is triggered when Microsoft Learn setup is discovered.

### <a id="AL0018MLC"></a>AL0018MLC - Microsoft Learn Setup Changed
This event is triggered when Microsoft Learn setup is changed.

### <a id="AL0019MLE"></a>AL0019MLE - Microsoft Learn Enabled
This event is triggered when Microsoft Learn is enabled.

### <a id="AL0020MLD"></a>AL0020MLD - Microsoft Learn Disabled
This event is triggered when Microsoft Learn is disabled.

### <a id="AL0021MLU"></a>AL0021MLU - Microsoft Learn Used
This event is triggered when Microsoft Learn is used.

### <a id="AL0022CKD"></a>AL0022CKD - Community Knowledge Setup Discovered
This event is triggered when Community Knowledge setup is discovered.

### <a id="AL0023CKC"></a>AL0023CKC - Community Knowledge Setup Changed
This event is triggered when Community Knowledge setup is changed.

### <a id="AL0024CKE"></a>AL0024CKE - Community Knowledge Enabled
This event is triggered when Community Knowledge is enabled.

### <a id="AL0025CKD"></a>AL0025CKD - Community Knowledge Disabled
This event is triggered when Community Knowledge is disabled.

### <a id="AL0026CKU"></a>AL0026CKU - Community Knowledge Used
This event is triggered when Community Knowledge is used.

### <a id="AL0027PKD"></a>AL0027PKD - Private Knowledge Setup Discovered
This event is triggered when Private Knowledge setup is discovered.

### <a id="AL0028PKC"></a>AL0028PKC - Private Knowledge Setup Changed
This event is triggered when Private Knowledge setup is changed.

### <a id="AL0029PKE"></a>AL0029PKE - Private Knowledge Enabled
This event is triggered when Private Knowledge is enabled.

### <a id="AL0030PKD"></a>AL0030PKD - Private Knowledge Disabled
This event is triggered when Private Knowledge is disabled.

### <a id="AL0031PKU"></a>AL0031PKU - Private Knowledge Used
This event is triggered when Private Knowledge is used.

### <a id="AL0032PKO"></a>AL0032PKO - Private Knowledge Opened
This event is triggered when Private Knowledge is opened.

### <a id="AL0033FUD"></a>AL0033FUD - File Upload Initiated
This event is triggered when a user initiates a file upload, allowing us to understand user engagement.

### <a id="AL0034FUS"></a>AL0034FUS - File Upload Started
This event is triggered when a user starts a file upload, allowing us to understand user engagement.

### <a id="AL0036FUC"></a>AL0036FUC - File Upload Completed
This event is triggered when a user completes a file upload, allowing us to understand user engagement.

### <a id="AL0037FUX"></a>AL0037FUX - File Validation Failed
This event is triggered when a user fails to validate a file, allowing us to understand user engagement.

### <a id="AL0038FUE"></a>AL0038FUE - File Extension is Supported
This event is triggered when a user uploads a file with a supported extension, allowing us to understand user engagement.

### <a id="AL0039FUX"></a>AL0039FUX - File Extension is Not Supported
This event is triggered when a user uploads a file with an unsupported extension, allowing us to understand user engagement.

### <a id="AL0040FUX"></a>AL0040FUX - Not Supported File Extension Value
This event is triggered when a user uploads a file with an unsupported extension value, and shows the name of the extension, allowing to collect data about unsupported extensions.

### <a id="AL0041FUZ"></a>AL0041FUZ - File Size
This event is triggered when a user uploads a file, and shows the size of the file, allowing to collect data about file sizes.

### <a id="AL0042FUX"></a>AL0042FUX - File Size is Too Large
This event is triggered when a user uploads a file that is too large, and shows the size of the file, allowing to collect data about file sizes.

### <a id="AL0043FUV"></a>AL0043FUV - New File Version Upload Initiated
This event is triggered when a user initiates a new file version upload, allowing us to understand user engagement.

### <a id="AL0044FUV"></a>AL0044FUV - New File Version Uploaded
This event is triggered when a user uploaded a new file version, allowing us to understand user engagement.

### <a id="AL0045FUE"></a>AL0045FUE - File Content Embedding Initiated
This event is triggered when a user initiates a file content embedding.

### <a id="AL0046FUX"></a>AL0046FUX - File Content Embedding Failed
This event is triggered when a user fails to embed file content.

### <a id="AL0047UUE"></a>AL0047UUE - Url Content Embedding Initiated
This event is triggered when a user initiates a url content embedding.

### <a id="AL0048UUX"></a>AL0048UUX - Url Content Embedding Failed
This event is triggered when a user fails to embed url content.

### <a id="AL0049UUD"></a>AL0049UUD - Url Upload Initiated
This event is triggered when a user initiates a url upload.

### <a id="AL0050UUS"></a>AL0050UUS - Url Upload Started
This event is triggered when a user starts a url upload.

### <a id="AL0051UUP"></a>AL0051UUP - Url Passed Validation
This event is triggered when a user passes url validation.

### <a id="AL0052UUC"></a>AL0052UUC - Url Upload Completed
This event is triggered when a user completes a url upload.

### <a id="AL0053FDD"></a>AL0053FDD - File Download Initiated
This event is triggered when a user initiates a file download.

### <a id="AL0054FDS"></a>AL0054FDS - File Download Started
This event is triggered when a user starts a file download.

### <a id="AL0055FDP"></a>AL0055FDP - File Download Started
This event is triggered when a user passes file download validation.

### <a id="AL0056FDC"></a>AL0056FDC - File Download Completed
This event is triggered when a user completes a file download.

### <a id="AL0057UUD"></a>AL0057UUD - Url Deleted
This event is triggered when a user deletes a url.

### <a id="AL0058FUD"></a>AL0058FUD - File Deleted
This event is triggered when a user deletes a file.

### <a id="AL0059FUX"></a>AL0059FUX - File Deletion Failed
This event is triggered when a user fails to delete a file.

### <a id="AL0060UUX"></a>AL0060UUX - Url Deletion Failed
This event is triggered when a user fails to delete a url.

### <a id="AL0061STO"></a>AL0061STO - Statistics Opened
This event is triggered when a user opens the statistics page.

### <a id="AL0062FUE"></a>AL0062FUE - Uploaded File Extension Value
This event is triggered when a user uploads a file, and shows the name of the extension, allowing to collect data about file extensions.

### <a id="AL0063UUV"></a>AL0063UUV - New Url Version Upload Initiated
This event is triggered when a user initiates a new url version upload, allowing us to understand user engagement.

### <a id="AL0064UUV"></a>AL0064UUV - New Url Version Uploaded
This event is triggered when a user uploaded a new url version, allowing us to understand user engagement.

### <a id="AL0065PKF"></a>AL0065PKF - No Permission to Manage Private Data
This event is triggered when a user tries to manage private data without permission.

## WebApp Telemetry Events

### <a id="PY0065CHS"></a>PY0065CHS - Chat Session Started
This event is triggered when a user starts a new chat session, allowing us to understand user engagement.

### <a id="PY0066CHQ"></a>PY0066CHQ - New Question Asked
This event is triggered when a user asks a new question, allowing us to understand user engagement. Question text is included in the event.

### <a id="PY0067CHQ"></a>PY0067CHQ - Follow-up Question Asked
This event is triggered when a user asks a follow-up question, allowing us to understand user engagement. Question text is included in the event, as well as the conversation history.

### <a id="PY0068CHA"></a>PY0068CHA - Answer Generated
This event is triggered when a user receives an answer, allowing us to understand user engagement. Answer text is included in the event, as well as the conversation history and sources used to generate the answer (with text and metadata).

### <a id="PY0069CHL"></a>PY0069CHL - Maximum Monthly Requests Limit Reached
This event is triggered when a user reaches the maximum monthly requests limit

### <a id="PY0070CHR"></a>PY0070CHR - Question Rephrased
This event is triggered when question is automatically rephrased by the AI. Original question text is included in the event.

### <a id="PY0071CHP"></a>PY0071CHP - Private Knowledge Found
This event is triggered when Private Knowledge is found for the question. Question text is included in the event, as well as private knowledge metadata.

### <a id="PY0072CHM"></a>PY0072CHM - Microsoft Learn Found
This event is triggered when Microsoft Learn is found for the question. Question text is included in the event, as well as Microsoft Learn metadata.

### <a id="PY0073CHC"></a>PY0073CHC - Community Knowledge Found
This event is triggered when Community Knowledge is found for the question. Question text is included in the event, as well as Community Knowledge metadata.


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
