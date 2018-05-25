{
  "info": {
    "name": "Azure Logic Apps API Certificates List By Integration Accounts",
    "_postman_id": "3b3f94ff-4f4d-4139-b0ac-83c3d850d5e0",
    "description": "Gets a list of integration account certificates.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "certificates integration accounts",
      "item": [
        {
          "id": "c8402c1e-36ae-4b62-bd74-69a0b551444f",
          "name": "Certificates_ListByIntegrationAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/integrationAccounts/:integrationAccountName/certificates"
              ],
              "query": [
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Gets a list of integration account certificates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "677bb010-7782-419c-ac6c-6f96ace44b24"
            }
          ]
        }
      ]
    }
  ]
}