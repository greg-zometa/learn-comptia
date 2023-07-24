# Domain Name System

The [Domain Name System (DNS)](https://www.cloudflare.com/learning/dns/what-is-dns/) is the phonebook of the Internet.

## Name resolution

Name resolution is important because it is the process of mapping what's known as a fully qualified domain name or an FQDN to an IP address.

## Fully-qualified domain name

A fully qualified domain name is a combination of what's known as **a host name and a domain name**. When we talk about .com .org .gov etc., that is the farthest right portion of what's known as the DNS name space. Our DNS servers are responsible for locating records within the domain name space. The next part of this domain name is typically the company or the organization that has basically leased the portion of that name space. And then finally, we have what's known as the host and the host is typically owned and controlled by the company whose portion of that DNS name space we see here.

```text
# example
https://www.example.com

# protocol
https://

# subdomain
www

# domain name
example

# top-level domain
com

# root domain (domain name and top-level name)
example.com
```

## Name resolution process

1. A user types ‘example.com’ into a web browser and the query travels into the Internet and is received by a DNS recursive resolver.
2. The resolver then queries a DNS root nameserver (.).
3. The root server then responds to the resolver with the address of a Top Level Domain (TLD) DNS server (such as .com or .net), which stores the information for its domains. When searching for example.com, our request is pointed toward the .com TLD.
4. The resolver then makes a request to the .com TLD.
5. The TLD server then responds with the IP address of the domain’s nameserver, example.com.
6. Lastly, the recursive resolver sends a query to the domain’s nameserver.
7. The IP address for example.com is then returned to the resolver from the nameserver.
8. The DNS resolver then responds to the web browser with the IP address of the domain requested initially.

Once the 8 steps of the DNS lookup have returned the IP address for example.com, the browser is able to make the request for the web page:

10. The browser makes a [HTTP](https://www.cloudflare.com/learning/ddos/glossary/hypertext-transfer-protocol-http/) request to the IP address.
11. The server at that IP returns the webpage to be rendered in the browser.

## DNS database and records

[DNS records](https://www.cloudflare.com/learning/dns/dns-records/) (aka zone files) are instructions that live in authoritative [DNS servers](https://www.cloudflare.com/learning/dns/dns-server-types/) and provide information about a domain including what [IP address](https://www.cloudflare.com/learning/dns/glossary/what-is-my-ip-address/) is associated with that domain and how to handle requests for that domain. These records consist of a series of text files written in what is known as DNS syntax. DNS syntax is just a string of characters used as commands that tell the DNS server what to do.

### What are the most common types of DNS record?

- **A record** - The record that holds the IP address of a domain. [Learn more about the A record.](https://www.cloudflare.com/learning/dns/dns-records/dns-a-record/)
- **AAAA record** - The record that contains the IPv6 address for a domain (as opposed to A records, which list the IPv4 address). [Learn more about the AAAA record.](https://www.cloudflare.com/learning/dns/dns-records/dns-aaaa-record/)
- **CNAME record** - Forwards one domain or subdomain to another domain, does NOT provide an IP address. [Learn more about the CNAME record.](https://www.cloudflare.com/learning/dns/dns-records/dns-cname-record/)
- **MX record** - Directs mail to an email server. [Learn more about the MX record.](https://www.cloudflare.com/learning/dns/dns-records/dns-mx-record/)
- **TXT record** - Lets an admin store text notes in the record. These records are often used for email security. [Learn more about the TXT record.](https://www.cloudflare.com/learning/dns/dns-records/dns-txt-record/)
- **NS record** - Stores the name server for a DNS entry. [Learn more about the NS record.](https://www.cloudflare.com/learning/dns/dns-records/dns-ns-record/)
- **SOA record** - Stores admin information about a domain. [Learn more about the SOA record.](https://www.cloudflare.com/learning/dns/dns-records/dns-soa-record/)
- **SRV record** - Specifies a port for specific services. [Learn more about the SRV record.](https://www.cloudflare.com/learning/dns/dns-records/dns-srv-record/)
- **PTR record** - Provides a domain name in reverse-lookups. [Learn more about the PTR record.](https://www.cloudflare.com/learning/dns/dns-records/dns-ptr-record/)
