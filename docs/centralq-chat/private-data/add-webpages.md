## Adding Webpages

CentralQ Chat allows users to enrich their private knowledge base by adding URLs to publicly available webpages. This feature enables CentralQ Chat to scrape text from webpages and embed the content into the cloud vector database for use in chat responses.

### How to Add URLs

1. **Accessing URL Addition**: Navigate to `Search > CentralQ Chat > Private Data` or `Search > CentralQ Chat Setup > Private Data`.
2. **Adding the URL**: Click on `Add URL`, enter the webpage URL, and submit.
3. **Status and Insights**: After submitting, you can view the URL's status in the Private Data list. The status might show as `Processing` or `Ready`. AI-generated summaries and token counts are visible in the Insights factbox.
4. **Error Handling**: In case of an error, an error message will be displayed.

### Considerations for Adding URLs

- **Webpage Content**: CentralQ Chat scrapes and processes only the text content of the webpage. Video URLs or webpages with non-textual content are currently not supported.
- **Public Accessibility**: Ensure that the URL points to a publicly accessible webpage.
- **One-Page Limitation**: CentralQ Chat adds only the specified webpage. It does not scrape or include any linked or child pages.

    !!! note "Note"
        Only the content of the provided URL is added to CentralQ Chat. Linked or child pages are not included in the scraping process.

- **No Storage in Business Central**: URLs do not impact Business Central's database size as the data is stored externally.

    !!! note "No Impact on Database Size"
        Added URLs do not increase the size of your Business Central environment, ensuring efficient database management.


### Deletion and Replacement

URLs can be deleted or replaced similarly to files. Be cautious, as deletions are irreversible and replacements require the same URL for smooth transition.

!!! warning "Important"
    Changes to URLs are permanent and cannot be undone. Exercise caution when deleting or replacing URLs.