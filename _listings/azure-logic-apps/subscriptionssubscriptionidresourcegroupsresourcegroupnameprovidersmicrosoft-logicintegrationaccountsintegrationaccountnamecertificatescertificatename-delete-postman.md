{
  "info": {
    "name": "Azure Logic Apps API Certificates Delete",
    "_postman_id": "6c6efa88-6bea-41f7-88f7-12ab992b188f",
    "description": "Deletes an integration account certificate.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "certificates",
      "item": [
        {
          "id": "1b877fcd-70fd-4855-9ce1-a485f69cc87c",
          "name": "Certificates_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an integration account certificate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff5abb9b-5176-4193-b4ae-3b974595685f"
            }
          ]
        }
      ]
    }
  ]
}