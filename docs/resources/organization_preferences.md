---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "grafana_organization_preferences Resource - terraform-provider-grafana"
subcategory: "Grafana OSS"
description: |-
  Official documentation https://grafana.com/docs/grafana/latest/administration/manage-organizations/HTTP API https://grafana.com/docs/grafana/latest/developers/http_api/preferences/#get-current-org-prefs
---

# grafana_organization_preferences (Resource)

* [Official documentation](https://grafana.com/docs/grafana/latest/administration/manage-organizations/)
* [HTTP API](https://grafana.com/docs/grafana/latest/developers/http_api/preferences/#get-current-org-prefs)

## Example Usage

```terraform
resource "grafana_organization_preferences" "test" {
  theme      = "light"
  timezone   = "utc"
  week_start = "Tuesday"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `home_dashboard_id` (Number) The Organization home dashboard ID.
- `home_dashboard_uid` (String) The Organization home dashboard UID.
- `theme` (String) The Organization theme. Available values are `light`, `dark`, or an empty string for the default.
- `timezone` (String) The Organization timezone. Available values are `utc`, `browser`, or an empty string for the default.
- `week_start` (String) The Organization week start.

### Read-Only

- `id` (String) The ID of this resource.

