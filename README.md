# DNS-Server

> **Fast • Secure • Lightweight • Multi-Upstream DNS-over-HTTPS Server powered by Cloudflare Workers**

A lightweight and production-ready DNS-over-HTTPS (DoH) server running entirely on Cloudflare Workers.

This project acts as a high-performance DNS proxy with support for multiple upstream providers, automatic failover, response caching, and low-latency request routing.

Designed for developers who need a reliable DoH endpoint without deploying traditional DNS infrastructure.

---

## ✨ Features

* ⚡ Ultra-fast DNS-over-HTTPS proxy
* 🌍 Multiple upstream DNS providers
* 🔄 Automatic failover
* 🚀 Lowest-latency upstream selection
* 💾 Built-in Cloudflare edge caching
* 📦 Lightweight serverless architecture
* 🔒 HTTPS only
* 🌐 Supports DNS Message and JSON APIs
* 🛠 Easy deployment with Cloudflare Workers
* 📄 Open source

---

## Supported Upstream Providers

The server can be configured to use one or more upstream DNS providers.

Examples include:

* Cloudflare DNS
* Google Public DNS
* Quad9
* NextDNS
* AdGuard DNS
* Mullvad DNS
* Control D

---

## Why this project?

Instead of exposing a single public resolver, this project forwards DNS queries to configurable upstream providers while taking advantage of Cloudflare's global edge network.

Benefits include:

* Lower latency
* Improved availability
* Better reliability
* Simple deployment
* No VPS required
* Free Cloudflare Worker tier supported

---

## Architecture

```
Client
   │
   ▼
Cloudflare Worker
   │
   ├── Cloudflare DNS
   ├── Google DNS
   ├── Quad9
   ├── NextDNS
   └── AdGuard
```

---

## Deployment

1. Clone the repository

```bash
git clone https://github.com/yourname/DNS-Server.git
```

2. Install dependencies

```bash
npm install
```

3. Login to Cloudflare

```bash
npx wrangler login
```

4. Deploy

```bash
npm run deploy
```

Your DNS-over-HTTPS endpoint will be available immediately.

---

## Roadmap

* Multiple upstream configuration
* Health checks
* Automatic upstream benchmarking
* Smart load balancing
* Analytics dashboard
* Custom DNS filtering
* Rate limiting
* Admin configuration page

---

## Contributing

Contributions, bug reports, feature requests, and pull requests are always welcome.

If you find this project useful, consider giving it a ⭐ on GitHub.

---

## License

This project is released under the Apache-2.0 License.
