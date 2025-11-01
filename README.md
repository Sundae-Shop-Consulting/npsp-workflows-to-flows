# npsp-workflows-to-flows

This is a small project to replace workflow rules packaged as part of the Nonprofit Success Pack with flows. These still need to be tested before being considered production ready. 

### Install links
- [Install in a dev org](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tbm000000CXoD)
- [install in a sandbox or scratch org](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tbm000000CXoD)

Once the package is installed you will still need to activate the flows:
- Opportunity: Copy FMV to Amount
- Contact: Email Changed
- Contact: Phone Changed

This package does not include the Opportunity Email Acknowledgment workflow. The email alert from that workflow requires significant customization to be useful in its current state, so you might as well make the whole thing from the scratch. 

## Development

This project was developed using CumulusCI. To work on this project in a scratch org:

1. [Set up CumulusCI](https://cumulusci.readthedocs.io/en/latest/tutorial.html)
2. Run `cci flow run dev_org --org dev` to deploy this project.
3. Run `cci org browser dev` to open the org in your browser.
