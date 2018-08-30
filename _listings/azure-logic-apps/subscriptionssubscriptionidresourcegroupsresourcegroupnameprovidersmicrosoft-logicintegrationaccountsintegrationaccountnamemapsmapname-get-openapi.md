---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Maps Get
  description: Gets an integration account map.
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
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-logicworkflows-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflows-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-put
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-patch
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflowname-delete
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownamedisable-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownameenable-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownamegenerateupgradeddefinition-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownamelistswagger-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownameregenerateaccesskey-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownameversions-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownameversionsversionid-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownametriggers-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownametriggerstriggername-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownametriggerstriggernamerun-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownametriggerstriggernamelistcallbackurl-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownameversionsversionidtriggerstriggernamelistcallbackurl-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownametriggerstriggernamehistories-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownametriggerstriggernamehistorieshistoryname-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownametriggerstriggernamehistorieshistorynameresubmit-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownameruns-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownamerunsrunname-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownamerunsrunnamecancel-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownamerunsrunnameactions-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicworkflowsworkflownamerunsrunnameactionsactionname-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logiclocationslocationworkflowsworkflownamevalidate-post
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
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-logicintegrationaccounts-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccounts-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-get
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
    put:
      summary: Integration Accounts Create Or Update
      description: Creates or updates an integration account.
      operationId: IntegrationAccounts_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-put
      parameters:
      - in: body
        name: integrationAccount
        description: The integration account
        schema:
          $ref: '#/definitions/holder'
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
    patch:
      summary: Integration Accounts Update
      description: Updates an integration account.
      operationId: IntegrationAccounts_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-patch
      parameters:
      - in: body
        name: integrationAccount
        description: The integration account
        schema:
          $ref: '#/definitions/holder'
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
    delete:
      summary: Integration Accounts Delete
      description: Deletes an integration account.
      operationId: IntegrationAccounts_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountname-delete
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/listCallbackUrl
  : post:
      summary: Integration Accounts Get Callback Url
      description: Gets the integration account callback URL.
      operationId: IntegrationAccounts_GetCallbackUrl
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamelistcallbackurl-post
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
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
      responses:
        200:
          description: OK
      tags:
      - Integration Accounts Callback Url
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/schemas
  : get:
      summary: Schemas List By Integration Accounts
      description: Gets a list of integration account schemas.
      operationId: Schemas_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameschemas-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Schemas Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/schemas/{schemaName}
  : get:
      summary: Schemas Get
      description: Gets an integration account schema.
      operationId: Schemas_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameschemasschemaname-get
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: schemaName
        description: The integration account schema name
      responses:
        200:
          description: OK
      tags:
      - Schemas
    put:
      summary: Schemas Create Or Update
      description: Creates or updates an integration account schema.
      operationId: Schemas_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameschemasschemaname-put
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: body
        name: schema
        description: The integration account schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: schemaName
        description: The integration account schema name
      responses:
        200:
          description: OK
      tags:
      - Schemas
    delete:
      summary: Schemas Delete
      description: Deletes an integration account schema.
      operationId: Schemas_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameschemasschemaname-delete
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: schemaName
        description: The integration account schema name
      responses:
        200:
          description: OK
      tags:
      - Schemas
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/maps
  : get:
      summary: Maps List By Integration Accounts
      description: Gets a list of integration account maps.
      operationId: Maps_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamemaps-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
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
      - Maps Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/maps/{mapName}
  : get:
      summary: Maps Get
      description: Gets an integration account map.
      operationId: Maps_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamemapsmapname-get
      parameters:
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: path
        name: mapName
        description: The integration account map name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Maps
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