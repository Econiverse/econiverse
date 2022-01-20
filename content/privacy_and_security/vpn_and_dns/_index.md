To start, check [here](https://browserleaks.com/ip) to see what you look like to everyone else on the internet and run a DNS leak test [here](https://www.dnsleaktest.com/) and/or [here](https://dnscheck.tools/#basic) to see who you are trusting with your private data.




## VPN

An IP address is a unique digital location that is used to route data back and forth
between your device and the source of the data. This location is represented in
the form of numbers, such as [65.156.112.48]. Since this is a unique location, it can
be used to identify your physical location and track your activity across the
internet.

A VPN is a service that routes all traffic from your device to the VPN providers
servers, and then they use their IP address to send your data across the internet.
Thus, if anyone was to trace your activity on the internet, it would trace back
to your VPN provider.

In addition, since the information sent between your device
and your VPN provider is encrypted, your internet service provider will no
longer be able to view your activity.

{{< hint danger >}}
If you use a VPN, your privacy is only as good as your VPN provider. The provider
may log your activity and then sell these to 3rd parties or hand them over to
governments. Be very weary of free VPN providers, since they all have to pay bills
somehow.
{{< /hint >}}

**General Recommendations**
1. Use a VPN and pay for it
2. Do not use a VPN based in a country who is part of [Five Eyes](https://en.wikipedia.org/wiki/Five_Eyes)
3. Consider using a provider who runs RAM-Only servers


## DNS

All internet locations are represented by numbers. A Domain Name System (DNS) service maintains a list of which numbers correspond with which alphabetic names for each website. For example, this website is https://econiverse.github.io which when searched with a DNS lookup service, is associated with 185.199.109.153 (a GitHub ip address).

Since a DNS service provider is taking alphabetic website requests and translating it to the numerical representation, they have knowledge of every website that you visit. Some of these providers log and even sell this data for profit. There are a few steps you can take to protect against these practices.

**General Recommendations**
1. Change your DNS service provider to one that you trust. [Quad9 - 9.9.9.9](https://www.quad9.net/) and [Cloudflare - 1.1.1.1](https://1.1.1.1/dns/) are two great places to start. Quad9 is a non-profit organization that [does not collect personal data](https://www.quad9.net/service/privacy) and Cloudflare is one of the fastest DNS providers who [promise to be transparent & to not sell your personal data](https://www.cloudflare.com/privacypolicy/).
2. Enable Secure DNS. This encrypts the request between your device and the DNS provider so that anyone watching cannot see what site you are requesting.
    1. Instructions to enable this for various web browsers can be found [here](https://www.ghacks.net/2021/10/23/how-to-enable-dns-over-https-secure-dns-in-chrome-brave-edge-firefox-and-other-browsers/).
    2. Instructions to enable this on Android devices can be found [here](https://www.unbxtech.com/2021/07/howto-enable-private-dns-android.html)
