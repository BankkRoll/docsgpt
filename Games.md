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
