[![Board Status](https://dev.azure.com/executech/d9801214-ce08-4062-b742-24ee756e36f2/664aae17-a5c0-477e-b4ef-8d011773dadf/_apis/work/boardbadge/fb0b109c-ada9-4bc4-9304-2b8da2212236)](https://dev.azure.com/executech/d9801214-ce08-4062-b742-24ee756e36f2/_boards/board/t/664aae17-a5c0-477e-b4ef-8d011773dadf/Microsoft.RequirementCategory)
# Azure

- Create a new function app inside the Azure Portal.
- In platform features tab, select deployment credentials
- Select setup and choose deployment source as External Repository.
- Enter https://github.com/executechit/ConnectWise-MSTeams.git as the source.
- In your Azure function app Application Settings add a new setting with the name as your connectwise service board name and the value as the webhook url of the MS teams channel you want to post to. To get the webhook url, right click the channel and select connectors. Configure a webhook.



# Connectwise

- Create a new Integrator login
- Select All Records
- Set Service ticket callback url to https://<functionappname>.azurewebsites.net/api/CWIncoming?serviceid=
