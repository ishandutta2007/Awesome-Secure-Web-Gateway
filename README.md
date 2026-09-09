# Awesome-Secure-Web-Gateway

## Top Secure Web Gateway (SWG) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Cloud Web Filtering, HTTPS Inspection, URL Filtering, Malware Protection, Acceptable Use Policy & SSE/SASE Web Security*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Secure Web Gateway (SWG)**. These solutions inspect outbound web traffic, enforce acceptable-use policies, decrypt and scan HTTPS, block malicious destinations, and protect users whether they are on-network or remote.



**Examples** include Zscaler Internet Access, Netskope SWG, Cisco Umbrella, Forcepoint ONE, Cloudflare Gateway, iboss, Skyhigh Security, Lookout Secure Web Gateway, Versa Secure Internet Access, and Cato Networks (the category leaders).



**Open-source emphasis**: Full cloud-native SWG / SSE platforms with global Points of Presence, SSL inspection at scale, and managed threat intelligence are commercial. Open-source options center on classic proxy + content-filtering stacks (**Squid** + **e2guardian**, Web Safety, etc.) that organizations can self-host for on-premises or private-cloud web security. This section lists every major relevant project found.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Zscaler Internet Access (ZIA)](https://www.zscaler.com/products/zscaler-internet-access)**  

  Leading cloud-native Secure Web Gateway and cornerstone of Zscaler’s SSE platform, delivering scalable SSL inspection, threat protection, and policy enforcement from a global security cloud.



- **[Netskope SWG](https://www.netskope.com/)**  

  Cloud SWG tightly integrated with Netskope’s SSE/SASE platform, strong in data protection, CASB context, and advanced threat defense.



- **[Cisco Umbrella](https://umbrella.cisco.com/)**  

  DNS-layer security and cloud SWG (part of Cisco Secure Access / SSE) that provides first-line protection and full proxy capabilities, especially popular in Cisco environments.



- **[Cloudflare Gateway](https://www.cloudflare.com/products/zero-trust/gateway/)**  

  Secure web gateway delivered on Cloudflare’s global edge network, offering DNS filtering, HTTP/S inspection, and Zero Trust policy enforcement with strong performance.



- **[Forcepoint ONE](https://www.forcepoint.com/)**  

  Cloud security platform that includes SWG capabilities alongside DLP and other data-centric controls.



- **[iboss, Skyhigh Security, Lookout](https://www.iboss.com/)**  

  Cloud SWG and SSE offerings focused on web security, remote user protection, and threat prevention.



- **[Versa Secure Internet Access, Cato Networks](https://www.catonetworks.com/)**  

  SASE platforms that include Secure Web Gateway functionality as part of a converged networking and security service.



- **[Other SWG / SSE platforms](https://www.zscaler.com/)**  

  Additional cloud-delivered web security and Security Service Edge solutions from major security vendors.



## Open-Source GitHub Projects



- **[Squid](http://www.squid-cache.org/)**  

  The classic open-source caching and forwarding proxy. Forms the foundation of most self-hosted secure web gateway deployments and supports SSL bumping for HTTPS inspection.



- **[e2guardian](https://github.com/e2guardian/e2guardian)**  

  Leading open-source web content filter that works with Squid (or standalone/ICAP). Provides URL filtering, content phrase matching, HTTPS MITM inspection, virus scanning integration, and group-based policies.



- **[Web Safety for Squid](https://github.com/diladele/websafety)**  

  Secure web gateway and admin UI built around Squid. Adds category-based filtering, HTTPS inspection, antivirus scanning, ad blocking, and easier management for schools and enterprises.



- **[Squid + SSL-Bump / ICAP stacks](https://github.com/search?q=squid+ssl+bump+OR+e2guardian)**  

  Community Docker images, configurations, and integration projects that combine Squid SSL interception with e2guardian or other ICAP content filters.



- **[Other proxy & filtering tools](https://github.com/search?q=web+content+filter+OR+secure+web+gateway+OR+proxy+filter)**  

  Additional open-source proxies, DNS filters, and content-filtering projects used for self-hosted web security.



- **[DNS filtering & blocklist tools](https://github.com/search?q=DNS+filter+OR+Pi-hole+OR+blocklist)**  

  Tools such as Pi-hole and related blocklist managers that provide lightweight DNS-layer protection (complementary to full SWG).



- **[ICAP servers & antivirus modules](https://github.com/search?q=ICAP+OR+ClamAV+proxy)**  

  Open-source ICAP implementations and ClamAV integrations commonly paired with Squid/e2guardian for malware scanning of downloads.



- **[Policy & logging helpers](https://github.com/search?q=squid+log+OR+proxy+policy)**  

  Scripts and dashboards for analyzing proxy logs, reporting, and refining filtering policies.



### Additional Strong Open-Source Options



- **TLS interception tooling**: Documentation and helper scripts for generating and distributing organizational root CAs required for HTTPS inspection.

- **Category & reputation lists**: Community-maintained URL and domain blocklists that can be loaded into e2guardian or Squid.

- **Container deployments**: Ready-to-run Docker/Kubernetes stacks for Squid + e2guardian.

- **Authentication integrations**: LDAP, Kerberos, and captive-portal solutions that work with open-source proxies.

- **Monitoring**: Prometheus exporters and log pipelines for proxy health and usage metrics.

- Emerging eBPF or transparent-proxy experiments for modern Linux environments.



**Frameworks for building custom systems**:  

For a self-hosted Secure Web Gateway, the standard open-source stack is **Squid** (proxy + SSL bump) + **e2guardian** or **Web Safety** (content filtering, categories, AV).  

This combination can enforce acceptable-use policies, block malicious content, and inspect HTTPS when clients trust the organizational CA.  

Cloud-native SWG / SSE platforms (Zscaler, Netskope, Cisco Umbrella, Cloudflare Gateway, Cato, etc.) provide global scale, continuous threat intelligence, zero-maintenance PoPs, CASB/DLP integration, and support that self-hosted proxies cannot match.  

Many organizations run open-source proxies for specific sites or lab environments while adopting a commercial cloud SWG for the distributed workforce.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Secure Web Gateways perform TLS interception and traffic inspection. Deployment requires careful legal, privacy, and change-management consideration (user consent, certificate distribution, performance impact, and compliance).

- Open-source proxy and filtering stacks demand ongoing maintenance, security hardening, capacity planning, and threat-intelligence updates. They do not automatically provide the same real-time protection or global footprint as commercial cloud SWGs. Operators remain responsible for the security and reliability of any solution they run.



---



**Made for network security engineers, SASE/SSE architects, IT administrators, and privacy-conscious organizations.**  

Let's keep web security effective and transparent—whether delivered from the cloud or built on proven open-source proxy technology.
