---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = WorkflowVersionRequestBuilder.WorkflowVersionRequestBuilderGetQueryParameters(
		select = ["category","displayName","versionNumber","executionConditions"],
		expand = ["tasks"],
)

request_configuration = WorkflowVersionRequestBuilder.WorkflowVersionRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.identity_governance.lifecycle_workflows.workflows.by_workflow_id('workflow-id').versions.by_version_id('workflowVersion-versionNumber').get(request_configuration = request_configuration)


```