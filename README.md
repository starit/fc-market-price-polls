# Farcaster Frames MarketSense

A simple Market Price Prediction app using [Farcaster Frames](https://warpcast.notion.site/Farcaster-Frames-4bd47fe97dc74a42a48d3a234636d8c5).

This example lets you create a market prediction poll and have users vote on it. Those who win the prediction will be rewarded an NFT after checking the price from oracle.

On-chain smart contracts and Oracle price verification are used.

## Related Repos

- [Farcaster MarketSense Scripts](https://github.com/starit/fc-prediction-scripts)
- [Farcaster MarketSense Smart Contracts](https://github.com/starit/fc-prediction-contracts)
- [Farcaster MarketSense Frames](https://github.com/starit/fc-prediction-frames)

## Demo

- [https://fc-market-price-polls.vercel.app/](https://fc-market-price-polls.vercel.app/)
- [Warpcast Frames Developer Tool](https://warpcast.com/~/developers/frames)

### Launched Prediction Frame

Notice: The Chain means the blockchain for users to receive the rewardings.

- [Base][BTC] How will BTC's price change from $50,000 in a week? https://fc-market-price-polls.vercel.app/polls/37d99a88-280b-43e7-93df-97c0df5ecd31

- [Linea][ETH] How will ETH's price change from $3,500 in a week? https://fc-market-price-polls.vercel.app/polls/cbc44873-f88d-47de-a1f6-701509610deb

- [Hedera][BTC] How will BTC's price change from $50,000 in a week? https://fc-market-price-polls.vercel.app/polls/2b6fe656-cccf-4636-8c3b-ce85001c63e6


## Setup
- After deploying your repo to Vercel...
- Create a `kv` database `https://vercel.com/<name>/<project>/stores`
- Set the `KV` prefix url's for the new `kv` database
- Navigate to env variables: https://vercel.com/gregan/fc-links-vote/settings/environment-variables
- If you're doing something production facing w/ trusted data, set the `HUB_URL` environment variable to a production hub's public ip address port 2283 ref: https://docs.farcaster.xyz/reference/frames/spec#frame-signature-packet
- Set the `HOST` env variable to your public facing url or domain, ie; `https://<project>.vercel.app/`
