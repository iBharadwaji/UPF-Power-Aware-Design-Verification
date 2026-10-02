# Glossary

UPF terms used in these notes, in alphabetical order.

| Term | Meaning | Note |
| --- | --- | --- |
| Atomic power domain | A domain created with `-atomic`; no later command can move part of its extent into another domain | [2.1](../02-power-aware-design/01-power-domains.md) |
| Boundary instance | An instance whose parent is in a different power domain; its ports are where the two domains meet | [2.1](../02-power-aware-design/01-power-domains.md#domain-boundaries) |
| Current scope | The instance that UPF names are resolved against, and where new UPF objects are created; moved with `set_scope` | [2.1](../02-power-aware-design/01-power-domains.md#moving-around-with-set_scope) |
| Design top instance | The instance the UPF applies to; `set_scope /` returns to it | [2.1](../02-power-aware-design/01-power-domains.md#moving-around-with-set_scope) |
| Domain boundary | The ports where one power domain meets another: the upper boundary faces the domain's parent, the lower boundary faces child domains carved out of it | [2.1](../02-power-aware-design/01-power-domains.md#domain-boundaries) |
| Extent | The set of instances that belong to a power domain | [2.1](../02-power-aware-design/01-power-domains.md#upf-example) |
| Power domain | A group of instances that share one primary supply, so they power up, power down and change voltage together | [2.1](../02-power-aware-design/01-power-domains.md) |
