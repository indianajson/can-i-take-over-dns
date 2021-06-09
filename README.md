<h1 align="center">Can I Take Over DNS?<br><sup><sub>A list of DNS providers and whether their zones are vulnerable to DNS takeover!</sub></sup></h1>

Inspired by the popular [Can I Take Over XYZ?](https://github.com/EdOverflow/can-i-take-over-xyz) project by [@EdOverflow](https://github.com/EdOverflow) this project is uniquely oriented towards [DNS takeovers](#what-is-a-dns-takeover). While dangling DNS records pose a high threat to companies and warrant high bounties, DNS takeovers pose even greater risks and are sometimes even easier to find. We are trying to make this list comprehensive, so please [contribute](#contributions)!

## DNS Providers

These companies provide DNS nameserver services to the general public. In this list you will find out whether domains pointing to these nameservers are vulnerable to DNS takeover and where you can learn more about them. 

Provider                                        | Status         | Fingerprint                                                             | Takeover Instructions                                                    
--------------------------------------------- | -------------- | -----------------------------------------------------------------------  | -------------------------------------------------------------------------------------------------------------------------------------------
<a href="https://aws.amazon.com/" target="_blank">AWS Route 53</a> | **Not Vulnerable** | ns-\*\*\*\*.awsdns-\*\*.org<br>ns-\*\*\*\*.awsdns-\*\*.co.uk<br>ns-\*\*\*.awsdns-\*\*.com<br>ns-\*\*\*.awsdns-\*\*.net | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/1" target="_blank">Issue #1</a>
<a href="https://azure.microsoft.com/" target="_blank">Azure (Microsoft)</a> | **Vulnerable** | ns1-\*\*.azure-dns.com<br>ns2-\*\*.azure-dns.net<br>ns3-\*\*.azure-dns.org<br>ns4-\*\*.azure-dns.info | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/5" target="_blank">Issue #5</a>
<a href="https://bizland.com/" target="_blank">Bizland</a> | **Vulnerable** | ns1.bizland.com<br>ns2.bizland.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/3" target="_blank">Issue #3</a>
<a href="https://cloudflare.com/" target="_blank">Cloudflare</a> | **Vulnerable** | \*.ns.cloudflare.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/10" target="_blank">Issue #10</a>
<a href="https://dnsmadeeasy.com/" target="_blank">DNSMadeEasy</a> | **Vulnerable** | ns\*\*.dnsmadeeasy.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/6" target="_blank">Issue #6</a>
<a href="https://domainpeople.com/" target="_blank">DomainPeople</a> | **Not Vulnerable** | ns1.domainpeople.com<br>ns2.domainpeople.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/14" target="_blank">Issue #14</a>
<a href="https://easydns.com/" target="_blank">EasyDNS</a> | **Vulnerable** | dns1.easydns.com<br>dns2.easydns.net<br>dns3.easydns.org<br>dns4.easydns.info| <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/9" target="_blank">Issue #9</a>
<a href="https://cloud.google.com/" target="_blank">Google Cloud DNS</a> | **Vulnerable** | ns-cloud-\*\*.googledomains.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/2" target="_blank">Issue #2</a>
<a href="https://mydomain.com/" target="_blank">MyDomain</a> | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1.mydomain.com<br>ns2.mydomain.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/4" target="_blank">Issue #4</a>
<a href="https://name.com/" target="_blank">Name.com</a> | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1***.name.com<br>ns2***.name.com<br>ns3***.name.com<br>ns4***.name.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/8" target="_blank">Issue #8</a>
<a href="https://networksolutions.com/" target="_blank">Network Solutions</a> | **Not Vulnerable** | ns\*\*.worldnic.com | 
<a href="https://nsone.net/" target="_blank">NS1</a> | **Vulnerable** | dns1.p\*\*.nsone.net<br>dns2.p\*\*.nsone.net<br>dns3.p\*\*.nsone.net<br>dns4.p\*\*.nsone.net | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/7" target="_blank">Issue #7</a>


## Private DNS

These are private nameservers operated by various companies. The general public cannot create zones on these nameservers and thus takeovers are not possible. Knowning nameservers that are not vulnerable can be helpful to eliminate false positives from your testing. 

Owner                                        | Status         | Fingerprint                                                             |                                                     
--------------------------------------------- | -------------- | -----------------------------------------------------------------------  |
<a href="https://activision.com/">Activision</a> | **Not Vulnerable** | ns\*.activision.com | 
<a href="https://apple.com/">Apple</a> | **Not Vulnerable** | a.ns.apple.com<br>b.ns.apple.com<br>c.ns.apple.com<br>d.ns.apple.com |
<a href="https://capitalone.com/">Capital One</a> | **Not Vulnerable** | ns1.capitalone.com<br>ns2.capitalone.com<br>ns3.capitalone.com | 
<a href="https://CSU.ST/">CSU.ST</a> | **Not Vulnerable** | 0xd0a1.csust.net<br>0xd0a2.csust.net<br>0xd0a3.csust.net<br>0xd0a4.csust.net | 
<a href="https://disney.com/">The Walt Disney Company</a> | **Not Vulnerable** | ns1.twdcns.com<br>ns2.twdcns.com<br>ns3.twdcns.info<br>ns4.twdcns.info<br>ns5.twdcns.co.uk<br>ns6.twdcns.co.u |
<a href="https://lowes.com/">Lowe's</a> | **Not Vulnerable** | authns1.lowes.com<br>authns2.lowes.com | 
<a href="https://tmobileus.com/">T-Mobile</a> | **Not Vulnerable** | ns10.tmobileus.com<br>ns10.tmobileus.net | 

## What is a DNS takeover?

> DNS takeover vulnerabilities occur when a subdomain (subdomain.example.com) or domain has its authoritative nameserver set to a provider (e.g. AWS Route 53, Akamai, Microsoft Azure, etc.) but the hosted zone has been removed or deleted. Consequently, when making a [request for DNS records](https://www.diggui.com/#type=A&hostname=github.technology&nameserver=public&public=8.8.8.8&specify=&clientsubnet=&tcp=def&transport=def&mapped=def&nssearch=def&trace=def&recurse=def&edns=def&dnssec=def&subnet=def&cookie=def&all=def&cmd=def&question=def&answer=def&authority=def&additional=def&comments=def&stats=def&multiline=def&short=def&colorize=on) the server responds with a `SERVFAIL` error. This allows an attacker to create the missing hosted zone on the service that was being used and thus control all DNS records for that (sub)domain. <!--For example, if subdomain.example.com was pointing to a GitHub page and the user decided to delete their GitHub page, an attacker can now create a GitHub page, add a CNAME file containing subdomain.example.com, and claim subdomain.example.com.-->

You can read more at: https://0xpatrik.com/subdomain-takeover-ns/

## Contributions

We welcome contributions! 

We need new DNS providers added with information of their vulernability status. You can submit new services [here](https://github.com/indianajson/can-i-take-over-dns/issues/new?assignees=&labels=&template=add--or-update--dns-provider.md&title=%5BService+Name%5D+-+%5BStatus%5D)! We have a list of DNS providers that need to be investigated [here](https://github.com/indianajson/can-i-take-over-dns/issues/13).

We also need to identify as many DNS providers as possible. We have compiled and begun to organize a list of DNS servers. If you want to help read more about it  [here](https://github.com/indianajson/can-i-take-over-dns/issues/12). 
