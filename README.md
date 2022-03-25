# Easy LN address with LNDhub.go

This code is meant to be hosted on [Vercel](https://vercel.com).

[LNDhub.go](https://github.com/getalby/lndhub.go) supports unauthenticated invoice requests and `description_hash`, you only need your LNDhub username.
These endpoints should give you a fully functioning LN Address on your own domain that is backed by an LNDhub.go server such as https://ln.getalby.com.

LNURL Comments are supported, payer info is not.


## Vercel instructions

- Fork this repo
- Signup on [Vercel](https://vercel.com)
- Link your Github account
- Import this project in Vercel
- In the project configuration page, add the following environment variables:
    - LNDHUB_HOST: eg. `ln.getalby.com` (be aware that lndhub.io will not work)
    - LNDHUB_LOGIN: the "username" of your LNDhub account (lndhub://USERNAME:password@https://example.com)
    - (optional) MIN_SENDABLE: the minimum amount of msats people should send. Default 1000 (minimum 1000)
    - (optional) MAX_SENDABLE: the maximum amount of msats people should send. Default 1e10 (0.1 BTC).
