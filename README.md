# free-proxies

Free proxies are publicly available, often unreliable, slow, short-lived, and potentially insecure (some may log traffic or be malicious). They're mostly datacenter IPs, which get blocked easily by WAFs (e.g., Cloudflare) during mass scanning/recon. Great for testing scripts on small scales, but not recommended for serious bug bounty recon on large lists (like 35k domains) — expect frequent blocks and low success rates.Top sources (updated frequently as of December 2025):Proxifly (GitHub): Updated every 5 minutes, supports HTTP/SOCKS4/SOCKS5. ~5,500 working proxies.
Download: curl -sL https://cdn.jsdelivr.net/gh/proxifly/free-proxy-list@main/proxies/all/data.txt
ProxyScrape: Updates every minute, thousands of proxies.
https://proxyscrape.com/free-proxy-list
Geonode Free Proxy List: Regularly scraped public proxies.
https://geonode.com/free-proxy-list
ProxyNova: Checks over a million proxies daily.
https://www.proxynova.com/proxy-server-list/
Free-Proxy-List.net: Updated every 10 minutes.
https://free-proxy-list.net/
Spys.one: Advanced filtering by country/ASN.
https://spys.one/en/
Other GitHub repos: TheSpeedX/PROXY-List (daily updates), gfpcom/free-proxy-list (massive lists).

Tip: Always verify proxies (e.g., with proxy-checker tools) and rotate them. For your Retire.js/Nuclei scripts, load into a proxies.txt file (one per line: http://ip:port).

