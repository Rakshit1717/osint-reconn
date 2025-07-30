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
#whois example.com
dig example.com ANY
nslookup -type=MX example.com
curl "https://api.hunter.io/v2/domain-search?domain=example.com&api_key=YOUR_API_KEY"
https://haveibeenpwned.com/unifiedsearch/example@example.com
theharvester -d example.com -b all
recon-ng
> workspaces create example
> modules load recon/domains-hosts/bing_domain_web
> set SOURCE example.com
> run
shodan host 8.8.8.8
shodan search apache
sublist3r -d example.com -o subdomains.txt
amass enum -d example.com -o amass_subdomains.txt
https://crt.sh/?q=%25.example.com
eyewitness --web -f urls.txt -d ./reports/
