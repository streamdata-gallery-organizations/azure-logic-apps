---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Workflow Versions List
  description: Gets a list of workflow versions.
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