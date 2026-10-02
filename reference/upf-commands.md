# UPF command cheat sheet

UPF commands used in these notes, each linked to the note that covers it.

| Command | Purpose | Minimal form | Note |
| --- | --- | --- | --- |
| `upf_version` | Declare which UPF version the file is written in | `upf_version 2.1` | [2.1](../02-power-aware-design/01-power-domains.md#upf-example) |
| `set_scope` | Move the current scope; later names resolve relative to it | `set_scope u_cpu` | [2.1](../02-power-aware-design/01-power-domains.md#moving-around-with-set_scope) |
| `create_power_domain` | Group instances that share a primary supply | `create_power_domain PD_CPU -elements {u_cpu}` | [2.1](../02-power-aware-design/01-power-domains.md#building-domains-with-create_power_domain) |
| `create_supply_port` | Create a supply connection point on an instance | `create_supply_port VDD_AON` | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#supply-ports) |
| `create_supply_net` | Create a wire that carries a supply | `create_supply_net VDD_AON` | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#supply-nets) |
| `connect_supply_net` | Tie a supply net to ports | `connect_supply_net VDD_AON -ports VDD_AON` | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#supply-nets) |
| `set_domain_supply_net` | Legacy: bind a domain's primary power and ground nets | `set_domain_supply_net PD_AON -primary_power_net VDD_AON -primary_ground_net VSS` | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#upf-example) |
