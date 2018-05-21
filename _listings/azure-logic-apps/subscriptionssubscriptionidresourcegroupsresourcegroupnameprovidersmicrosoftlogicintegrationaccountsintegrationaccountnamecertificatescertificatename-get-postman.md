{
  "info": {
    "name": "Azure Logic Apps API Certificates Get",
    "_postman_id": "67d8dc0f-a0da-457a-8d3f-6d3e421fb69e",
    "description": "Gets an integration account certificate.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "certificates",
      "item": [
        {
          "id": "688e622b-f236-423a-b65f-0304030ab799",
          "name": "Certificates_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/integrationAccounts/:integrationAccountName/certificates/:certificateName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "certificateName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "integrationAccountName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets an integration account certificate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae82896e-743d-4a43-944c-4406ac5a24cc"
            }
          ]
        }
      ]
    }
  ]
}