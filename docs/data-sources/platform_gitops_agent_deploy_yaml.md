---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "harness_platform_gitops_agent_deploy_yaml Data Source - terraform-provider-harness"
subcategory: "Next Gen"
description: |-
  Datasource for fetching a Harness Gitops Agent deployment manifest YAML.
---

# harness_platform_gitops_agent_deploy_yaml (Data Source)

Datasource for fetching a Harness Gitops Agent deployment manifest YAML.

## Example Usage

```terraform
data "harness_platform_gitops_agent_deploy_yaml" "example" {
  identifier = "identifier"
  account_id = "account_id"
  project_id = "project_id"
  org_id     = "org_id"
  namespace  = "namespace"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `account_id` (String) Account identifier of the GitOps agent.
- `identifier` (String) Identifier of the GitOps agent.
- `namespace` (String) The kubernetes namespace where the agent is installed.

### Optional

- `org_id` (String) Organization identifier of the GitOps agent.
- `project_id` (String) Project identifier of the GitOps agent.

### Read-Only

- `id` (String) The ID of this resource.
- `yaml` (String) The deployment manifest YAML of the GitOps agent.
