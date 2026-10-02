# UPF command cheat sheet

UPF commands used in these notes, each linked to the note that covers it.

| Command | Purpose | Minimal form | Note |
| --- | --- | --- | --- |
| `upf_version` | Declare which UPF version the file is written in | `upf_version 2.1` | [2.1](../02-power-aware-design/01-power-domains.md#upf-example) |
| `set_scope` | Move the current scope; later names resolve relative to it | `set_scope u_cpu` | [2.1](../02-power-aware-design/01-power-domains.md#moving-around-with-set_scope) |
| `create_power_domain` | Group instances that share a primary supply | `create_power_domain PD_CPU -elements {u_cpu}` | [2.1](../02-power-aware-design/01-power-domains.md#building-domains-with-create_power_domain) |
