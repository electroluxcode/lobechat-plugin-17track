# lobechat-plugin-17track

[LobeChat](https://github.com/lobehub/lobe-chat) function plugin for
[17TRACK](https://www.17track.net/) — cross-border e-commerce order tracking for
2900+ carriers (China Post, DHL, FedEx, UPS, USPS, Yanwen, Cainiao, etc.).

## Files

| File | Purpose |
|---|---|
| `public/manifest.json` | Plugin manifest (ChatGPT ai-plugin format), served raw |
| `public/openapi.json` | OpenAPI 3.1 spec for the 11 Tracking API v2.4 operations |
| `public/plugin.json` | LobeChat plugin entry copy |

Official API doc: https://asset.17track.net/api/document/v2.4_zh/index.html

## Auth

Each user brings their own 17TRACK API key (https://api.17track.net/admin/settings),
sent as the `17token` header — declared via the OpenAPI `securitySchemes`.

The plugin index entry lives in
[lobe-chat-plugins](https://github.com/lobehub/lobe-chat-plugins).
