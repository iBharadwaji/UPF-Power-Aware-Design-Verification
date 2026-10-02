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
| HighConn, LowConn | The outside (HighConn) and inside (LowConn) of a port | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#supply-ports) |
| Power domain | A group of instances that share one primary supply, so they power up, power down and change voltage together | [2.1](../02-power-aware-design/01-power-domains.md) |
| Resolved supply net | A supply net allowed to have several drivers, combined by its `-resolve` method | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#supply-nets) |
| Supply net | A wire that carries a supply's state and voltage between supply ports and to the logic | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#supply-nets) |
| Supply port | A connection point for a supply on an instance; its direction sets which way the supply state flows | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#supply-ports) |
| Supply state | What a supply carries besides its voltage: `FULL_ON`, `PARTIAL_ON`, `OFF` or `UNDETERMINED` | [2.2](../02-power-aware-design/02-supply-nets-and-ports.md#what-a-supply-carries) |
