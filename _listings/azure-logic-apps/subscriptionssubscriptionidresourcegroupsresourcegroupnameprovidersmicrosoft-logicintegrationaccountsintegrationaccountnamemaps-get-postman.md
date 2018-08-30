{
  "info": {
    "name": "Azure Logic Apps API Maps List By Integration Accounts",
    "_postman_id": "6c103eb2-7c38-4638-a9da-87f0622545e4",
    "description": "Gets a list of integration account maps.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "maps integration accounts",
      "item": [
        {
          "id": "2a36e20a-4b91-4b70-ad19-3b6cae42bbf5",
          "name": "Maps_ListByIntegrationAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/integrationAccounts/:integrationAccountName/maps"
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
            "description": "Gets a list of integration account maps"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e765fdd-6029-4512-a7ea-e06506f733c3"
            }
          ]
        }
      ]
    }
  ]
}