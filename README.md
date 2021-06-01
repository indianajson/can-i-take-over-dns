## Summary

Inspired by the increasingly popular <a href='https://github.com/EdOverflow/can-i-take-over-xyz' target="_blank">Can I Take Over XYZ?</a> project by <a href='https://github.com/EdOverflow/' target="_blank">EdOverflow</a> this project is uniquely oriented towards DNS takeovers. While dangling DNS records pose a high threat to companies and warrant high bounties, DNS takeovers pose even greater risks and are sometimes even easier to find.

## What is a DNS takeover?

> DNS takeover vulnerabilities occur when a subdomain (subdomain.example.com) or domain has its authoritative nameserver set to a provider (e.g. AWS Route 53, Akamai, Microsoft Azure, etc.) but the hosted zone has been removed or deleted. Consequently, when making a <a href="https://www.diggui.com/#type=A&hostname=github.technology&nameserver=public&public=8.8.8.8&specify=&clientsubnet=&tcp=def&transport=def&mapped=def&nssearch=def&trace=def&recurse=def&edns=def&dnssec=def&subnet=def&cookie=def&all=def&cmd=def&question=def&answer=def&authority=def&additional=def&comments=def&stats=def&multiline=def&short=def&colorize=on" target="_blank">request for DNS records</a> the server responds with a `SERVFAIL` error. This allows an attacker to create the missing hosted zone on the service that was being used and thus control all DNS records for that (sub)domain. <!--For example, if subdomain.example.com was pointing to a GitHub page and the user decided to delete their GitHub page, an attacker can now create a GitHub page, add a CNAME file containing subdomain.example.com, and claim subdomain.example.com.-->

You can read more at: https://0xpatrik.com/subdomain-takeover-ns/

## Identified Providers
Provider                                        | Status         | Fingerprint                                                             | Discussion                                                    
--------------------------------------------- | -------------- | -----------------------------------------------------------------------  | -------------------------------------------------------------------------------------------------------------------------------------------
AWS Route 53 | **Not Vulnerable** | ns-\*\*\*\*.awsdns-\*\*.org<br>ns-\*\*\*\*.awsdns-\*\*.co.uk<br>ns-\*\*\*.awsdns-\*\*.com<br>ns-\*\*\*.awsdns-\*\*.net | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/1" target="_blank">Issue #1</a>
<a href="https://azure.microsoft.com/" target="_blank">Azure (Microsoft)</a> | **Vulnerable** | ns1-\*\*.azure-dns.com<br>ns2-\*\*.azure-dns.net<br>ns3-\*\*.azure-dns.org<br>ns4-\*\*.azure-dns.info | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/5" target="_blank">Issue #5</a>
<a href="https://bizland.com/" target="_blank">Bizland</a> | **Vulnerable** | ns1.bizland.com<br>ns2.bizland.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/3" target="_blank">Issue #3</a>
<a href="https://dnsmadeeasy.com/" target="_blank">DNSMadeEasy</a> | **Vulnerable** | ns\*\*.dnsmadeeasy.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/6" target="_blank">Issue #6</a>
<a href="https://cloud.google.com/" target="_blank">Google Cloud DNS</a> | **Vulnerable** | ns-cloud-\*\*.googledomains.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/2" target="_blank">Issue #2</a>
<a href="https://mydomain.com/" target="_blank">MyDomain</a> | **Vulnerable <sub><sup>(w/ purchase)</sub></sup>** | ns1.mydomain.com<br>ns2.mydomain.com | <a href="https://github.com/libertalialtd/can-i-take-over-dns/issues/4" target="_blank">Issue #4</a>



