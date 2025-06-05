# Browser Extension Security Audit

This document summarizes the results of a manual review and security risk assessment of extensions installed in Microsoft Edge. The goal is to identify any extensions that may introduce privacy concerns, security risks, or malicious behavior.


## Extensions Analyzed

| Extension                    | Permissions Summary                    | Site Access        | Risk Level   |
|------------------------------|----------------------------------------|--------------------|--------------|
| Google Docs Offline          | Basic functionality only               | Google Docs/Drive  | Low          |
| Microsoft Rewards            | Read history, modify settings          | All sites          | Medium-High  |
| Automate Your Bing Searches  | Block content, script injection        | *.bing.com only    | Medium       |
| Hoxx VPN Proxy               | View and change data on all sites      | All sites          | High         |

## Key Findings

- High Risk: Hoxx VPN Proxy has extensive permissions, including access to all browsing data and websites. This poses significant privacy and security concerns.
- Medium Risk:
  - Microsoft Rewards tracks browsing history and can modify browser behavior.
  - Automate Your Bing Searches may be used for automation that could violate platform policies.
- Low Risk: Google Docs Offline has limited access and poses minimal security concerns.

## Recommendations

- Remove or disable high-risk extensions, especially those with full access to all sites.
- Regularly review extension permissions and limit access to specific sites where possible.
- Avoid keeping Developer Mode enabled unless actively developing or testing.
- Be cautious when using InPrivate Browsing, as many extensions remain active unless explicitly disabled.

## Conclusion

Browser extensions can pose serious risks if not properly vetted. Conduct regular reviews to ensure only trusted and essential extensions are installed, and that they have the minimum necessary permissions.


