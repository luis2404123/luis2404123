<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:141414,50:311214,100:f91127&height=220&text=BirdProxies&fontColor=ffffff&fontSize=72&fontAlignY=38&desc=Proxy%20Infrastructure%20for%20Developers&descSize=20&descAlignY=58&descColor=a5a3a3&animation=fadeIn" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?lines=Residential+%7C+ISP+%7C+Mobile+Proxies;Global+Coverage+%E2%80%93+DE+US+UK+JP+HK+FR;99.9%25+Uptime+SLA;Built+for+Scraping+%26+Automation&font=JetBrains+Mono&center=true&width=520&height=45&duration=3000&pause=1000&color=f91127&size=18" alt="BirdProxies"/>

<br/>

[![Website](https://img.shields.io/badge/birdproxies.com-141414?style=for-the-badge&logo=googlechrome&logoColor=f91127)](https://birdproxies.com)&nbsp;
[![Dashboard](https://img.shields.io/badge/Dashboard-141414?style=for-the-badge&logo=windowsterminal&logoColor=f91127)](https://dash.birdproxies.com)&nbsp;
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/birdproxies)

</div>

<br/>

## About

BirdProxies provides high-performance proxy infrastructure built for scraping, automation, and data collection at scale. Direct ISP partnerships, clean IP pools, and sub-second response times across multiple regions.

<br/>

<table>
<tr>
<td width="50%" valign="top">

### Residential Proxies
- Rotating residential IPs from a global pool
- City and country-level targeting
- Rotating and sticky sessions
- HTTP, HTTPS & SOCKS5

</td>
<td width="50%" valign="top">

### ISP Proxies
- Static IPs from real ISPs
- Available in DE, US, UK, JP, HK, FR
- Dedicated per-user allocation
- Ideal for accounts and long sessions

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Mobile Proxies
- Real 4G/5G carrier IPs
- Lowest detection rate available
- Automatic IP rotation
- Carrier-level targeting

</td>
<td width="50%" valign="top">

### Chrome Extension
- One-click proxy switching
- Per-tab proxy assignment
- Sync proxies from dashboard
- Auto-rotate on interval

</td>
</tr>
</table>

<br/>

## Quick Start

```bash
curl -x http://USER:PASS@gate.birdproxies.com:7777 https://httpbin.org/ip
```

<details>
<summary><b>Python</b></summary>

```python
import requests

proxies = {
    "http":  "http://USER:PASS@gate.birdproxies.com:7777",
    "https": "http://USER:PASS@gate.birdproxies.com:7777",
}

response = requests.get("https://httpbin.org/ip", proxies=proxies)
print(response.json())
```

</details>

<details>
<summary><b>Node.js</b></summary>

```javascript
import { HttpsProxyAgent } from 'https-proxy-agent';

const agent = new HttpsProxyAgent('http://USER:PASS@gate.birdproxies.com:7777');
const res = await fetch('https://httpbin.org/ip', { agent });
console.log(await res.json());
```

</details>

<details>
<summary><b>Go</b></summary>

```go
proxyURL, _ := url.Parse("http://USER:PASS@gate.birdproxies.com:7777")
client := &http.Client{
    Transport: &http.Transport{Proxy: http.ProxyURL(proxyURL)},
}
resp, _ := client.Get("https://httpbin.org/ip")
```

</details>

<br/>

## Open Source Tools

| Repository | Description |
|:---|:---|
| [`stealth-requests`](https://github.com/luis2404123/stealth-requests) | Stealth HTTP client with fingerprint rotation and anti-detection |
| [`stealth-fetch`](https://github.com/luis2404123/stealth-fetch) | Drop-in `fetch()` replacement with automatic stealth headers |
| [`proxy-mcp`](https://github.com/luis2404123/proxy-mcp) | MCP server — give AI agents proxy-powered web scraping |
| [`scraping-recipes`](https://github.com/luis2404123/scraping-recipes) | Tested code recipes for bypassing Cloudflare, Akamai & more |
| [`proxy-checker`](https://github.com/luis2404123/proxy-checker) | Bulk proxy validation with protocol detection and geo lookup |
| [`proxy-benchmarks`](https://github.com/luis2404123/proxy-benchmarks) | Benchmark proxy latency, throughput, and reliability |
| [`puppeteer-proxy-plugin`](https://github.com/luis2404123/puppeteer-proxy-plugin) | Per-page proxy rotation for Puppeteer and Playwright |

<br/>

<div align="center">

**[Get Started](https://birdproxies.com)** &nbsp;&middot;&nbsp; **[Documentation](https://docs.birdproxies.com)** &nbsp;&middot;&nbsp; **[Discord](https://discord.gg/birdproxies)**

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:f91127,50:311214,100:141414&height=100&section=footer&reversal=true" width="100%"/>

</div>
