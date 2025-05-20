# CentralQ Chat Release Notes

## 0.1.86.0 - [15 May 2025]

### New Features

- **Data Insights Agent:**
  CentralQ Chat now includes the powerful Data Insights Agent feature that enables users to analyze their Business Central data using natural language queries. Ask business questions directly in the chat interface and receive both textual answers and visual representations like charts and graphs. This feature transforms how users interact with their data by:
  
  - Providing natural language data analysis of live Business Central data
  - Generating visualizations to identify trends, patterns, and outliers
  - Supporting queries about sales, customers, inventory, financials, and more
  - Respecting user permissions to ensure data security
  - Offering transparent "Thoughts" sections to explain how answers are derived

### Compatibility
- This version is compatible with Business Central version 25.0 and later.

## 0.1.85.0 - [24 Sep 2024]

### Bug Fixes
- **Improved DateTime Parsing:** Enhanced the parsing of datetimes in private documents when the Business Central date format is set to a non-English language. This improvement ensures more accurate interpretation and processing of date-related information across various language settings.

### Compatibility
- This version is compatible with Business Central version 24.0 and later.

## 0.1.81.1 - [20 Sep 2024]

### Bug Fixes
- Fixed an issue where file uploads with non-ASCII characters in the filename were not being processed correctly. This resolves problems with importing files that have special characters or are named in non-English languages.

## Version 0.1.80.0 - [29 Apr 2024]

### New Features

- **Exporting User Manuals to Markdown Format:**
  Users can now export user manuals generated from page scripting to Markdown format. This feature provides additional flexibility for users who prefer to work with Markdown files, enabling seamless integration with other platforms and tools.

## Version 0.1.77.0 - [16 Apr 2024]

### New Features

- **Page Scripting Import to CentralQ Knowledgebase:**
  CentralQ Chat now supports the import of page scripting from YAML files or direct links. This enhancement allows for the automatic generation of user manuals in the current language of Business Central, which are then integrated into the CentralQ knowledgebase for immediate use in chat responses. Users can upload page scripting via the `Private Data` section under `CentralQ Chat`, enhancing the AI's ability to provide contextual answers based on the imported scripts.

- **Interactive Link Integration in Chat Responses:**
  Each chat response generated from the new user manuals includes an interactive link to the page script link. This feature enables users to directly view and execute the page scripting workflow, significantly improving the interactive experience within CentralQ Chat.

- **Editing and Exporting User Manuals:**
  Modifications to the generated user manuals can now be made directly within the CentralQ interface. Users have the flexibility to export these manuals to Word or YAML formats for external use or archiving, ensuring adaptability to various business needs.

- **Multi-Language Support for Page Scripting:**
  The import and automatic generation of user manuals now support multiple languages, aligning with the current settings in Business Central. This update ensures that all users, regardless of their selected language, receive accurate and understandable support from CentralQ Chat.


## Initial Release - Version 0.1.68.0 - [19 Jan 2024]

Welcome to the first release of CentralQ Chat, your comprehensive guide to Microsoft Business Central. This inaugural release brings together the power of AI and a vast repository of knowledge to enhance your Business Central experience.

### Features
- **Business Central Integration:** CentralQ Chat is fully integrated with Microsoft Business Central for seamless user experience.
- **AI-Driven Answers:** Utilizes AI to provide instant responses to queries about Business Central, based on various knowledge sources.
- **Chat:** Follow-up questions and answers are delivered in a conversational format, allowing for a more natural interaction.
- **Microsoft Learn Integration:** Access a wealth of information from Microsoft Learn directly within CentralQ Chat.
- **Community Knowledge Access:** Harness the power of community-sourced knowledge, including blogs, YouTube, tweets, and books.
- **Private Documentation Support:** Upload and use your private Business Central documents (PDF, Word, Text) for personalized answers.

### Known Issues
- **Context Window Limitation:** Due to AI model limitations, longer conversations may lead to loss of earlier context.

### Compatibility
- This version is compatible with Business Central version 23.0 and later.
<!-- RELEASE NOTES STRUCTURE -->
<!-- ---

## Version [Latest Version Number] - [Release Date]

### New Features
- **[Feature 1 Description]:** Brief explanation of the new feature.
- **[Feature 2 Description]:** Brief explanation of the new feature.
- ...additional features as applicable...

### Enhancements
- **[Enhancement 1]:** Description of the enhancement to existing functionality.
- **[Enhancement 2]:** Description of the enhancement to existing functionality.
- ...additional enhancements as applicable...

### Bug Fixes
- **[Bug Fix 1]:** Description of the bug fix.
- **[Bug Fix 2]:** Description of the bug fix.
- ...additional bug fixes as applicable...

### Known Issues
- **[Issue 1]:** Description of any known issues that are pending resolution.
- ...additional known issues as applicable...

## Version [Previous Version Number] - [Release Date]

### New Features
- ...new features for this version...

### Enhancements
- ...enhancements for this version...

### Bug Fixes
- ...bug fixes for this version...

### Known Issues
- ...known issues for this version...

...continue with past versions as applicable...