# CLOUT roulette airdrop

Single-file site (`index.html`): Solana CT influencer card roulette, X tasks, in-app balance, collection, referrals.

## Economy (edit `cfg` and `RF` at the top of the script)
- 1 free spin, $20 for completing the X tasks, $5 per spin
- Odds / card value: Common 45% $1 · Uncommon 30% $2 · Rare 21.5% $4 · Epic 3% $15 · Legendary 0.5% $100 (RTP ≈ 57%)
- Insta sell pays 80% of card value
- Referral: $2.50 per friend, link = `domain/@xhandle` (customizable slug)

## Backend TODO
- X OAuth → set `cfg.authUrl`, return handle via `window.CLOUT_X = {handle}` or `?x=` on callback
- Route `/@slug` to index.html (also supports `?ref=slug`)
- Server-side referral credit, slug uniqueness, task verification, balance and spins
- Set `cfg.domain`, `cfg.postUrl`
