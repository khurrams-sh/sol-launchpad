# Sol Launchpad

A modern Solana token launchpad platform powered by Meteora's Dynamic Bonding Curve (DBC) technology. Create and trade tokens with real-time price discovery, built-in liquidity, and seamless trading.

## 🚀 Features

- **Token Creation**: Launch tokens with customizable bonding curves
- **Real-time Trading**: Integrated Jupiter Terminal for instant swaps
- **Live Data**: WebSocket streaming for prices, volume, and transactions
- **Mobile Responsive**: Optimized for all devices
- **Advanced Charts**: TradingView integration with technical indicators
- **Token Discovery**: Browse and filter newly launched tokens

## 🛠 Tech Stack

- **Frontend**: Next.js 15, TypeScript, Tailwind CSS
- **Blockchain**: Solana Web3.js, Meteora DBC SDK
- **Real-time Data**: Jupiter APIs & WebSocket streaming
- **Storage**: Cloudflare R2
- **Charts**: TradingView integration

## 📦 Installation

1. Clone the repository

```bash
git clone <your-repo-url>
cd sol-launchpad
```

2. Install dependencies

```bash
pnpm install
```

3. Set up environment variables

Create a `.env.local` file in the root directory:

```env
# Cloudflare R2 Storage (for token metadata & images)
R2_ACCESS_KEY_ID=your_r2_access_key_id
R2_SECRET_ACCESS_KEY=your_r2_secret_access_key
R2_ACCOUNT_ID=your_r2_account_id
R2_BUCKET=your_r2_bucket_name

# Solana RPC URL (Helius, QuickNode, etc.)
RPC_URL=your_rpc_url

# Meteora Pool Configuration
POOL_CONFIG_KEY=your_pool_config_key
```

4. Run the development server

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) to see your launchpad.

## 🔧 Configuration

### Cloudflare R2 Setup
1. Create account at [Cloudflare](https://dash.cloudflare.com)
2. Navigate to R2 Object Storage
3. Create a bucket for token metadata
4. Generate API tokens with R2 edit permissions

### Solana RPC Provider
Get an RPC URL from providers like:
- [Helius](https://helius.xyz)
- [QuickNode](https://quicknode.com)
- [Alchemy](https://alchemy.com)

### Pool Config Key
The pool configuration key defines bonding curve parameters. Contact Meteora for configuration options.

## 🚀 Deployment

### Deploy to Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)

1. Push to GitHub
2. Connect to Vercel
3. Add environment variables
4. Deploy

### Environment Variables
Set these in your deployment platform:
- `R2_ACCESS_KEY_ID`
- `R2_SECRET_ACCESS_KEY` 
- `R2_ACCOUNT_ID`
- `R2_BUCKET`
- `RPC_URL`
- `POOL_CONFIG_KEY`

## 📖 How It Works

1. **Token Creation**: Users create tokens with custom metadata and bonding curve parameters
2. **Price Discovery**: Meteora's DBC provides automatic pricing based on supply/demand
3. **Real-time Updates**: Jupiter WebSocket streams live price and transaction data
4. **Trading**: Integrated Jupiter Terminal enables instant token swaps
5. **Graduation**: Successful tokens can graduate to full AMM pools

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

Built with [Meteora's Dynamic Bonding Curve](https://meteora.ag) technology and [Jupiter](https://jup.ag) infrastructure.
