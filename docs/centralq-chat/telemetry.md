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
| AL0033IAE    | Insights Agent        | [Insights Agent enabled](#AL0033IAE)                     |
| AL0034IAD    | Insights Agent        | [Insights Agent disabled](#AL0034IAD)                    |
| AL0035IAS    | Insights Agent        | [Setup Insights Agent opened from Setup](#AL0035IAS)     |
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
| AL0066FPD    | File Upload           | [Page Scripting File upload initiated](#AL0066FPD)       |
| AL0067FPS    | File Upload           | [Page Scripting File upload started](#AL0067FPS)         |
| AL0068FPP    | File Upload           | [Page Scripting File passed validation](#AL0068FPP)      |
| AL0069FPC    | File Upload           | [Page Scripting File upload completed](#AL0069FPC)       |
| AL0070UPD    | Url Upload            | [Page Scripting Url upload initiated](#AL0070UPD)        |
| AL0071UPS    | Url Upload            | [Page Scripting Url upload started](#AL0071UPS)          |
| AL0072UPP    | Url Upload            | [Page Scripting Url passed validation](#AL0072UPP)       |
| AL0073UPC    | Url Upload            | [Page Scripting Url upload completed](#AL0073UPC)        |
| AL0074FPD    | Private Knowledge     | [Page Scripting User Manual edit initiated](#AL0074FPD)  |
| AL0075FPS    | Private Knowledge     | [Page Scripting User Manual edit started](#AL0075FPS)    |
| AL0076FPC    | Private Knowledge     | [Page Scripting User Manual edit completed](#AL0076FPC)  |
| AL0077FDD    | File Download         | [User Manual download to Word initiated](#AL0077FDD)     |
| AL0078FDS    | File Download         | [User Manual download to Word started](#AL0078FDS)       |
| AL0079FDC    | File Download         | [User Manual download to Word completed](#AL0079FDC)     |
| AL0080FDD    | File Download         | [User Manual download to MD initiated](#AL0080FDD)       |
| AL0081FDS    | File Download         | [User Manual download to MD started](#AL0081FDS)         |
| AL0082FDC    | File Download         | [User Manual download to MD completed](#AL0082FDC)       |
| AL0083CSD    | Cloud Connection      | [Setup record deleted, associated secrets cleared](#AL0083CSD) |
| AL0084IAS    | Insights Agent        | [Insights Agent client secret is cleared](#AL0084IAS)    |
| AL0085IAT    | Insights Agent        | [Insights Agent client secret is set](#AL0085IAT)        |
| AL0086IAU    | Insights Agent        | [Insights Agent client secret is not set](#AL0086IAU)    |
| AL0087IAV    | Insights Agent        | [Insights Agent client secret get failed](#AL0087IAV)    |
| AL0088CCC    | Cloud Connection      | [CentralQ Cloud connection cleared (Table Trigger)](#AL0088CCC) |
| AL0089IAC    | Insights Agent        | [Insights Agent setup cleared (Table Trigger)](#AL0089IAC) |
| AL0090IAC    | Insights Agent        | [Insights Agent setup cleared via Setup Page action](#AL0090IAC) |
| AL0091CCC    | Cloud Connection      | [CentralQ Cloud connection cleared via Setup Page action](#AL0091CCC) |
| AL0092IBD    | Insights Agent        | [Failed to acquire access token (HTTP send error)](#AL0092IBD) |
| AL0093IBE    | Insights Agent        | [Failed to acquire access token (HTTP non-success status)](#AL0093IBE) |
| AL0094IBF    | Insights Agent        | [Failed to acquire access token (Token not found in response)](#AL0094IBF) |
| AL0095IAZ    | Insights Agent        | [Access token acquired successfully](#AL0095IAZ)         |
| AL0096IBB    | Insights Agent        | [Successfully connected to Business Central API (Test Connection)](#AL0096IBB) |
| AL0097IBC    | Insights Agent        | [Failed to connect to Business Central API (Test Connection)](#AL0097IBC) |
| AL0098CTI    | Chat Session          | [Insights Agent used](#AL0098CTI)                        |
| AL0099INS    | Insights Agent        | [Insights Agent Feature Uptake](#AL0099INS)              |
| AL0100IAW    | Insights Agent        | [Insights Agent Discovered (Feature Uptake)](#AL0100IAW) |
| AL0101IWS    | Insights Agent        | [Insights Agent Wizard opened from Notification](#AL0101IWS)|
| AL0102IAD    | Insights Agent        | [Insights Agent notification dismissed](#AL0102IAD)      |
| AL0103IAS    | Insights Agent        | [Insights Agent notification shown](#AL0103IAS)          |
| AL0104IAD    | Insights Agent        | [Insights Agent setup discovered](#AL0104IAD)            |
| AL0105IAC    | Insights Agent        | [Insights Agent setup changed](#AL0105IAC)               |
| AL0106IAW    | Insights Agent        | [Insights Agent Wizard discovered](#AL0106IAW)           |
| AL0107IAX    | Insights Agent        | [Insights Agent Wizard setup completed](#AL0107IAX)      |
| AL0108IAY    | Insights Agent        | [Insights Agent setup completed](#AL0108IAY)             |
| PY0065CHS    | Chat Session          | [Chat session started](#PY0065CHS)                       |
| PY0066CHQ    | Chat Question         | [New question asked](#PY0066CHQ)                         |
| PY0067CHQ    | Chat Question         | [Follow-up Question Asked](#PY0067CHQ)                   |
| PY0068CHA    | Chat Answer           | [Answer generated](#PY0068CHA)                           |
| PY0069CHL    | Chat Session          | [Maximum monthly requests limit reached](#PY0069CHL)     |
| PY0070CHR    | Chat Question         | [Question rephrased](#PY0070CHR)                         |
| PY0071CHP    | Chat Answer           | [Private Knowledge Found](#PY0071CHP)                    |
| PY0072CHM    | Chat Session          | [Microsoft Learn Found](#PY0072CHM)                      |
| PY0073CHC    | Chat Session          | [Community Knowledge Found](#PY0073CHC)                  |
| PY0074CHF    | Chat Answer           | [Positive Feedback](#PY0074CHF)                          |
| PY0075CHF    | Chat Answer           | [Negative Feedback](#PY0075CHF)                          |
| PY0076CCE    | Chat Session          | [Invalid Access Token](#PY0076CCE)                       |
| PY0077CCE    | Chat Session          | [Access Token is missing](#PY0077CCE)                    |
| PY0078CCE    | Chat Session          | [Chat Id is missing](#PY0078CCE)                         |
| PY0079CCE    | Chat Session          | [Secret Key is missing](#PY0079CCE)                      |
| PY0080CCE    | Chat Session          | [Authentication failed](#PY0080CCE)                      |
| PY0081CCS    | Chat Session          | [Authenticated successfully](#PY0081CCS)                 |
| PY0082CHR    | Chat Question         | [Related Queries Generated](#PY0082CHR)                  |
| PY0085CHI    | Intent Detection      | [Intent Detected](#PY0085CHI)                            |
| PY0086CHE    | Data Insights         | [Data Insights API Fetch Unexpected Error](#PY0086CHE)   |
| PY0087CHG    | Data Insights         | [Data Insights Code Generated](#PY0087CHG)               |
| PY0088CHA    | Data Insights         | [Data Insights Result Generated](#PY0088CHA)             |
| PY0089CHS    | Data Insights         | [Data Insights Code Executed Successfully](#PY0089CHS)   |
| PY0090CHE    | Data Insights         | [Data Insights Helper Code Error](#PY0090CHE)            |
| PY0091CHE    | Data Insights         | [Data Insights Build Script Error](#PY0091CHE)           |
| PY0092CHE    | Data Insights         | [Data Insights Execution Error](#PY0092CHE)              |
| PY0093CHI    | Data Insights         | [Data Insights Result Interpreted](#PY0093CHI)           |
| PY0094CHE    | Data Insights         | [Data Insights Interpret Error](#PY0094CHE)              |
| PY0095CHG    | Data Insights         | [Data Insights Corrected Code Generated](#PY0095CHG)     |

## Business Central Telemetry Events

### <a id="AL0001CHS"></a>AL0001CHS - Chat Session Started
This event is triggered when a user begins a new chat session, allowing us to understand user engagement.

### <a id="AL0021UNS"></a>AL0021UNS - App Uninstalled from Business Central
This event is important for understanding the app's lifecycle and reasons for uninstallation.

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

### <a id="AL0033IAE"></a>AL0033IAE - Insights Agent Enabled
This event is triggered when the Insights Agent is enabled.

### <a id="AL0034IAD"></a>AL0034IAD - Insights Agent Disabled
This event is triggered when the Insights Agent is disabled.

### <a id="AL0035IAS"></a>AL0035IAS - Setup Insights Agent Opened from Setup
This event is triggered when the Insights Agent setup is opened from the Setup page.

### <a id="AL0033FUD"></a>AL0033FUD - File Upload Initiated
This event is triggered when a user initiates a file upload, allowing us to understand user engagement.

### <a id="AL0034FUS"></a>AL0034FUS - File Upload Started
This event is triggered when a user starts a file upload, allowing us to understand user engagement.

### <a id="AL0035FUP"></a>AL0035FUP - File Passed Validation
This event is triggered when a user passes file validation, allowing us to understand user engagement.

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

### <a id="AL0066FPD"></a>AL0066FPD - Page Scripting File Upload Initiated
This event is triggered when a user initiates a page scripting file upload.

### <a id="AL0067FPS"></a>AL0067FPS - Page Scripting File Upload Started
This event is triggered when a user starts a page scripting file upload.

### <a id="AL0068FPP"></a>AL0068FPP - Page Scripting File Passed Validation
This event is triggered when a user passes page scripting file validation.

### <a id="AL0069FPC"></a>AL0069FPC - Page Scripting File Upload Completed
This event is triggered when a user completes a page scripting file upload.

### <a id="AL0070UPD"></a>AL0070UPD - Page Scripting Url Upload Initiated
This event is triggered when a user initiates a page scripting url upload.

### <a id="AL0071UPS"></a>AL0071UPS - Page Scripting Url Upload Started
This event is triggered when a user starts a page scripting url upload.

### <a id="AL0072UPP"></a>AL0072UPP - Page Scripting Url Passed Validation
This event is triggered when a user passes page scripting url validation.

### <a id="AL0073UPC"></a>AL0073UPC - Page Scripting Url Upload Completed
This event is triggered when a user completes a page scripting url upload.

### <a id="AL0074FPD"></a>AL0074FPD - Page Scripting User Manual Edit Initiated
This event is triggered when a user initiates a generated page scripting user manual edit.

### <a id="AL0075FPS"></a>AL0075FPS - Page Scripting User Manual Edit Started
This event is triggered when a user starts a generated page scripting user manual edit.

### <a id="AL0076FPC"></a>AL0076FPC - Page Scripting User Manual Edit Completed
This event is triggered when a user completes a generated page scripting user manual edit.

### <a id="AL0077FDD"></a>AL0077FDD - User Manual Download to Word Initiated
This event is triggered when a user initiates a user manual download to Word.

### <a id="AL0078FDS"></a>AL0078FDS - User Manual Download to Word Started
This event is triggered when a user starts a user manual download to Word.

### <a id="AL0079FDC"></a>AL0079FDC - User Manual Download to Word Completed
This event is triggered when a user completes a user manual download to Word.

### <a id="AL0080FDD"></a>AL0080FDD - User Manual Download to MD Initiated
This event is triggered when a user initiates a user manual download to Markdown.

### <a id="AL0081FDS"></a>AL0081FDS - User Manual Download to MD Started
This event is triggered when a user starts a user manual download to Markdown.

### <a id="AL0082FDC"></a>AL0082FDC - User Manual Download to MD Completed
This event is triggered when a user completes a user manual download to Markdown.

### <a id="AL0083CSD"></a>AL0083CSD - Setup Record Deleted, Associated Secrets Cleared
This event is triggered when a setup record is deleted, and associated secrets are cleared.

### <a id="AL0084IAS"></a>AL0084IAS - Insights Agent Client Secret is Cleared
This event is triggered when the Insights Agent client secret is cleared.

### <a id="AL0085IAT"></a>AL0085IAT - Insights Agent Client Secret is Set
This event is triggered when the Insights Agent client secret is set.

### <a id="AL0086IAU"></a>AL0086IAU - Insights Agent Client Secret is Not Set
This event is triggered when an attempt to get the Insights Agent client secret finds it is not set.

### <a id="AL0087IAV"></a>AL0087IAV - Insights Agent Client Secret Get Failed
This event is triggered when getting the Insights Agent client secret fails due to an IsolatedStorage issue.

### <a id="AL0088CCC"></a>AL0088CCC - CentralQ Cloud Connection Cleared (Table Trigger)
This event is triggered when the CentralQ Cloud connection is cleared via a table trigger.

### <a id="AL0089IAC"></a>AL0089IAC - Insights Agent Setup Cleared (Table Trigger)
This event is triggered when the Insights Agent setup is cleared via a table trigger.

### <a id="AL0090IAC"></a>AL0090IAC - Insights Agent Setup Cleared via Setup Page Action
This event is triggered when the Insights Agent setup is cleared via an action on the Setup Page.

### <a id="AL0091CCC"></a>AL0091CCC - CentralQ Cloud Connection Cleared via Setup Page Action
This event is triggered when the CentralQ Cloud connection is cleared via an action on the Setup Page.

### <a id="AL0092IBD"></a>AL0092IBD - Failed to Acquire Access Token (HTTP Send Error)
This event is triggered when acquiring the access token fails due to an HTTP send error.

### <a id="AL0093IBE"></a>AL0093IBE - Failed to Acquire Access Token (HTTP Non-success Status)
This event is triggered when acquiring the access token fails because the HTTP response status was not successful.

### <a id="AL0094IBF"></a>AL0094IBF - Failed to Acquire Access Token (Token Not Found in Response)
This event is triggered when acquiring the access token fails because the token was not found in the HTTP response.

### <a id="AL0095IAZ"></a>AL0095IAZ - Access Token Acquired Successfully
This event is triggered when the access token is acquired successfully.

### <a id="AL0096IBB"></a>AL0096IBB - Successfully Connected to Business Central API (Test Connection)
This event is triggered when the connection test to the Business Central API is successful.

### <a id="AL0097IBC"></a>AL0097IBC - Failed to Connect to Business Central API (Test Connection)
This event is triggered when the connection test to the Business Central API fails.

### <a id="AL0098CTI"></a>AL0098CTI - Insights Agent Used
This event is triggered when the Insights Agent is used during a chat session.

### <a id="AL0099INS"></a>AL0099INS - Insights Agent Feature Uptake
This event is triggered to log the uptake status of the Insights Agent feature, specifically when it's used.

### <a id="AL0100IAW"></a>AL0100IAW - Insights Agent Discovered (Feature Uptake)
This event is triggered when the Insights Agent feature is discovered by the user, typically via a notification or wizard prompt.

### <a id="AL0101IWS"></a>AL0101IWS - Insights Agent Wizard Opened from Notification
This event is triggered when the Insights Agent setup wizard is opened directly from the enablement notification.

### <a id="AL0102IAD"></a>AL0102IAD - Insights Agent Notification Dismissed
This event is triggered when the user dismisses the notification prompting them to enable the Insights Agent.

### <a id="AL0103IAS"></a>AL0103IAS - Insights Agent Notification Shown
This event is triggered when the notification prompting the user to enable the Insights Agent is shown.

### <a id="AL0104IAD"></a>AL0104IAD - Insights Agent Setup Discovered
This event is triggered when the Insights Agent feature is discovered in the Setup page.

### <a id="AL0105IAC"></a>AL0105IAC - Insights Agent Setup Changed
This event is triggered when Insights Agent setup is changed in the Setup page.

### <a id="AL0106IAW"></a>AL0106IAW - Insights Agent Wizard Discovered
This event is triggered when the Insights Agent Wizard page is opened/discovered.

### <a id="AL0107IAX"></a>AL0107IAX - Insights Agent Wizard Setup Completed
This event is triggered when the Insights Agent Wizard setup process is completed successfully.

### <a id="AL0108IAY"></a>AL0108IAY - Insights Agent Setup Completed
This event is triggered when the Insights Agent setup is fully completed.

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

### <a id="PY0074CHF"></a>PY0074CHF - Positive Feedback
This event is triggered when a user submits positive feedback for the answer. Answer text is included in the event, as well as the conversation history and sources used to generate the answer (with text and metadata).

### <a id="PY0075CHF"></a>PY0075CHF - Negative Feedback
This event is triggered when a user submits negative feedback for the answer. Answer text is included in the event, as well as the conversation history and sources used to generate the answer (with text and metadata).

### <a id="PY0076CCE"></a>PY0076CCE - Invalid Access Token
This event is triggered when a user fails to authenticate to CentralQ Cloud, due to Access token is not valid.

### <a id="PY0077CCE"></a>PY0077CCE - Access Token is Missing
This event is triggered when a user fails to authenticate to CentralQ Cloud, due to Access token is missing.

### <a id="PY0078CCE"></a>PY0078CCE - Chat Id is Missing
This event is triggered when a user fails to authenticate to CentralQ Cloud, due to Chat Id is missing.

### <a id="PY0079CCE"></a>PY0079CCE - Secret Key is Missing
This event is triggered when a user fails to authenticate to CentralQ Cloud, due to Secret Key is missing.

### <a id="PY0080CCE"></a>PY0080CCE - Authentication Failed
This event is triggered when a user fails to authenticate to CentralQ Cloud.

### <a id="PY0081CCS"></a>PY0081CCS - Authenticated Successfully
This event is triggered when a user successfully authenticates to CentralQ Cloud.

### <a id="PY0082CHR"></a>PY0082CHR - Related Queries Generated
This event is triggered when related queries are generated for the question. Question text is included in the event, as well as related queries.

### <a id="PY0085CHI"></a>PY0085CHI - Intent Detected
This event is triggered when the intent of a user's query is detected, determining whether it's a guidance question or a data insights question.

### <a id="PY0086CHE"></a>PY0086CHE - Data Insights API Fetch Unexpected Error
This event is triggered when an unexpected error occurs during fetching APIs for the Data Insights agent.

### <a id="PY0087CHG"></a>PY0087CHG - Data Insights Code Generated
This event is triggered when Python code is successfully generated by the LLM for a data insights query.

### <a id="PY0088CHA"></a>PY0088CHA - Data Insights Result Generated
This event is triggered when the Data Insights agent successfully completes a data analysis and generates results.

### <a id="PY0089CHS"></a>PY0089CHS - Data Insights Code Executed Successfully
This event is triggered when the Python code generated for data analysis executes successfully and returns a valid result dictionary.

### <a id="PY0090CHE"></a>PY0090CHE - Data Insights Helper Code Error
This event is triggered when there's an error loading the helper code for the Data Insights agent.

### <a id="PY0091CHE"></a>PY0091CHE - Data Insights Build Script Error
This event is triggered when there's an unexpected error during the building of the execution script for data analysis.

### <a id="PY0092CHE"></a>PY0092CHE - Data Insights Execution Error
This event is triggered when there's an error during the execution of the generated Python code for data analysis.

### <a id="PY0093CHI"></a>PY0093CHI - Data Insights Result Interpreted
This event is triggered when the Data Insights agent successfully interprets the results of the data analysis.

### <a id="PY0094CHE"></a>PY0094CHE - Data Insights Interpret Error
This event is triggered when there's an error during the interpretation of data analysis results.

### <a id="PY0095CHG"></a>PY0095CHG - Data Insights Corrected Code Generated
This event is triggered when the LLM generates corrected Python code after an execution failure. This helps track how often code corrections are needed and their performance characteristics. The event includes telemetry data about the correction process such as input/output tokens, generation time, and other contextual information.

## Telemetry Data Compliance
All telemetry data is collected in compliance with privacy laws and regulations. Users are informed of the data collection.