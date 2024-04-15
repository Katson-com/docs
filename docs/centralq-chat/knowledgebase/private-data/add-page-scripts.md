## Importing Page Scripting to CentralQ Knowledgebase

CentralQ Chat enables users to enhance their knowledge base by importing page scripting from a YAML file or link. This feature generates a user manual in the current Business Central language and also integrates it into the CentralQ knowledgebase for use in chat responses. 

### Page Scripting Recording
[Page Scripting](https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-page-scripting?wt.mc_id=DX-MVP-5003099) is a feature available from the Business Central version `24.0` that allows users to record their interactions with the user interface (UI) and replay them to replicate the exact same actions in the UI.

You will need a recording file in YAML format or a link to the recording to import it into CentralQ Chat.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934826292?h=21e1492450&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Recording Steps With Page Scripting"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

!!! note "Add Description"
    For best results, add a description to the page script, as shown in the video.

### Importing Page Scripting Recording Files

Once you have the YAML file, follow these steps to import the page scripting into CentralQ Chat:

1. **Navigate to CentralQ Chat**: Access the Business Manager Role Center and locate the CentralQ Chat.
2. **Access Private Data**: Within the CentralQ Chat, select the `Private Data` to manage your files.
3. **Import the Recording File**: Click on `Import Recording` and upload your YAML file. 

    <div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934942288?h=159c7af6ee&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Import Recording (Yaml) file"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

4. **Completion**: After the file is uploaded, it is processed, and a user manual is automatically generated and added to your knowledgebase. The status of the import can be viewed in the Private Data section.

### Using the Generated User Manual

Once imported, the manual is available for immediate use within CentralQ Chat responses. If a query related to the imported script is asked, the relevant section from the manual is used as a response, enhancing user support.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934950995?h=1e8f35d01b&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Page Scripting Retrieval"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

- **Interactive Link**: Each response derived from the manual includes a link to the source recording URL. Users can click this link to view and run the page scripting workflow directly.

### Editing and Exporting the Manual

#### Modifications 
You can edit the manual directly within the CentralQ interface to refine the content or update any changes.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934955419?h=8cbb15c4de&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Edit User Manual Generated From Page Scripting"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

**Export Options**: If necessary, export the manual to Word format or `Yaml` file for external use or archiving.

#### Export to Word
To export the manual to Word format, follow these steps: `CentralQ Chat` > `Private Data` > `Export to Word`

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934960176?h=f28a82581a&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="ps-video-manual-export-to-word-formatted"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

!!! note "Changing in Word"
    You can change the content in Word, but the changes will not be reflected in the CentralQ Chat knowledgebase. To update the manual you can copy-paste the content back into the `CentralQ Chat` > `Private Data` > `User Manual` page. If you will import the updated document using the `Upload File` feature, the manual will be duplicated and this will decrease the chat quality, as two manuals will be available for the same topic.

#### Export to Yaml
To export the manual to a `Yaml` file, follow these steps: `CentralQ Chat` > `Private Data` > `Download File`

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934967268?h=b40db6a52b&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Export Page Scripting as Yaml"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

!!! note "Changing in Yaml"
    You can change the content in Yaml, but the changes will not be reflected in the CentralQ Chat knowledgebase. To update the manual you will need to [replace](../add-files/#replacing-files) existing recording file.

### Importing Page Scripting Recording Links

If you have a recording link instead of a file, follow these steps to import the page scripting into CentralQ Chat:

1. **Navigate to CentralQ Chat**: Access the Business Manager Role Center and locate the CentralQ Chat.
2. **Access Private Data**: Within the CentralQ Chat, select the `Private Data` to manage your files.
3. **Import the Recording Link**: Click on `Import Recording Link` and paste the link to the recording.

    <div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934975870?h=88d194b370&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Page Scripting Import Link"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

4. **Completion**: After the link is processed, a user manual is automatically generated and added to your knowledgebase. The status of the import can be viewed in the Private Data section.

### Muli-Language Support

CentralQ Chat supports multiple languages for page scripting. The user manual is generated in the current Business Central language (`Setup` > `My Settings` > `Language`), ensuring that the content is relevant and accurate for the user.

<div style="padding:57.01% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/934992661?h=a01cdf6966&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="CentralQ Chat - Multilanguage Page Scripting User Manual"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

!!! note "Chat Language"
    Once the manual is imported, it is available in the chat, even if the chat language differs from the user manual language.
