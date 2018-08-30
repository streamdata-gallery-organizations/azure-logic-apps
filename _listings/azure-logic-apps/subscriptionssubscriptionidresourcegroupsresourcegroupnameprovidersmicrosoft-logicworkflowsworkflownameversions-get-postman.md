{
  "info": {
    "name": "Azure Logic Apps API Workflow Versions List",
    "_postman_id": "1f101110-49b5-4845-baeb-56056126f1b6",
    "description": "Gets a list of workflow versions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflow versions",
      "item": [
        {
          "id": "da8a36e3-4dc5-44da-a9b9-0984deb6eff3",
          "name": "WorkflowVersions_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/workflows/:workflowName/versions"
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
                  "id": "resourceGroupName",
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
            "description": "Gets a list of workflow versions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e129332-30ba-4fc4-a0f5-754c4697b6ff"
            }
          ]
        }
      ]
    }
  ]
}