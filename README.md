# OpenNFTauction


OpenNFTAuction is a decentralized auction platform designed to work on the BRC-20 standard using the Fractal Bitcoin chain. It allows users to list their NFTs for auction, place bids, and claim NFTs in a secure and decentralized manner. The platform integrates with the Unisat Wallet for seamless interaction with the Bitcoin network.

---

## Project Structure

- **contracts**: Smart contract logic for handling NFT auctions on the BRC-20 Fractal chain.
- **frontend**: User-friendly React-based interface for interacting with the auction platform.

---

## Getting Started

### Prerequisites

#### 1. Operating System

This project is compatible with macOS, Linux, and Windows.

#### 2. Node.js and npm

Ensure you have Node.js installed. Download it from [Node.js official website](https://nodejs.org/).

#### 3. Bun Runtime

Install Bun as the package manager for faster dependency management and runtime. Follow the [Bun installation guide](https://bun.sh/docs/installation) or run:

```bash
curl -fsSL https://bun.sh/install | bash
```

#### 4. Unisat Wallet

You will need the Unisat Wallet browser extension to connect your wallet and interact with the auction platform on the Fractal chain. Download it from the [Unisat website](https://unisat.io/).

#### 5. Fractal Testnet Tokens

To test the platform, you can get Fractal Bitcoin testnet tokens using the [Fractal Testnet Faucet](https://fractal-testnet.unisat.io/explorer/faucet).

### Clone the Repository

Clone the project from GitHub and navigate to the frontend directory to set up the application:

```bash
git clone https://github.com/Kishore-MK/OpenNFTauction.git
cd OpenNFTauction
```
### Frontend Setup

Navigate to the NftFrontend directory to set up and run the frontend application:

```bash
cd NftFrontend
npm install
npm run dev
```
### Using OpenNFTAuction

#### 1. Connect Wallet

  - Open the frontend in your browser.
  - Connect your Unisat Wallet to interact with the auction platform.

#### 2. Create an Auction

  - Select an NFT from your connected wallet.
  - Specify auction parameters such as starting bid, duration, and more.
  - Confirm the transaction to deploy the auction on the Fractal Bitcoin network.

#### 3. Place a Bid

  - Browse ongoing auctions.
  - Select an auction and place a bid.
  - Confirm the transaction in your Unisat Wallet.

#### 4. Claim NFT or Refund

   - If you win the auction, claim your NFT by completing the transaction.
   - If the auction ends without meeting the criteria, claim your refund.

## Environment Variables
To configure API keys and wallet settings, create an .env file in the NftFrontend directory based on the example provided:

```bash
cp .env.example .env
```
Edit the .env file to include your details:

```env
# Run npm run genprivkey to generate a private key along with a testnet address
# You can fund its address using the sCrypt faucet https://scrypt.io/faucet
PRIVATE_KEY=""
UNISAT_BASE_URL=https://open-api-fractal-testnet.unisat.io # testnet
UNISAT_API_KEY=<your_unisat_api_key>
```

## FAQ

### How to get BRC-20 tokens for testing?
Visit the [Fractal Testnet Faucet](https://fractal-testnet.unisat.io/explorer/faucet) to get testnet tokens.

### Can I use my main Unisat Wallet for testing?
We recommend creating a separate wallet for testing to avoid risks to your main wallet's assets.

### How to debug issues with the frontend?
Ensure all dependencies are installed, the .env file is correctly configured, and your Unisat Wallet is connected to the appropriate network.

## Todo

- Add advanced auction features like multiple bids per user.
- Support for dynamic fee structures.
- Implement additional wallet integration options.
- Develop a detailed auction analytics dashboard.

## References

  - [BRC-20 Standard](https://brc-20.com/)
  - [Fractal Bitcoin](https://www.fractalbitcoin.io/)
  - [Unisat Wallet](https://unisat.io/)
  - [React Documentation](https://reactjs.org/)

