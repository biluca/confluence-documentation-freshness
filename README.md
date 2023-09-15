# Confluence Documentation Freshness

No team can operate without documentation regardless of its size and type of activity. They must be clear, precise, and easily accessible by all concerned. It is also vital that this documentation is up-to-date, incorporating the latest evolutions and changes while eliminating obsolete items. In summary, documents must be updated to be applicable. By being updated, the documentation is getting rid of outdated information. This greatly reduces the risk of making mistakes, sending erroneous instructions to new team members, and ending up with obsolete documentation. That being said, we’ve established a workflow that will help to review & maintain the Custom Integrations Documentation up-to-date.

## Documentation Freshness Categorization

At regular intervals, the team will gather in a Meeting and will run the analysis of the documentation, categorizing them into 5 categories:

- Baby Doc
- Recent
- Fresh
- Check-Up
- Old Doc

As the names are suggesting, each category describes how long the documentation has been without an update. This categorization will help the team to build a backlog of documentation that needs to be reviewed. This backlog will be estimated and prioritized, and a plan will be elaborate.

## Freshness Parameters

- **Baby Doc**  - 0 to 60        - Light Blue  - It was update within 2 months
- **Recent**    - 61 to 130      - Blue        - It was update within 1.5 Quarter
- **Fresh**     - 131 to 270     - Green       - It was update within 3 Quarters
- **Check-up**  - 271 to 340     - Yellow      - It was update within 5 Quarters
- **Old Doc**   - 341 to 450+    - Red         - It was updated  a long time ago

## Running the Application

### Change the Environment File removing the *.sample* extension.


```sh
As is: confluence_data_freshness/confluence_data_retriever/.env.sample

To be: confluence_data_freshness/confluence_data_retriever/.env
```

You should have access to the **BASIC_AUTH_TOKEN** provided by the Confluence API Security Dashboard. That way the application will be able to make calls to the Confluence API.

### Run the Application

```sh
python manage.py runserver
```
