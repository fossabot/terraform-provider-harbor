# Data Source: harbor_label

## Example Usage

```hcl
data "harbor_label" "label_1" {
  name   = "main"
  scope  = "g"
}

data "harbor_label" "label_2" {
  id = 4
}

```

## Argument Reference

- `id` - (Optional, int) ID of the label.
- `name` - (Optional, string) Name of the label.
- `scope` - (Optional, string) Scope of the label.

## Attributes Reference

- `id` - (int) Unique ID of the label.
- `name` - (string) Name of the label.
- `description` - (Optional)  The description of the label account will be displayed in harbor.
- `color` - (Optional) The color the label.
- `scope` - (Optional) The scope the label, `p` for project and `g` for global.
- `project_id` - (Optional) The ID of project that the label belongs to.
