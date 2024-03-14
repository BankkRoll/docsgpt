# 🎲 Apps

Gamba Apps/Platforms are the cutting-edge frontends that merge flawlessly with the Gamba on-chain program. These platforms empower users to partake in an array of betting games, harnessing blockchain's might to guarantee fairness and transparency.

### 💡 The Essence of Gamba Apps

At their heart, 🎲 Gamba Apps are crafted to offer an immersive betting experience, linking users directly with the decentralized gaming world of Gamba. App owners tap into Gamba's vast liquidity pools across various tokens, generating revenue through transaction fees without any financial risk on their part.

## 💸 Revenue Generation Model

### Creator Address

The bedrock of income for app proprietors is the "creator address"—a distinct Solana address tied to each app. This ingenious system captures a slice of the transaction fees from gameplay, diving into the rich liquidity pools of Gamba.

#### Advantages:

- **Access to Gamba's Liquidity**: Utilize the abundant liquidity available across diverse tokens within the Gamba ecosystem.
- **Fee-Based Revenue**: Benefit from the transaction fees produced by the betting games on your platform.
- **Zero Initial Investment**: Create a revenue stream without any upfront financial outlay.

## 🛠️ Simplified Platform Setup

Launching a Gamba App is designed to be as simple as possible, necessitating nothing more than a basic webpage to get started. This methodology strips away the need for backend deployments, simplifying the process for anyone to kickstart their betting games or casinos.

### 🚀 Getting Started with Your Gamba App

Venturing into the development and hosting of your Gamba App is a straightforward path:

