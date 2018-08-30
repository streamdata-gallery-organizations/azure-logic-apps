{
  "info": {
    "name": "Azure Logic Apps API Partners List By Integration Accounts",
    "_postman_id": "22cfef13-10c4-4ea5-ada0-ec9750336a5b",
    "description": "Gets a list of integration account partners.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "partners integration accounts",
      "item": [
        {
          "id": "5b1bc547-e44a-49a5-b7cc-34ee7e8e046d",
          "name": "Partners_ListByIntegrationAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/integrationAccounts/:integrationAccountName/partners"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "description": "Gets a list of integration account partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c82d2d9b-7fd4-4639-a8f9-e0bf6a2e763b"
            }
          ]
        }
      ]
    }
  ]
}