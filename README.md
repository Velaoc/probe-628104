<!-- foundation:identity -->
# probe-628104

One-page guestbook: visitors type a short message and see the wall of messages, newest first. No accounts, no commerce the smallest possible foundation app.

- Site: https://probe-628104.api.holode.xyz
- Support: support@probe-628104.api.holode.xyz
<!-- /foundation:identity -->

## What this is

One-page guestbook: visitors type a short message and see the wall of messages, newest first. No accounts, no commerce — the smallest possible foundation app.

## Who it is for

- Visitor

## Main features

- **Post a message** — Visitor types a name and a short message and submits; it appears at the top of the wall.
- **View the wall** — Public root lists all messages, newest first.

## Core entities

- Message

## Run locally

```bash
bundle install
bin/rails db:prepare
bin/dev
```

Requires Ruby, PostgreSQL, and the usual Rails toolchain. See `bin/setup` if present.

## Demo

Three sample messages with names and timestamps so the wall looks alive on first load.

## Deploy notes

Production `config.hosts` is derived from `domain` in `config/foundation.yml`. Keep that value aligned with the real host or every request will 403.
