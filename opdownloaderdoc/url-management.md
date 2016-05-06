# URL Management

## 1. URL Structure
Your URL will be defined by the domain where content gets published, docset name(base url), folder structure, and file names in your repo. 

 `http://{site}/{BaseURL}{ContentPath}`

**Parameter**|**Required**|**Source**|**Description**  
---------|---------|---------|---------|---------
Site| Required | Publishing metadata set at account provisioning | The URLs to the host name of the Web app that renders the content. It can be the URL for public site, internal testing or staging environment, or even localhost of local preview. Not related to git directory structure
BaseURL | Required | Base URL which maps to the starting folder of the docset
ContentPath | Required | File name in [GIT repository](repo-config.md) | A path structure for a content item that authors their content. This path structure is the folder path of a content item in a repo, including the markdown file name without extension

### 1.1 Example
http://trustcenterchina-sandboxlive.azurewebsites.net/trustcenter/homepage.html
- Corresponding Git repository https://github.com/Microsoft/trustcenterchina-sandbox/blob/live/trustcenter/homepage.md
- Site: trustcenterchina-sandboxlive.azurewebsites.net
- BaseURL: trustcenter
- ContentPath: homepage.html

With this URL schema defined, content author and site management are given great flexibility in the layout of the content files in repo as well as rendering URLs. 