### [🎰 Apps](./Apps.md): Guides and information related to Gamba applications built within this project.
Gamba Apps/Platforms are frontends that interact with the Gamba on-chain Program, typically by allowing users to play betting games. Owners can earn revenue by having a Solana address attached to each play occurring on their App (known as a "creator address"). This means that they can make use of Gamba's liquidity across various tokens, earn fees on plays, all without risking a dime of their own. A simple webpage is all that's needed to host a betting app like a game or a casino. No backend deployments are necessary.

### [💧 Pools](./Pools.md): Information on Gamba pools and related components.
Gamba liquidity pools serve as counterparties to bets made by players via various frontend apps. They function similarly to the house of a traditional casino, with the added benefit that anyone can participate and earn a part of the profits.

### [🎲 Games](./Games.md): Learn about the exciting Gamba games available in this project.
Games are initiated by the player, typically via a frontend app. The Gamba on-chain Program will validate each game, ensuring the player doesn't have an unfair advantage. A random number is then generated to determine the winner (either the player or the liquidity pool being played against).

---

- [🚀 Next.js Integration](./Nextjs.md): Integration guide for Gamba with Next.js applications.
- [⚡ Vite.js Integration](./Vite.md): Integration guide for Gamba with Vite.js applications.

### Packages

- [![gamba-core-v2](https://img.shields.io/npm/v/gamba-core-v2?color=blue&label=gamba-core-v2)](https://www.npmjs.com/package/gamba-core-v2) Core package with a provider for the Anchor program + utilities.

- [![gamba-react-v2](https://img.shields.io/npm/v/gamba-react-v2?color=blue&label=gamba-react-v2)](https://www.npmjs.com/package/gamba-react-v2) Essential hooks and context providers for interacting with the Gamba program in a React app.

- [![gamba-react-ui-v2](https://img.shields.io/npm/v/gamba-react-ui-v2?color=blue&label=gamba-react-ui-v2)](https://www.npmjs.com/package/gamba-react-ui-v2) UI components and utilities.
