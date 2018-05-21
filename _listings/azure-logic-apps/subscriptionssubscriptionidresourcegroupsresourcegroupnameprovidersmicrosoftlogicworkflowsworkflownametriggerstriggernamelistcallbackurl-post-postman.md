{
  "info": {
    "name": "Azure Logic Apps API Workflow Triggers List Callback Url",
    "_postman_id": "836eef41-f87d-4f8f-8682-664eb520fd67",
    "description": "Gets the callback URL for a workflow trigger.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "workflow triggers callback url",
      "item": [
        {
          "id": "f788ceb1-6fc8-490a-991d-c6bbb7626391",
          "name": "WorkflowTriggers_ListCallbackUrl",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/workflows/:workflowName/triggers/:triggerName/listCallbackUrl"
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
                  "id": "triggerName",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the callback URL for a workflow trigger"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb39b627-a91b-4667-a1f2-7034043fa5ec"
            }
          ]
        }
      ]
    }
  ]
}