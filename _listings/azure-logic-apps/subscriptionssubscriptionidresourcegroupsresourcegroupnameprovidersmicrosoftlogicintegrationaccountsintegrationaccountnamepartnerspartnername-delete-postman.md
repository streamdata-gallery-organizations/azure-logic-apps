{
  "info": {
    "name": "Azure Logic Apps API Partners Delete",
    "_postman_id": "353fb182-23ec-40b0-a00f-3d7f63fe89ff",
    "description": "Deletes an integration account partner.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "partners",
      "item": [
        {
          "id": "4342085c-6e9b-4e1c-a4ac-f9c04d352958",
          "name": "Partners_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an integration account partner"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eeae8a30-bddd-46a9-bb4b-f790c7e07e15"
            }
          ]
        }
      ]
    }
  ]
}