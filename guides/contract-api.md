# Contract API

## Link record

| Field | Type | Meaning |
|---|---|---|
| `owner` | `Address` | Address authorized to mutate the alias |
| `destination` | `String` | Current redirect destination |
| `active` | `bool` | Whether resolution returns the record |
| `created_at` | `u64` | Creation ledger timestamp |
| `updated_at` | `u64` | Most recent mutation timestamp |

## Methods

- `create(owner, alias, destination)` claims an unused alias.
- `resolve(alias)` returns an active record without authorization.
- `update(owner, alias, destination)` changes the route and reactivates it.
- `deactivate(owner, alias)` disables public resolution.

Aliases are 3–32 characters. Destinations are limited to 2,048 characters. Clients should additionally enforce allowed URL schemes.

