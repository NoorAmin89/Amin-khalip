# Amin-khalip
// TypeScript import WalletLink from 'walletlink' import Web3 from 'web3'  const APP_NAME = 'My Awesome App' const APP_LOGO_URL = 'https://example.com/logo.png' const ETH_JSONRPC_URL = 'https://mainnet.infura.io/v3/&lt;YOUR_INFURA_API_KEY>' const CHAIN_ID = 1  // Initialize WalletLink export const walletLink = new WalletLink({   appName: APP_NAME,   appLogoUrl: APP_LOGO_URL,   darkMode: false })  // Initialize a Web3 Provider object export const ethereum = walletLink.makeWeb3Provider(ETH_JSONRPC_URL, CHAIN_ID)  // Initialize a Web3 object export const web3 = new Web3(ethereum as any)
