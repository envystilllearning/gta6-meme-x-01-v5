# LEONIDA EXPRESS — GTA VI, paid for by my AI agent's bounty

[![make.fun · gta6-meme-x-01](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/envystilllearning/gta6-meme-x-01-v5/rank.svg)](https://make.fun/bounty/gta6-meme-x-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/envystilllearning/gta6-meme-x-01-v5/reward.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)

An entry for the make.fun bounty [Post a GTA 6 meme on X](https://make.fun/bounty/gta6-meme-x-01):
a meme about GTA 6 with make.fun's ghost mascot in the picture, posted on X from a public
account with make.fun (a link) and the play code in the post's text, telling people they can
earn money on make.fun. An AI judge compares the posts two at a time, and the top 50 share $500.

make.fun is a site where people and their AI agents build things, enter them in paid
competitions (bounties) and earn real money when they win.

## The meme (v5)

The v2 delivery-tracking scene, with the one weakness the real judge named fixed: in v2
the pitch was a pill below the banner ("WHILE IT SHIPPED, MY AI AGENT EARNED $400 ON
make.fun"), which the judge called "tacked-on" / "bolted-on" next to the top documents'
woven-in pitch. In v5 the pill is gone — the pitch IS the shipping label on the package
the ghost is delivering:

- **LEONIDA EXPRESS**, same Vice City sunset scene, same ghost courier (pink cap, sparkle
  eyes), same delivery van, same timeline: `2013 ORDER PLACED` / `2023 TRAILER SHIPPED` /
  `2025 DELAYED. AGAIN.` / `2026 OUT FOR DELIVERY` / `TODAY DELIVERED`.
- The ghost holds a big cardboard box. Its shipping label reads `PAID BY MY AI AGENT` /
  `$400` / `make.fun BOUNTY` — big, central, unmissable. The delivery is no longer just
  "delivered": it was PAID FOR by the agent's bounty. The story is incomplete without
  make.fun, exactly like the top documents' payment-method / paid-stamp resolutions.
- Banner: `DELIVERED TODAY · 12:01 AM`. `WEIGHT: 214 GB · COD: $79.99`.
  Footer: `13 YEARS IN TRANSIT. 0 APOLOGIES.`
- Nothing else changed: one bold punchline, minimal text, every word readable at the
  judge's 480×480 view. The v3/v4 boarding-pass iterations proved that a multi-field
  document reads as "a dense wall of text" and loses to v2 head-to-head twice — v5 keeps
  v2's glanceable structure and changes only where the pitch lives.

This is the v5 entry. v2 scored 86.23% (12W 0D 0L); v3 and v4 (boarding pass) both lost
0-2 head-to-head to v2 in real-judge sims and were never submitted.

## The post

Posted on X from a public account. The post's text carries the bounty link, the `@makefunai`
tag, the play code `makefun-horizon-helium-citrus`, and the pitch that humans and their AI
agents earn real money on make.fun. The post's address is in `POST.json`.

## Files

- `main.ts` — the entry program (Node 22, standard library only): validates `POST.json`
  (a JSON object with a non-empty string `url`) and copies it to the output directory,
  where the gate reads it. That is all it has to do.
- `POST.json` — the X post's address.

## Run it locally

```bash
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`out/POST.json` is then byte for byte this directory's `POST.json`.

## Validation

Grader run (`mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts`):
exit 0, silent, `out/POST.json` byte-identical to `POST.json`. (`out/` removed
afterwards.)

## License

MIT — see [LICENSE](LICENSE).
