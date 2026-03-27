Newforma Konekt stores project data and metadata differently and manages data across multiple regions.

### How Data Is Stored by Region

Newforma Konekt stores data differently depending on its type:

- **Project data**: All project-related data is stored within a specific region (e.g., Canada, US East, and Europe). Project-related data includes issues, models, sheets, comments, attachments, and other project information. Project data does not leave the region in which the project is hosted.

- **Metadata**: System-level data, such as user accounts and hub subscriptions, are global and may be stored and shared across multiple regions. Metadata does not contain project data.

### Available Hosting Regions

Newforma Konekt currently stores data in the following regions:

- Canada
- US East
- Europe

Each region includes both primary (active) and backup data storage locations.

### How Data Is Hosted

Within each region:

- Both Microsoft Azure and Amazon Web Services (AWS) are used.
- Each provider has active and backup infrastructure deployed within the same region, located in separate physical locations.

### Data Hosting by Feature

| Cloud provider | Activity center |
|---|---|
| AWS | RFIs<br>Submittals<br>Change Management<br>Emails |
| Azure | Authentication and users<br>Project files<br>Document Control<br>Sharing Center<br>Issues |

!!! info
    While metadata, such as user information, is stored in physical locations, it is replicated across regions using Azure Cosmos DB, making it effectively global.