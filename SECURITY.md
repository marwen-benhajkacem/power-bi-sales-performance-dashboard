# Security and publication checklist

Before switching this repository to public visibility, verify all of the following:

- [ ] Confirm the dataset's exact origin and that its license permits redistribution.
- [ ] Inspect the rows in Power BI Desktop, including customer names/IDs, addresses, emails, phone numbers, order IDs, and any free-text fields.
- [ ] Check whether the data reveals confidential revenue, margins, supplier/customer relationships, or internal business performance.
- [ ] Check Power Query (`Transform data`) for local file paths, server names, database names, usernames, tokens, or private endpoints.
- [ ] Check model metadata, measures, calculated columns, hidden tables, and report filters for internal names or identifiers.
- [ ] Remove credentials and do not include `.env`, configuration files, or exported raw data.
- [ ] Confirm that any images, logos, and themes can be redistributed.
- [ ] Obtain written permission if the report or data came from an employer, client, school partner, or another organization with usage restrictions.

## Important

A `.pbix` file is not just a picture of the dashboard. It can contain the underlying imported data, model metadata, Power Query definitions, and report content. Hiding a visual or deleting a page does not necessarily remove data from the model.

If you cannot verify the dataset and redistribution rights, keep the GitHub repository **private** or publish only screenshots with sensitive details removed, after checking that the screenshots themselves are safe.
