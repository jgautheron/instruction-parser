# Parser for Jupiter V5 Contract

A library you can use to parse the Jupiter v5 swap instruction. It is also the same library that we use to parse the swap information on the https://station.jup.ag/stats page.

After cloning the repo, in the project directory run `yarn install`. Then:


```
yarn start lookup-tx --signature <TRANSACTION_SIGNATURE> --rpc <RPC_URL>
```

For an example on how to use the library, you can check out: `src/cli.ts`.

## Note

We are using Anchor events for extracting swap details. One downside about this approach is that we cannot longer extract swap details if the log is being truncated.

## Jupiter V4 Contract

For the old V4 contract, check out [v4 tag](https://github.com/jup-ag/instruction-parser/tree/v4).

## Jupiter V3 Contract

For the old V3 contract, check out [v3 tag](https://github.com/jup-ag/instruction-parser/tree/v3).