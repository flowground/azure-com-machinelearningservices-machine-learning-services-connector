# ![LOGO](logo.png) Azure Machine Learning Workspaces **flow**ground Connector

## Description

A generated **flow**ground connector for the Azure Machine Learning Workspaces API (version 2018-11-19).

Generated from: https://api.apis.guru/v2/specs/azure.com/machinelearningservices-machineLearningServices/2018-11-19/swagger.json<br/>
Generated at: 2019-05-07T17:38:20+03:00

## API Description

These APIs allow end users to operate on Azure Machine Learning Workspace resources.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all of the available Azure Machine Learning Workspaces REST API operations.

*Tags:* `Operation`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.

### Gets the current usage information as well as limits for AML resources for given subscription and location.

*Tags:* `Usage`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `location` - _required_ - The location for which resource usage is queried.

### Returns supported VM Sizes in a location

*Tags:* `VirtualMachineSizes`

#### Input Parameters
* `location` - _required_ - The location upon which virtual-machine-sizes is queried.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.

### Lists all the available machine learning workspaces under the specified subscription.

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `$skiptoken` - _optional_ - Continuation token for pagination.

### Lists all the available machine learning workspaces under the specified resource group.

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `$skiptoken` - _optional_ - Continuation token for pagination.

### Deletes a machine learning workspace.

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.

### Gets the properties of the specified machine learning workspace.

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.

### Updates a machine learning workspace with the specified parameters.

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.

### Creates or updates a workspace with the specified parameters.

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.

### Gets computes in specified workspace.

*Tags:* `OperationalizationClusters` `MachineLearningComputes`

#### Input Parameters
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `$skiptoken` - _optional_ - Continuation token for pagination.

### Deletes specified Machine Learning compute.

*Tags:* `OperationalizationClusters` `MachineLearningComputes`

#### Input Parameters
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.
* `computeName` - _required_ - Name of the Azure Machine Learning compute.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `underlyingResourceAction` - _required_ - Delete the underlying compute if 'Delete', or detach the underlying compute from workspace if 'Detach'.
    Possible values: Delete, Detach.

### Gets compute definition by its name. Any secrets (storage keys, service credentials, etc) are not returned - use 'keys' nested resource to get them.

*Tags:* `OperationalizationClusters` `MachineLearningComputes`

#### Input Parameters
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.
* `computeName` - _required_ - Name of the Azure Machine Learning compute.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.

### Updates properties of a compute. This call will overwrite a compute if it exists. This is a nonrecoverable operation.

*Tags:* `OperationalizationClusters` `MachineLearningComputes`

#### Input Parameters
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.
* `computeName` - _required_ - Name of the Azure Machine Learning compute.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.

### Creates or updates compute. This call will overwrite a compute if it exists. This is a nonrecoverable operation. If your intent is to create a new compute, do a GET first to verify that it does not exist yet.

*Tags:* `OperationalizationClusters` `MachineLearningComputes`

#### Input Parameters
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.
* `computeName` - _required_ - Name of the Azure Machine Learning compute.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.

### Gets secrets related to Machine Learning compute (storage keys, service credentials, etc).

*Tags:* `OperationalizationClusters` `MachineLearningComputes`

#### Input Parameters
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.
* `computeName` - _required_ - Name of the Azure Machine Learning compute.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.

### Get the details (e.g IP address, port etc) of all the compute nodes in the compute.

*Tags:* `MachineLearningComputes`

#### Input Parameters
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.
* `computeName` - _required_ - Name of the Azure Machine Learning compute.
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.

### Lists all the keys associated with this workspace. This includes keys for the storage account, app insights and password for container registry

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.

### Resync all the keys associated with this workspace. This includes keys for the storage account, app insights and password for container registry

*Tags:* `Workspaces`

#### Input Parameters
* `api-version` - _required_ - Version of Azure Machine Learning resource provider API.
* `subscriptionId` - _required_ - Azure subscription identifier.
* `resourceGroupName` - _required_ - Name of the resource group in which workspace is located.
* `workspaceName` - _required_ - Name of Azure Machine Learning workspace.

## License

**flow**ground :- Telekom iPaaS / azure-com-machinelearningservices-machine-learning-services-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
