# Security model

## Protected assets

- Alias ownership
- Destination integrity
- Transaction authorization
- Redirect availability
- User safety when following a Blink link

## Primary threats

| Threat | Existing control | Required follow-up |
|---|---|---|
| Unauthorized mutation | Soroban `require_auth` | Independent contract audit |
| Malicious destination | Frontend URL validation | Contract enforcement and blocklists |
| RPC outage | Explicit failures | Provider fallback and caching |
| Phishing links | None in MVP | Reporting and interstitial policies |
| Storage archival | TTL extension | Restoration and renewal automation |
| Redirect abuse | Basic alias validation | Rate limits and operational monitoring |

The MVP is not audited and should not be treated as production infrastructure.

