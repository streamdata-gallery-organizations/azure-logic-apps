{
  "info": {
    "name": "Azure Logic Apps API Partners Get",
    "_postman_id": "bbee82ea-55d7-4696-a1eb-c98ff5e0eb68",
    "description": "Gets an integration account partner.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "partners",
      "item": [
        {
          "id": "64fe92f5-ed45-4b1c-9dc2-51869fd71bf4",
          "name": "Partners_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/integrationAccounts/:integrationAccountName/partners/:partnerName"
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
                  "id": "partnerName",
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
            "description": "Gets an integration account partner"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d11a7e4-4e93-488e-86ce-85cbbc3029ca"
            }
          ]
        }
      ]
    }
  ]
}