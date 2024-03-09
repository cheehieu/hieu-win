# nimble-hour

This is a sandbox repo for developing a GitHub Pages portfolio. I'll be testing some things out with a more modern approach...

## DNS

To set up [GitHub Pages with a custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) from Namecheap, adjust the DNS settings to include the following records:

+----------+------------------+----------------------------------------+---------+
| **Type** | **Host** | **Value** | **TTL** |
+----------+------------------+----------------------------------------+---------+
| A | @ | 185.199.108.153 | Auto |
+----------+------------------+----------------------------------------+---------+
| A | @ | 185.199.109.153 | Auto |
+----------+------------------+----------------------------------------+---------+
| A | @ | 185.199.110.153 | Auto |
+----------+------------------+----------------------------------------+---------+
| A | @ | 185.199.111.153 | Auto |
+----------+------------------+----------------------------------------+---------+
| AAAA | @ | 2606:50c0:8000::153 | Auto |
+----------+------------------+----------------------------------------+---------+
| AAAA | @ | 2606:50c0:8001::153 | Auto |
+----------+------------------+----------------------------------------+---------+
| AAAA | @ | 2606:50c0:8002::153 | Auto |
+----------+------------------+----------------------------------------+---------+
| AAAA | @ | 2606:50c0:8003::153 | Auto |
+----------+------------------+----------------------------------------+---------+
| CNAME | www | cheehieu.github.io. | Auto |
+----------+------------------+----------------------------------------+---------+
| TXT | @ | zoho-verification=...zmverify.zoho.com | Auto |
+----------+------------------+----------------------------------------+---------+
| TXT | @ | v=spf1 include:zoho.com ~all | Auto |
+----------+------------------+----------------------------------------+---------+
| TXT | zmail.\_domainkey | v=DKIM1; k=rsa; p=... | Auto |
+----------+------------------+----------------------------------------+---------+

For a free email account using the custom domain with Zoho, adjust the mail settings to "Custom MX" and add the following records:

+----------+------------------+----------------------------------------+----+---------+
| **Type** | **Host** | **Value** | | **TTL** |
+----------+------------------+----------------------------------------+----+---------+
| MX | @ | mx.zoho.com | 10 | Auto |
+----------+------------------+----------------------------------------+----+---------+
| MX | @ | mx2.zoho.com | 20 | Auto |
+----------+------------------+----------------------------------------+----+---------+
| MX | @ | mx3.zoho.com | 50 | Auto |
+----------+------------------+----------------------------------------+----+---------+

## TODO

- simplify home screen with links to LinkedIn, GitHub, Resume (pdf), Contact
- About Me section
- Projects section
- Resume section
- optimize for mobile
- optimize load times, image sizes
- support for light/dark themes
- analytics
- Jekyll blogs
- Disqus commenting
