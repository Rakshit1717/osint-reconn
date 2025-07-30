# General Reconnaissance
This folder contains tools and techniques for whois, DNS lookups, email enumeration, etc.
## Tools Used
- whois
- dig/nslookup
- hunter.io
- haveibeenpwned.com
- whatweb
- shodan.io
- theHarvester
- Recon-ng
- Sublist3r
- Amass
- crt.sh
- eyewitness 
  ### Usage
```bash
#### Summary Table
| Tool/Command                     | Recon Type | Notes                                         |
| -------------------------------- | ---------- | --------------------------------------------- |
| whois example.com                | Passive    | Public domain info                            |
| dig example.com ANY              | Passive    | DNS records query                             |
| nslookup -type=MX example.com    | Passive    | DNS mail servers                              |
| curl hunter.io API call          | Passive    | Third-party data retrieval                    |
| haveibeenpwned.com query         | Passive    | Third-party breach database                   |
| theharvester -b all (default)    | Passive    | Public sources, may have active options       |
| recon-ng (public source modules) | Passive    | Depends on module, mostly passive             |
| shodan search apache             | Passive    | Uses Shodan’s database                        |
| shodan host 8.8.8.8              | Active     | Retrieves live data on IP (scanned by Shodan) |
| sublist3r                        | Passive    | Passive DNS enumeration                       |
| amass enum (passive mode)        | Passive    | Passive enumeration                           |
| amass enum (with active flags)   | Active     | Active scanning options                       |
| crt.sh query                     | Passive    | Certificate transparency logs                 |
| eyewitness --web                 | Active     | Connects to URLs and screenshots              |

