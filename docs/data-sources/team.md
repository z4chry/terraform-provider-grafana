---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "grafana_team Data Source - terraform-provider-grafana"
subcategory: ""
description: |-
  Official documentation https://grafana.com/docs/grafana/latest/administration/manage-users-and-permissions/manage-teams/HTTP API https://grafana.com/docs/grafana/latest/http_api/team/
---

# grafana_team (Data Source)

* [Official documentation](https://grafana.com/docs/grafana/latest/administration/manage-users-and-permissions/manage-teams/)
* [HTTP API](https://grafana.com/docs/grafana/latest/http_api/team/)

## Example Usage

```terraform
resource "grafana_team" "test" {
  name  = "test-team"
  email = "test-team-email@test.com"
}

data "grafana_team" "from_name" {
  name = grafana_team.test.name
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) The name of the Grafana team.

### Read-Only

- `id` (String) The ID of this resource.

