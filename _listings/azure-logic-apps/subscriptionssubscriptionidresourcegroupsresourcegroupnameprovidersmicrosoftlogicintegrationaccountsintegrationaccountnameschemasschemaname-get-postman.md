{
  "info": {
    "name": "Azure Logic Apps API Schemas Get",
    "_postman_id": "57ffc1ea-a8d1-4793-b448-b1c18ac2484b",
    "description": "Gets an integration account schema.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "schemas",
      "item": [
        {
          "id": "20593412-9da1-4958-b34f-70b8ef25486b",
          "name": "Schemas_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/integrationAccounts/:integrationAccountName/schemas/:schemaName"
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
                  "id": "schemaName",
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
            "description": "Gets an integration account schema"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca929e49-1b4a-4468-9c4c-6dfd0028eba5"
            }
          ]
        }
      ]
    }
  ]
}