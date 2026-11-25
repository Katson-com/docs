## Importing Page Scripting to CentralQ Knowledgebase

CentralQ Chat enables users to enhance their knowledge base by importing page scripting from a YAML file or link. This feature generates a user manual in the current Business Central language and also integrates it into the CentralQ knowledgebase for use in chat responses. 

### Page Scripting Recording
[Page Scripting](https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-page-scripting?wt.mc_id=DX-MVP-5003099) is a feature available from the Business Central version `24.0` that allows users to record their interactions with the user interface (UI) and replay them to replicate the exact same actions in the UI.

You will need a recording file in YAML format or a link to the recording to import it into CentralQ Chat.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/b1c86dcd-b404-4f96-9c0c-25a344aeea9d?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Recording Steps With Page Scripting"></iframe></div>

!!! note "Add Description"
    For best results, add a description to the page script, as shown in the video.

### Importing Page Scripting Recording Files

Once you have the YAML file, follow these steps to import the page scripting into CentralQ Chat:

1. **Navigate to CentralQ Chat**: Access the Business Manager Role Center and locate the CentralQ Chat.
2. **Access Private Data**: Within the CentralQ Chat, select the `Private Data` to manage your files.
3. **Import the Recording File**: Click on `Import Recording` and upload your YAML file. 

    <div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/f91a2f69-ba5e-4b8b-b984-147c8bd6b329?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Import Recording (Yaml) file"></iframe></div>

4. **Completion**: After the file is uploaded, it is processed, and a user manual is automatically generated and added to your knowledgebase. The status of the import can be viewed in the Private Data section.

### Using the Generated User Manual

Once imported, the manual is available for immediate use within CentralQ Chat responses. If a query related to the imported script is asked, the relevant section from the manual is used as a response, enhancing user support.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/ea5e19b6-07b9-4f00-bdf7-154cd5d3ee04?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Page Scripting Retrieval"></iframe></div>

- **Interactive Link**: Each response derived from the manual includes a link to the source recording URL. Users can click this link to view and run the page scripting workflow directly.

### Editing and Exporting the Manual

#### Modifications 
You can edit the manual directly within the CentralQ interface to refine the content or update any changes.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/c6d47563-afe9-4a42-b21d-66a990c195ef?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Edit User Manual Generated From Page Scripting"></iframe></div>

**Export Options**: If necessary, export the manual to `Word`, `Markdown` or `Yaml` file for external use or archiving.

#### Export to Word
To export the manual to Word format, follow these steps: `CentralQ Chat` > `Private Data` > `Export to Word`

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/ffae5a41-c701-4c28-9009-b191773f0b08?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="ps-video-manual-export-to-word-formatted"></iframe></div>

!!! note "Changing in Word"
    You can change the content in Word, but the changes will not be reflected in the CentralQ Chat knowledgebase. To update the manual you can copy-paste the content back into the `CentralQ Chat` > `Private Data` > `User Manual` page. If you will import the updated document using the `Upload File` feature, the manual will be duplicated and this will decrease the chat quality, as two manuals will be available for the same topic.

#### Export to Markdown
To export the manual to Markdown format, follow these steps: `CentralQ Chat` > `Private Data` > `Export to Markdown`

<div style="padding:53.96% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/a16126e2-b042-49fc-8383-321d94ba3f78?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Export User Manual to Markdown"></iframe></div>

!!! warning "Changing in Markdown"
    You can change the content in Markdown, but the changes will not be reflected in the CentralQ Chat knowledgebase.
    
#### Export to Yaml
To export the manual to a `Yaml` file, follow these steps: `CentralQ Chat` > `Private Data` > `Download File`

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/82b3c197-40b2-494e-a7f7-3c068855646e?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Export Page Scripting as Yaml"></iframe></div>

!!! note "Changing in Yaml"
    You can change the content in Yaml, but the changes will not be reflected in the CentralQ Chat knowledgebase. To update the manual you will need to [replace](../add-files/#replacing-files) existing recording file.

### Importing Page Scripting Recording Links

If you have a recording link instead of a file, follow these steps to import the page scripting into CentralQ Chat:

1. **Navigate to CentralQ Chat**: Access the Business Manager Role Center and locate the CentralQ Chat.
2. **Access Private Data**: Within the CentralQ Chat, select the `Private Data` to manage your files.
3. **Import the Recording Link**: Click on `Import Recording Link` and paste the link to the recording.

    <div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/86a3eca8-20a4-43be-99ce-3599d32e9c8a?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Page Scripting Import Link"></iframe></div>

4. **Completion**: After the link is processed, a user manual is automatically generated and added to your knowledgebase. The status of the import can be viewed in the Private Data section.

### Muli-Language Support

CentralQ Chat supports multiple languages for page scripting. The user manual is generated in the current Business Central language (`Setup` > `My Settings` > `Language`), ensuring that the content is relevant and accurate for the user.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://iframe.mediadelivery.net/embed/820419/254d8fca-a54c-4b49-be6d-1f06779258b4?autoplay=false&amp;preload=true&amp;responsive=true" loading="lazy" allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture; fullscreen" style="border:0;position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Multilanguage Page Scripting User Manual"></iframe></div>

!!! note "Chat Language"
    Once the manual is imported, it is available in the chat, even if the chat language differs from the user manual language.
