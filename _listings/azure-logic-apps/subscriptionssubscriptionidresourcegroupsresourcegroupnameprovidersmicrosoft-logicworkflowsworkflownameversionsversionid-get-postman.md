{
  "info": {
    "name": "Azure Logic Apps API Workflow Versions Get",
    "_postman_id": "2377ab87-f270-4a61-b830-ef76798f7715",
    "description": "Gets a workflow version.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflow versions",
      "item": [
        {
          "id": "49ce1730-c4bf-4623-b68e-dbf6bf7e1483",
          "name": "WorkflowVersions_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/workflows/:workflowName/versions/:versionId"
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "versionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "workflowName",
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
            "description": "Gets a workflow version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8721f086-c3a5-42c5-a54a-db77c88a8f07"
            }
          ]
        }
      ]
    }
  ]
}