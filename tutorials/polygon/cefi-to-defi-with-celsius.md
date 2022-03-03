---
description: >-
  Celsius bridge allows people to get their favorite assets on
  Polygon and benefit from DeFi without selling them. Let's see how.
---

# From CeFi to DeFi with Celsius

## Introduction

[Celsius Network](https://celsius.network/) is one of the big CeFi players where people can easily buy crypto assets with their bank account and stake the purchased tokens to get extra rewards. As an example, you can earn 6.20% APY on your BTC (Bitcoin), 5.35% on your ETH (Ether) etc ... Besides holding your assets and getting weekly gains that compound, you can also borrow additional assets against the one you already own (that are then used as collateral) to leverage your position or swap for other tokens. However, Celsius is a closed network, and this is why it's often referenced as a CeFi application (**Ce**ntralized **Fi**nance).

If you have assets on Celsius, you can still send them to other applications on the tokens' native blockchain. As an example, you can transfer ETH in and out of Celsius using your Ethereum wallet, or BTC using your address on the Bitcoin chain. In addition to this, Celsius launched in February a new bridge called CelsiusX that allows you to send some specific assets from the Celsius application to Polygon. The current tokens that are supported are

* ETH, the native token of the Ethereum Mainnet
* ADA, the native token of Cardano
* DOGE, the native token of Dogecoin blockchain

By sending your assets on Polygon, you also get a full access to the DeFi ecosystem, as well as additional bridge options to move your tokens to Fantom, Avalanche, and many more other chains. This guide will guide you through the different steps to get your assets from Celsius to Polygon, and will present a few things you can do there.

{% hint style="info" %}
This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs, end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.
{% endhint %}

![](<../../.gitbook/assets/Celsius-Coinbase-17.png>)

## Getting assets on Celsius

### Get an account

Of course, in order to be able to use Celsius, you will need a Celsius account. Simply head to their website and register a new account [using this link](https://celsius.onelink.me/EyfO/5321754e). Please note that for legal reasons, and because of the nature of the business model of Celsius, you will need to provide proofs of your identity, also known as KYC documents (**K**now **Y**our **C**ustomer), such as a driving license. Also, note that the Celsius application may not be available in your country. Check their [Terms of Use](https://celsius.network/terms-of-use) and [Privacy Policy](https://celsius.network/privacy-policy) for additional details.

{% hint style="info" %}
Please note that this guide, Mai Finance, or the QiDAO community is not responsible for the services provided by Celsius, and it is strongly recommended to do your own research before registering for a financial product.
{% endhint %}

Once your account is created, feel free to take a quick tour of the web application, and you can also download the mobile application.

### Getting your assets into your account

The mobile application is, for now, the only way for you to purchase assets directly using a Credit Card or a Bank Transfer. This option may also be restricted to certain countries/regions. Due to these restrictions, we will not cover this option, but feel free to explore this option if that's something you'd be willing to do.

For this guide, we will focus on ETH, and we will also assume you already have some Ether on the Ethereum Mainnet that you want to bridge to Celsius. From the web application, simply navigate to the `Receive` tab.

![Receiving ETH in your Celsius account in 4 simple steps](<../../.gitbook/assets/Celsius-Coinbase-0.png>)

The first step is to add the coin you want to receive. In our case, we want to get ETH, and it's as easy as clicking `Add New Coins` button and selecting ETH from the dropdown.

![List of accepted coins on Celsius](<../../.gitbook/assets/Celsius-Coinbase-6.png>)

Once selected, you will have the possibility to get the wallet address that corresponds to your Celsius account on the Ethereum network.

![Receiving address for ETH](<../../.gitbook/assets/Celsius-Coinbase-1.png>)

If you click on `View and Copy address`, a new popup will open with a QR code representing your wallet address on Celsius network, as well as its value in plain text that you can simply copy and paste.

![Feel free to send me some ETH](<../../.gitbook/assets/Celsius-Coinbase-2.png>)

With the wallet address, you initiate a transfer from where you have your Ether tokens. The example below is taken from Coinbase (another big player in the CeFi industry):

![Sending $100 worth of ETH from Coinbase to Celsius](<../../.gitbook/assets/Celsius-Coinbase-5.png>)

Of course, and as always with Ethereum Mainnet, you will have to pay some transaction fees. This is absolutely not linked to Coinbase or Celsius. As you can see below, a direct transfer from my MetaMask wallet would also require me to pay some fees. 

![Sending ETH form MetaMask to Celsius](<../../.gitbook/assets/Celsius-Coinbase-18.png>)

{% hint style="info" %}
Depending on the congestion of the network, the fees may be quite high. Make sure you check the gas price to benefit from the lowest fees possible.
{% endhint %}

Once the transfer is completed, you should be able to see your assets in your Celsius dashboard:

![The ETH is now in my Celsius account](<../../.gitbook/assets/Celsius-Coinbase-7.png>)

At this point, if I'm keeping the coins in my account on Celsius, I will receive staking rewards every week. For ETH, and as of March 2022, the APY is 5.35%. However, we will now have the possibility to move the assets to Polygon using the CelsiusX bridge **for free**. Simply head to the `Send` tab and select the asset you want to transfer to Polygon.

{% hint style="info" %}
Note: if you don't have any recipient address saved yet, now is time to create one. Pick your wallet address from Metamask and add it as your withdrawal address. For security reasons, when you create a withdrawal address or change it, this address is locked for 24h. As you will see in the screenshot below, 24 hours after I transferred $100 worth of ETH to Celsius, my balance already changed in price.
{% endhint %}

![Sending ETH from Celsius to my Polygon wallet](<../../.gitbook/assets/Celsius-Coinbase-9.png>)

You can also notice on this screenshot that I will receive cxETH on Polygon, which is a wrapped version of ETH. It would be the same thing for ADA (you'll get cxADA) and DOGE (you'll get cxDOGE). We will see later in this guide what to do with your cxTokens.

{% hint style="success" %}
Note that there are absolutely no fees for this transfer. It's also very fast.
{% endhint %}

Once sent, you will get an email asking you to confirm the transfer (always more security) and you will be able to see your transaction history reflecting this transfer in the Celsius app.

![Funds have been sent, see you on Polygon](<../../.gitbook/assets/Celsius-Coinbase-11.png>)

After a few minutes, you will have your assets (cxTokens) available in your wallet on Polygon. The best way to keep track of these transfers is probably to use [an application like DeBank](https://debank.com/) and take a look at your transaction history on the desired chain (here Polygon):

![Transaction as seen in your history on DeBank](<../../.gitbook/assets/Celsius-Coinbase-12.png>)

## Polygon and cxTokens

### What are cxTokens

Without going too deep in the details, cxTokens are wrapped tokens. When you transfer your assets from the Celsius Network to Polygon, the assets are kept locked in the Celsius Network and new tokens are minted on Polygon. However, for the case of Ether, Celsius doesn't have the possibility to mint WETH on Polygon directly, so they create a token which price is indexed on the price of ETH: cxETH.

The opposite is also true, meaning that when you transfer your cxETH back to Celsius, the cxToken is burnt and a corresponding amount of ETH is released on Celsius and added to your account.

To make sure the price of the cxToken is properly indexed on the price of the underlying asset, Celsius is using a Chainlink's technology: the Proof of Reserve.

If you are curious about the fine details of how Celsius is managing their cxTokens, you can read all the details in their [medium article from January 2022](https://medium.com/@CelsiusX/celsius-is-integrating-chainlink-proof-of-reserve-to-unlock-cross-chain-liquidity-with-wrapped-6c85bb2f2a60).

### Swapping your cxTokens

Because your cxTokens are wrapped versions of the underlying assets, you may not find many applications that will accept them as is. Luckily enough, you can swap them for some other assets using [QuickSwap DEX](https://quickswap.exchange/#/swap), the only DEX with liquidity for the cxTokens on Polygon as of March 2022.

![Swapping cxETH for ETH on QuickSwap](<../../.gitbook/assets/Celsius-Coinbase-13.png>)

Obviously, you can also operate the reverse operation and buy cxTokens using other assets.

{% hint style="success" %}
When you're swapping in or out of cxTokens, pay attention to the route taken, as well as the slippage. QuickSwap seems to only use 4 hops at most, and to access cxDOGE as an example, you always need to go through ETH, cxETH, and then cxDOGE. This means you need to have enough liquidity between the asset you swap and ETH so that the route can be ASSET > ETH > cxETH > cxDOGE.

That's currently not the case for MAI as an example. You may want to do MAI > USDC > ETH > cxETH in a first swap, and cxETH > cxDOGE in a second swap.

The same goes when you want to get out of your cxTokens: cxDOGE to MAI may suffer from high slippage, and you probably will want to go through cxETH or ETH first.
{% endhint %}

## Providing liquidity with your cxTokens

With you cxTokens, you can provide liquidity to the CelsiusX pools on QuickSwap. The previous paragraph explains how to swap your cxTokens, and this is done using LP pools (**L**iquidity **P**oviding pools). In order to make sure any user can swap their tokens, QuickSwap will give rewards paid in dQUICK and MATIC to users who stake their liquidity on their application. The 3 pairs that will get you rewards are

* ETH/cxETH
* cxETH/cxADA
* cxETH/cxDOGE

They all have different levels of rewards, and the best thing to do is to go to the QuickSwap app and check their dual mining programs.

![Details of the ETH/cxETH pool on QuickSwap as of March 2022](<../../.gitbook/assets/Celsius-Coinbase-15.png>)

In the screenshot above, you can see that if you provide liquidity for the ETH-cxETH pair, you can get up to 15% APY (**A**nnual **P**ercentage **Y**ield, which assumes you will compound the rewards) paid in dQUICK, WMATIC, and directly into ETH and cxETH from swap fees. If you don't compound the rewards, that's still a 13.97% APR that you will get, and you will be able to do whatever you want with the reward tokens. Feel free to explore this guide to get additional ideas on how to use them.

{% hint style="success" %}
To enter a liquidity pool, simply [provide liquidity](https://quickswap.exchange/#/add/0x7ceB23fD6bC0adD59E62ac25578270cFf1b9f619/0xfe4546feFe124F30788c4Cc1BB9AA6907A7987F9) for the chosen pair in a 1:1 ratio. This may mean you will have to swap some cxTokens for something else. Once the LP pair is created, you can deposit it in the pool, and start accumulating yields.
{% endhint %}

## Use your cxTokens as collateral and take a loan

Swapping your cxTokens means you are actually selling them to buy something else. [Mai Finance](https://app.mai.finance) is a DeFi (**De**centaralized **Fi**nance) application that will allow you to keep your assets locked in a vault and borrow some stable coins against them. Then you will be able to do whatever you want with your loan, including

* farming stable coins
* swapping the MAI stablecoin borrowed to buy other assets
* leverage your cxTokens
* bridge your MAI to other chains

Just explore the different pages of this guide to collect ideas on how to use your loan in a way that suits you the best.

**Note :** when you borrow the MAI stable coin on Mai Finance, you get paid with Qi tokens based on the amount you borrow. The reward rates vary based on the total amount borrowed for that vault, the price of Qi, and the Qi allocation for the vault. More details in our [guide on vault rewards](<../../mai-university/mai-loans-and-vaults-incentives.md>).

![Vault status for the cxTokens as of March 2022](<../../.gitbook/assets/Celsius-Coinbase-19.png>)

And of course, you can combine both solutions by swapping your MAI loan into LP pair of cxTokens and farm yields on QuickSwap. At this point, there's no limit to what you can do, and your initial investment is fully preserved in your vault on Mai Finance (as long as you don't get liquidated).

![](<../../.gitbook/assets/Celsius-Coinbase-20.png>)

## Disclaimer

This guide has been written to present to you how you can benefit from CelsiusX, the bridge between Celsius Network and Polygon, and experiment with everything DeFi can offer on Polygon. Of course, using protocols on Polygon presents risks. If you're using cxTokens as collateral on Mai Finance, you will have to pay attention to liquidations in case the price of your collateral position goes below the liquidation ratio, a threshold that indicates your loan may have a bigger value than the assets backing it. These risks are presented in several tutorials on this site, so once again, you are highly encouraged to read some of them and make sure you understand how the different protocols presented in this guide are working before investing anything. And as always, this is not financial advice, always do your own research.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}

