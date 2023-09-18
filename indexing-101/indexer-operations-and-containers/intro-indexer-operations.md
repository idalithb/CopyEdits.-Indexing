# Wallets Overview
It is crucial to understand that **wallets** are essential and necessary tools to securely manage and access Ethereum accounts. 

Ethereum wallets within the Web3 ecosystem are applications that allow you access to your account. They function like physical wallets where your identification and assets are held. Wallets allow you to sign into apps, view balances, send transactions, and verify your I.D. 

> It’s helpful to think of wallets as windows to view and manage your assets on Ethereum, and _**not**_ as an Ethereum account. So, a wallet allows you to use the keys associated with your Ethereum account to interact with it. 

However, most wallet products will let you generate an Ethereum account, so you don't need one before you download a wallet. 

**Types of wallets:**
  - Physical hardware wallets are physical devices that allow you to keep your crypto offline and they are the most secure.
  - Mobile application wallets allow you to easily access your accounts.
  - Browser wallets are web applications that allow you interact with your account directly on a browser.
  - Broser extension wallets are extensions that you download to interact with your account through a browser.
  - Desktop applications allow you to manage your funds from your macOS, Windows, or Linux system. 

_Keep this in mind as we move forward, and we review the differences between hot and cold wallets._

## Hot Wallets ##

----

Hot wallets are online wallets that are _**always**_ connected to the internet; they can be web-based, mobile, or a desktop app. They have private keys that grant you access to your blockchain address and all your digital assets. 

### Types of Hot Wallets: ###
  - Web Wallets: Allow you access to your account via web browser. They are provided by various online platforms such as MyEtherWallet, MetaMask, and Trust Wallet
  - Mobile Wallets: Apps that allow you quick on-the-go access to your account such as Trust Wallet and Coinbase Wallet

**Pros:**
  - They are highly convenient
  - Give you quick access 

**Cons:**
  - They are more vulnerable to cyber-attacks and hacks
  - They are considered less secure compared to cold wallets  

### Function & Security ###


You typically download and install hot wallets on your computer, smartphone, or use online wallet services.
When setting up the wallet, you generate a cryptographic key pair:
  - **Public Key:** Allows you to receive assets—this is the wallet address where others can send cryptocurrency to you.
  - **Private Key:** Authorizes direct access to assets within a blockchain address; it is used to access and control the funds in the wallet. This is a secret key that you must keep secure and never share with anyone. 

There are two broad categories of hot wallets, based on how you can access your account’s private keys: 

**Custodial wallets**, also known as hosted wallets or third-party wallets, are crypto exchange wallets like Binance and Coinbase. With this type of wallet, the third-party provider holds and manages your cryptocurrency assets on your behalf. They allow you to view your public keys, but the custodian or wallet provider controls the private keys. You access your wallet via login credentials, but it has no direct link to the address on the blockchain where your funds are stored. 
Essentially, you rely on the custodian to facilitate access. These types of wallets are designed to be user-friendly and more accessible. 

**Non-custodial wallets**, also known as self-hosted wallets, give you absolute control of your assets by leaving you in charge of the private key for this blockchain address. This means that you have direct access to your blockchain address, independently of the wallet. 
You get a seed phrase, a 12-word recovery phrase, when you set up the wallet. This seed phrase encodes your private keys and helps you regain access to the wallet if you lose your device. An example of a non-custodial hot wallet is Metamask. 

## Cold Wallets ##

---

Cold wallets, also known as cold storage solutions, are cryptocurrency wallets that are not connected to the internet. They protect your crypto by generating and storing private keys offline. It’s important to note that these keys are not the same as the seed phrase you generate every time you create a wallet (i.e., see hot wallets), but they are needed to sign a transaction and whoever holds them has authority to move that crypto to another address. 

### Types of Cold Wallets: ###
  - Hardware Wallets: Physical devices, like USB drives, that store your cryptocurrency keys offline. which means they are immune to online attacks.
  - Paper Wallets: A physical document that contains a public address for receiving cryptocurrency and a private key for spending or transferring the cryptocurrency. Since it's a physical item, it's immune to online threats. However, it must be stored securely to prevent physical theft or damage.
  - Metal Wallets: Are made of durable materials like metal but are like paper wallets and store cryptocurrency private keys. They are resistant to physical damage from fire or water.
  - Offline Software Wallets: These are installed on a computer that has never been connected to the internet. This isolation ensures that the wallet and its private keys are never exposed to online threats.

**Pros:**
  - Eliminate the risk of theft or hacking
  - Considered long-term storage of cryptocurrencies
  - Offer better security
    
**Cons:**
  - Cannot be accessed from anywhere since they’re offline

### Function: Regular Cold & Ultra-Cold Storage ###

There are two approaches to broadcasting signed transactions to the network when completing the transaction signing process: regular cold storage and ultra-cold storage.

**Regular Cold Storage** 

_What do you do?_

You connect the offline cold storage wallet to another device with an internet connection using a USB cable. This enables you to plug the hardware wallet into MetaMask to sign transactions, which allows you access to smart contracts. You can provide liquidity, vote on governance proposals, and even take out loans. Every transaction requires you to enter a pin on the device manually. 

_What are the potential risks?_

Although it is more secure than hot wallets, any USB connection can expose your device to malware.

_What are the benefits?_

Each initiated transaction is temporarily transferred to the secure offline space on the wallet, which stores the private key. The transaction is signed and returned to the online environment before being broadcast on the blockchain network. This process takes place in a matter of seconds, so it hides the complexities from you.


