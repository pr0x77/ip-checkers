# IP & DNS Checkers — RULE-SET for Shadowrocket / Surge

A curated list of popular IP, DNS-leak, WebRTC, browser-fingerprint, blacklist and speed-test checker websites — packaged as a ready-to-use `DOMAIN-SUFFIX` rule-set for proxy clients.

[![Domains](https://img.shields.io/badge/domains-66-blue)](ip-checkers.list)
[![Updated](https://img.shields.io/badge/updated-2026--11--04-lightgrey)](commits/main)

## Usage

Add to your `[Rule]` section. **Important:** place this rule *above* your `GEOIP` rules, otherwise test pages will be hijacked by geo-routing and you will see the wrong exit IP.

### Shadowrocket

```
https://raw.githubusercontent.com/pr0x77/ip-checkers/main/ip-checkers.list
```

### Surge

```
RULE-SET,https://raw.githubusercontent.com/pr0x77/ip-checkers/main/ip-checkers.list,🔍 Checkers
```

Replace the policy/group with your own. A dedicated `select` group is recommended — it lets you switch *whose* IP you are testing (auto node / specific node / DIRECT) with one tap.

## Categories

| Category | Domains | Examples |
|---|---|---|
| Whoami / IP info | 19 | 2ip, ifconfig.me, ipinfo.io, ip.sb, whoer |
| DNS leak tests | 10 | dnsleaktest, ipleak, browserleaks, ping.space |
| DNS propagation / tools | 7 | dnschecker.org, whatsmydns, intodns, he.net |
| Browser fingerprint / WebRTC | 7 | browserscan, amiunique, iphey, EFF Cover Your Tracks |
| IPv6 check | 2 | test-ipv6.com, ipv6-test.com |
| Blacklist / IP reputation | 5 | scamalytics, abuseipdb, talos, spamhaus |
| GeoIP lookup | 4 | ip2location, geoiptool, db-ip |
| Speed / connectivity | 8 | speedtest, fast.com, check-host.net, ping.pe |
| HTTP echo / headers | 1 | httpbin.org |

## Contributing

PRs are welcome. One `DOMAIN-SUFFIX` per line, alphabetical order within a category, keep the header comment block intact.

## License

MIT — see [LICENSE](LICENSE).