1. **Discover Existing Applications**: Kick off by visiting the [Gamba Platforms Explorer](https://explorer.gamba.so/platforms) to survey the landscape of live apps for inspiration.
2. **Adopt a Template**: Check out our [Example Page](https://docs-v2-delta.vercel.app/docs/examples) for a selection of customizable templates that align with your app's vision.

#### Steps to Launch:

- **Template Selection**: Choose a template from our assortment that matches your app's theme.
- **Customization**: Tailor the chosen template with your unique branding, desired game mechanics, and integrate your Solana creator address.
- **Deployment**: Publish your customized webpage on a hosting platform like GitHub Pages, Vercel, or Netlify, all offering straightforward, free hosting services.
- **Promotion**: Amplify your app's presence by connecting with the Gamba community and leveraging various marketing strategies to draw in users.


---

# 🎮 Games

Gamba Games represent the core of the gaming experience on the platform, powered by the innovative Gamba on-chain program. Players initiate games through a frontend app, engaging in a fair competition either against other players or the liquidity pool itself.

### 🛠 How Games Work

At the heart of every game lies the Gamba on-chain program, ensuring fairness and transparency by validating each game to prevent any unfair advantage. A cryptographically secure random number generation (RNG) mechanism determines the game's outcome, making each play a blend of strategy and chance.

## 🏗 Game Structure

The anatomy of a Gamba game consists of several critical components:

- **Pool**: Utilizes a specific liquidity pool and its underlying token for the game.
- **Wager**: The token amount placed by the player to participate in the game.
- **Bet**: An array of possible outcomes, represented as multipliers, which dictate the potential winnings.

### 🎲 Outcomes Explained

The essence of a bet lies in its multipliers. When a game kicks off, the system randomly selects a multiplier from the bet array. This multiplier then acts on the wagered amount to calculate the player's winnings.

For example:
- A coin toss game might use a bet array like `[2, 0]`, signifying a double win or nothing.
- More complex games adjust the array length and values to offer a varied range of outcomes, with fairness as the guiding principle.

Allowed and disallowed bets:
- `[0, 2]` (Equal odds) ➡️ Allowed ✅
- `[1.5, .5]` (Equal odds) ➡️ Allowed ✅
- `[0, 0, 0, 6]` (Player advantage) ➡️ Not Allowed ❌
- `[0, 3]` (Player advantage) ➡️ Not Allowed ❌

This flexible system enables the creation of diverse game types, from classics like Roulette and Plinko to innovative new formats.

## 🔐 Determining the Outcome

Gamba ensures the integrity and fairness of game results through several mechanisms:

- **rng_seed**: Supplied by Gamba's trusted RNG Provider.
- **client_seed**: Provided by the player's browser, customizable for varied game outcomes.
- **nonce**: Incrementally assigned to each bet, enhancing security and randomness.

### Security and Fair Play

Players receive an encrypted hash of the `rng_seed` before the game begins, assuring them that the outcome cannot be manipulated. The opportunity to adjust the `client_seed` allows players to influence the randomness, adding an element of control.

## 🕵️‍♂️ Verification and Transparency

The Gamba explorer plays a vital role in maintaining transparency, tracking games played across different frontends and offering proofs and methods to verify game outcomes.

- **Example Transaction**: For an in-depth look at a game's transaction and its verification process, visit [this link](https://explorer.gamba.so/tx/23ARo5bzvKXr5MJVMUnGtvfEYWHp4aPfvthna1Px5P8GCV5uBtqE7q37CQqhC7uhzA5PU7mEMBBkCDYi16oJqRK7).


---


# 🏦 Liquidity Pools

Gamba's liquidity pools are the cornerstone of the betting ecosystem, acting as the house that players bet against. These pools are not just integral to the mechanics of Gamba; they embody the spirit of decentralization and profit-sharing.

## 🚀 Creating a Pool

Creating a liquidity pool on Gamba is as straightforward as it is rewarding. With support for any custom Solana token, pools offer a versatile foundation for the platform's diverse gaming offerings.

- **Explorer UI**: Dive right in and create or join an existing pool via the [Gamba Explorer](https://explorer.gamba.so/create). This intuitive interface ensures that anyone, regardless of technical prowess, can participate.
- **Gamba SDK**: For those looking to interact with pools programmatically or create more complex integrations, the Gamba SDK provides all the necessary tools. [Delve deeper into the SDK](https://docs.gamba.so/sdk) to unlock the full potential of Gamba's liquidity pools.

## 💰 LP Token Mechanics

Upon pool creation, a corresponding LP (Liquidity Provider) token is minted. This token is pivotal, representing your share in the pool's liquidity and potential earnings.

- **Initial Deposit Ratio**: Start with a 1:1 ratio of LP tokens to the underlying token. This equitable starting point ensures fairness for early contributors.
- **Dynamic Ratios**: As the pool's liquidity fluctuates with game outcomes, so does the ratio of LP tokens. Winners and losers affect the pool, but ultimately, liquidity providers stand to gain, especially when the LP token's value increases due to the pool's success.

## 🎁 Bonuses Galore

In a move to enhance player engagement, each pool features Bonus tokens, serving as incentives for participation or as free play options.

- **Minting and Usage**: Exchange the pool's underlying token for Bonus tokens, which are earmarked for betting. It's a one-way transaction — these tokens are burned after use, emphasizing their role as a dynamic engagement tool rather than a static currency.
- **Allocation**: 90% of the underlying tokens used for minting Bonus tokens feed into a dedicated fund, ripe for the winning. The remaining 10% bolster the jackpot pool, creating a tantalizing target for players.

## 🎰 Jackpot Dynamics

The jackpot represents the pinnacle of excitement within Gamba's ecosystem, growing with each failed attempt until a lucky player strikes it big.

- **Contribution**: A minor portion of the jackpot winnings is funneled back into the liquidity pool, ensuring its continued growth and sustainability.
- **Flexibility**: Platform developers have the autonomy to integrate the jackpot feature as they see fit, tailoring the experience to their audience's preferences.

## 📊 Fees & Payouts

Understanding the economic underpinnings of Gamba's pools is crucial. Upcoming features will provide transparency on fees and maximum payouts, ensuring all participants have clear insights into their potential earnings and contributions.

- **Fees & Max Payout**: Stay tuned for detailed disclosures on [current fees and payout structures](https://explorer.gamba.so/fees).

## 🔒 Private Pools: A Glimpse into the Future

Private pools generally work the same way as public ones, but gives its owner the ability to configure various parameters - like fees, max potential payout, and more.
