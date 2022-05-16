<h1 align="center">Can I Take Over DNS?<br><sup><sub>A list of DNS providers and whether their zones are vulnerable to DNS takeover!<br><sup> Maintained by</sup> <a target="_blank" href="https://twitter.com/intent/user?screen_name=indianajson"><img src="https://img.shields.io/twitter/follow/indianajson?style=social&label=%40indianajson"/></a>&nbsp;</sub></sup> </h1>

Inspired by the popular [Can I Take Over XYZ?](https://github.com/EdOverflow/can-i-take-over-xyz) project by [@EdOverflow](https://github.com/EdOverflow) this project is uniquely oriented towards [DNS takeovers](#what-is-a-dns-takeover). While dangling DNS records pose a high threat to companies and warrant high bounties, DNS takeovers pose even greater risks and are sometimes even easier to find. We are trying to make this list comprehensive, so please [contribute](#contributions)!

## DNS Providers

These companies provide DNS nameserver services to the general public. In this list you will find out whether domains pointing to these nameservers are vulnerable to DNS takeover and where you can learn more about them. 

Provider                                        | Status         | Fingerprint                                                             | Takeover Instructions                                                    
--------------------------------------------- | -------------- | -----------------------------------------------------------------------  | -------------------------------------------------------------------------------------------------------------------------------------------
[000Domains](https://000domains.com/) | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1.000domains.com<br>ns2.000domains.com<br>fwns1.000domains.com<br>fwns2.000domains.com | [Issue #19](https://github.com/indianajson/can-i-take-over-dns/issues/19)
[AWS Route 53](https://aws.amazon.com/) | **Not Vulnerable** | ns-\*\*\*\*.awsdns-\*\*.org<br>ns-\*\*\*\*.awsdns-\*\*.co.uk<br>ns-\*\*\*.awsdns-\*\*.com<br>ns-\*\*\*.awsdns-\*\*.net | [Issue #1](https://github.com/indianajson/can-i-take-over-dns/issues/1)
[Azure (Microsoft)](https://azure.microsoft.com/) | **Edge Case** | ns1-\*\*.azure-dns.com<br>ns2-\*\*.azure-dns.net<br>ns3-\*\*.azure-dns.org<br>ns4-\*\*.azure-dns.info | [Issue #5](https://github.com/indianajson/can-i-take-over-dns/issues/5)
[Bizland](https://bizland.com/) | **Vulnerable** | ns1.bizland.com<br>ns2.bizland.com<br>clickme.click2site.com<br>clickme2.click2site.com | [Issue #3](https://github.com/indianajson/can-i-take-over-dns/issues/3)
[Cloudflare](https://cloudflare.com/) | **Edge Case** | \*.ns.cloudflare.com | [Issue #10](https://github.com/indianajson/can-i-take-over-dns/issues/10)
[Digital Ocean](https://digitalocean.com/) | **Vulnerable** | ns1.digitalocean.com<br>ns2.digitalocean.com<br>ns3.digitalocean.com | [Issue #22](https://github.com/indianajson/can-i-take-over-dns/issues/22)
[DNSMadeEasy](https://dnsmadeeasy.com/) | **Vulnerable** | ns\*\*.dnsmadeeasy.com | [Issue #6](https://github.com/indianajson/can-i-take-over-dns/issues/6)
[DNSimple](https://dnsimple.com/) | **Vulnerable** | ns1.dnsimple.com<br>ns2.dnsimple.com<br>ns3.dnsimple.com<br>ns4.dnsimple.com | [Issue #16](https://github.com/indianajson/can-i-take-over-dns/issues/16)
[Domain.com](https://domain.com/)| **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1.domain.com<br>ns2.domain.com | [Issue #17](https://github.com/indianajson/can-i-take-over-dns/issues/17)
[DomainPeople](https://domainpeople.com/)| **Not Vulnerable** | ns1.domainpeople.com<br>ns2.domainpeople.com | [Issue #14](https://github.com/indianajson/can-i-take-over-dns/issues/14)
[Dotster](https://dotster.com/)| **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1.dotster.com<br>ns2.dotster.com<br>ns1.nameresolve.com<br>ns2.nameresolve.com | [Issue #18](https://github.com/indianajson/can-i-take-over-dns/issues/18)
[EasyDNS](https://easydns.com/) | **Vulnerable** | dns1.easydns.com<br>dns2.easydns.net<br>dns3.easydns.org<br>dns4.easydns.info| [Issue #9](https://github.com/indianajson/can-i-take-over-dns/issues/9)
[Gandi.net](https://gandi.net/) | **Not Vulnerable** | a.dns.gandi.net<br>b.dns.gandi.net<br>c.dns.gandi.net | 
[Google Cloud](https://cloud.google.com/) | **Vulnerable** | ns-cloud-\*\*.googledomains.com | [Issue #2](https://github.com/indianajson/can-i-take-over-dns/issues/2)
[Hostinger (old NS)](https://hostinger.com/) | **Not Vulnerable** | ns1.hostinger.com<br>ns2.hostinger.com | 
[Hover](https://hover.com/) | **Not Vulnerable** | ns1.hover.com<br>ns2.hover.com | [Issue #21](https://github.com/indianajson/can-i-take-over-dns/issues/21)
[Hurricane Electric](https://dns.he.net/) | **Vulnerable** | ns5.he.net<br>ns4.he.net<br>ns3.he.net<br>ns2.he.net<br>ns1.he.net | [Issue #25](https://github.com/indianajson/can-i-take-over-dns/issues/25)
[Linode](https://linode.com/) | **Vulnerable** | ns1.linode.com<br>ns2.linode.com | [Issue #26](https://github.com/indianajson/can-i-take-over-dns/issues/26)
[MediaTemple (mt)](https://mediatemple.net/) | **Not Vulnerable** | ns1.mediatemple.net<br>ns2.mediatemple.net | [Issue #23](https://github.com/indianajson/can-i-take-over-dns/issues/23)
[MyDomain](https://mydomain.com/) | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1.mydomain.com<br>ns2.mydomain.com | [Issue #4](https://github.com/indianajson/can-i-take-over-dns/issues/4)
[Name.com](https://name.com/) | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1***.name.com<br>ns2***.name.com<br>ns3***.name.com<br>ns4***.name.com | [Issue #8](https://github.com/libertalialtd/can-i-take-over-dns/issues/8)
[namecheap](https://namecheap.com/) | **Not Vulnerable</sup>** | \*.namecheaphosting.com<br>\*.registrar-servers.com | 
[Network Solutions](https://networksolutions.com/) | **Not Vulnerable** | ns\*\*.worldnic.com | [Issue #15](https://github.com/indianajson/can-i-take-over-dns/issues/15)
[NS1](https://nsone.net/) | **Vulnerable** | dns1.p\*\*.nsone.net<br>dns2.p\*\*.nsone.net<br>dns3.p\*\*.nsone.net<br>dns4.p\*\*.nsone.net | [Issue #7](https://github.com/indianajson/can-i-take-over-dns/issues/7)
[TierraNet](https://tierra.net/) | **Vulnerable** | ns1.domaindiscover.com<br>ns2.domaindiscover.com | [Issue #24](https://github.com/indianajson/can-i-take-over-dns/issues/24)
[Reg.ru](https://reg.ru/) | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1.reg.ru<br>ns2.reg.ru | [Issue #28](https://github.com/indianajson/can-i-take-over-dns/issues/28)
[UltraDNS](https://www.home.neustar/dns-services/ultra-dns) | **Not Vulnerable** | pdns***.ultradns.com<br>udns***.ultradns.com<br>sdns***.ultradns.com | [Issue #29](https://github.com/indianajson/can-i-take-over-dns/issues/29)
[Yahoo Small Business](https://yahoosmallbusiness.com/) | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | yns1.yahoo.com<br>yns2.yahoo.com | [Issue #20](https://github.com/indianajson/can-i-take-over-dns/issues/20)


## Private DNS

These are private nameservers operated by various companies. The general public cannot create zones on these nameservers and thus takeovers are not possible. Knowning nameservers that are not vulnerable can be helpful to eliminate false positives from your testing. 

Owner                                        | Status         | Fingerprint                                                             |                                                     
--------------------------------------------- | -------------- | -----------------------------------------------------------------------  |
[Activision](https://activision.com/) | **Not Vulnerable** | ns\*.activision.com | 
[Adobe](https://adobe.com/) | **Not Vulnerable** | adobe-dns-0*.adobe.com | 
[Apple](https://apple.com/) | **Not Vulnerable** | a.ns.apple.com<br>b.ns.apple.com<br>c.ns.apple.com<br>d.ns.apple.com |
[Automattic](https://automattic.com/) | **Not Vulnerable** | ns*.automattic.com |
[Capital One](https://capitalone.com/) | **Not Vulnerable** | ns*.capitalone.com | 
[Disney](https://disney.com/) | **Not Vulnerable** | ns*.twdcns.com<br>ns*.twdcns.info<br>ns*.twdcns.co.uk |
[Google](https://google.com/) | **Not Vulnerable** | ns*.google.com |
[Lowe's](https://lowes.com/) | **Not Vulnerable** | authns*.lowes.com | 
[T-Mobile](https://tmobileus.com/) | **Not Vulnerable** | ns10.tmobileus.com<br>ns10.tmobileus.net | 


## What is a DNS takeover?

> DNS takeover vulnerabilities occur when a subdomain (subdomain.example.com) or domain has its authoritative nameserver set to a provider (e.g. AWS Route 53, Akamai, Microsoft Azure, etc.) but the hosted zone has been removed or deleted. Consequently, when making a [request for DNS records](https://www.diggui.com/#type=A&hostname=github.technology&nameserver=public&public=8.8.8.8&specify=&clientsubnet=&tcp=def&transport=def&mapped=def&nssearch=def&trace=def&recurse=def&edns=def&dnssec=def&subnet=def&cookie=def&all=def&cmd=def&question=def&answer=def&authority=def&additional=def&comments=def&stats=def&multiline=def&short=def&colorize=on) the server responds with a `SERVFAIL` error. This allows an attacker to create the missing hosted zone on the service that was being used and thus control all DNS records for that (sub)domain. <!--For example, if subdomain.example.com was pointing to a GitHub page and the user decided to delete their GitHub page, an attacker can now create a GitHub page, add a CNAME file containing subdomain.example.com, and claim subdomain.example.com.-->

You can read more at: https://0xpatrik.com/subdomain-takeover-ns/

## Contributions

We welcome contributions! 

We need new DNS providers added with information of their vulernability status. You can submit new services [here](https://github.com/indianajson/can-i-take-over-dns/issues/new?assignees=&labels=&template=add--or-update--dns-provider.md&title=%5BService+Name%5D+-+%5BStatus%5D)! We have a list of DNS providers that need to be investigated [here](https://github.com/indianajson/can-i-take-over-dns/issues/13).

We also need to identify as many DNS providers as possible. We have compiled and begun to organize a list of DNS servers. If you want to help read more about it  [here](https://github.com/indianajson/can-i-take-over-dns/issues/12). 
