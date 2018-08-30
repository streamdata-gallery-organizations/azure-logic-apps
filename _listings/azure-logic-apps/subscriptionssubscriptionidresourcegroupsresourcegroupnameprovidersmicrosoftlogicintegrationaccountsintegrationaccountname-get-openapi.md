---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Integration Accounts Get
  description: Gets an integration account.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.Logic/workflows:
    get:
      summary: Workflows List By Subscription
      description: Gets a list of workflows by subscription.
      operationId: Workflows_ListBySubscription
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftlogicworkflows-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Workflows Subscription
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows:
    get:
      summary: Workflows List By Resource Group
      description: Gets a list of workflows by resource group.
      operationId: Workflows_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflows-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Workflows Resource Group
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}:
    get:
      summary: Workflows Get
      description: Gets a workflow.
      operationId: Workflows_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows
    put:
      summary: Workflows Create Or Update
      description: Creates or updates a workflow.
      operationId: Workflows_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: body
        name: workflow
        description: The workflow
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows
    patch:
      summary: Workflows Update
      description: Updates a workflow.
      operationId: Workflows_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-patch
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: body
        name: workflow
        description: The workflow
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows
    delete:
      summary: Workflows Delete
      description: Deletes a workflow.
      operationId: Workflows_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflowname-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/disable:
    post:
      summary: Workflows Disable
      description: Disables a workflow.
      operationId: Workflows_Disable
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamedisable-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows Disable
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/enable:
    post:
      summary: Workflows Enable
      description: Enables a workflow.
      operationId: Workflows_Enable
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameenable-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows Enable
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/generateUpgradedDefinition
  : post:
      summary: Workflows Generate Upgraded Definition
      description: Generates the upgraded definition for a workflow.
      operationId: Workflows_GenerateUpgradedDefinition
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamegenerateupgradeddefinition-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for generating an upgraded definition
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows Generate Upgraded Definition
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/listSwagger
  : post:
      summary: Workflows List Swagger
      description: Gets an OpenAPI definition for the workflow.
      operationId: Workflows_ListSwagger
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamelistswagger-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows Swagger
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/regenerateAccessKey
  : post:
      summary: Workflows Regenerate Access Key
      description: Regenerates the callback URL access key for request triggers.
      operationId: Workflows_RegenerateAccessKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameregenerateaccesskey-post
      parameters:
      - in: body
        name: keyType
        description: The access key type
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows Regenerate Access Key
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/versions:
    get:
      summary: Workflow Versions List
      description: Gets a list of workflow versions.
      operationId: WorkflowVersions_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameversions-get
      parameters:
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Versions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/versions/{versionId}
  : get:
      summary: Workflow Versions Get
      description: Gets a workflow version.
      operationId: WorkflowVersions_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameversionsversionid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: versionId
        description: The workflow versionId
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Versions
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/triggers/:
    get:
      summary: Workflow Triggers List
      description: Gets a list of workflow triggers.
      operationId: WorkflowTriggers_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownametriggers-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Triggers
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/triggers/{triggerName}
  : get:
      summary: Workflow Triggers Get
      description: Gets a workflow trigger.
      operationId: WorkflowTriggers_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownametriggerstriggername-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: triggerName
        description: The workflow trigger name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Triggers
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/triggers/{triggerName}/run
  : post:
      summary: Workflow Triggers Run
      description: Runs a workflow trigger.
      operationId: WorkflowTriggers_Run
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownametriggerstriggernamerun-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: triggerName
        description: The workflow trigger name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Triggers Run
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/triggers/{triggerName}/listCallbackUrl
  : post:
      summary: Workflow Triggers List Callback Url
      description: Gets the callback URL for a workflow trigger.
      operationId: WorkflowTriggers_ListCallbackUrl
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownametriggerstriggernamelistcallbackurl-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: triggerName
        description: The workflow trigger name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Triggers Callback Url
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/versions/{versionId}/triggers/{triggerName}/listCallbackUrl
  : post:
      summary: Workflow Versions List Callback Url
      description: Lists the callback URL for a trigger of a workflow version.
      operationId: WorkflowVersions_ListCallbackUrl
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameversionsversionidtriggerstriggernamelistcallbackurl-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The callback URL parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: triggerName
        description: The workflow trigger name
      - in: path
        name: versionId
        description: The workflow versionId
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Versions Callback Url
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/triggers/{triggerName}/histories
  : get:
      summary: Workflow Trigger Histories List
      description: Gets a list of workflow trigger histories.
      operationId: WorkflowTriggerHistories_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownametriggerstriggernamehistories-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: triggerName
        description: The workflow trigger name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Trigger Histories
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/triggers/{triggerName}/histories/{historyName}
  : get:
      summary: Workflow Trigger Histories Get
      description: Gets a workflow trigger history.
      operationId: WorkflowTriggerHistories_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownametriggerstriggernamehistorieshistoryname-get
      parameters:
      - in: path
        name: historyName
        description: The workflow trigger history name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: triggerName
        description: The workflow trigger name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Trigger Histories
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/triggers/{triggerName}/histories/{historyName}/resubmit
  : post:
      summary: Workflow Trigger Histories Resubmit
      description: Resubmits a workflow run based on the trigger history.
      operationId: WorkflowTriggerHistories_Resubmit
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownametriggerstriggernamehistorieshistorynameresubmit-post
      parameters:
      - in: path
        name: historyName
        description: The workflow trigger history name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: triggerName
        description: The workflow trigger name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Trigger Histories Resubmit
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/runs:
    get:
      summary: Workflow Runs List
      description: Gets a list of workflow runs.
      operationId: WorkflowRuns_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownameruns-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Runs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/runs/{runName}
  : get:
      summary: Workflow Runs Get
      description: Gets a workflow run.
      operationId: WorkflowRuns_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamerunsrunname-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: runName
        description: The workflow run name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Runs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/runs/{runName}/cancel
  : post:
      summary: Workflow Runs Cancel
      description: Cancels a workflow run.
      operationId: WorkflowRuns_Cancel
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamerunsrunnamecancel-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: runName
        description: The workflow run name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Runs Cancel
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/runs/{runName}/actions
  : get:
      summary: Workflow Run Actions List
      description: Gets a list of workflow run actions.
      operationId: WorkflowRunActions_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamerunsrunnameactions-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: runName
        description: The workflow run name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Run Actions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/runs/{runName}/actions/{actionName}
  : get:
      summary: Workflow Run Actions Get
      description: Gets a workflow run action.
      operationId: WorkflowRunActions_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamerunsrunnameactionsactionname-get
      parameters:
      - in: path
        name: actionName
        description: The workflow action name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: runName
        description: The workflow run name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Run Actions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/locations/{location}/workflows/{workflowName}/validate
  : post:
      summary: Workflows Validate
      description: Validates the workflow definition.
      operationId: Workflows_Validate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogiclocationslocationworkflowsworkflownamevalidate-post
      parameters:
      - in: path
        name: location
        description: The workflow location
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: body
        name: workflow
        description: The workflow definition
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflows Validate
  /subscriptions/{subscriptionId}/providers/Microsoft.Logic/integrationAccounts:
    get:
      summary: Integration Accounts List By Subscription
      description: Gets a list of integration accounts by subscription.
      operationId: IntegrationAccounts_ListBySubscription
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftlogicintegrationaccounts-get
      parameters:
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts Subscription
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts:
    get:
      summary: Integration Accounts List By Resource Group
      description: Gets a list of integration accounts by resource group.
      operationId: IntegrationAccounts_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicintegrationaccounts-get
      parameters:
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts Resource Group
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}
  : get:
      summary: Integration Accounts Get
      description: Gets an integration account.
      operationId: IntegrationAccounts_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicintegrationaccountsintegrationaccountname-get
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---