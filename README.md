# ethdenver2024-workshop

## Steps

### 1. Setup your local development environment

#### 1.1 Install [Ollama](https://ollama.com/)

#### 1.2 Install openhermes model

```sh
ollama pull openhermes
```

#### 1.3 Install Bun

Go to https://bun.sh/docs/installation#installing to see how to install in different OSes.

###### System Requirements

- RAM
  - For 3B models: 8GB
  - For 7B models: At least 16GB
- CPU: Any modern CPU with at least 4 cores is recommended; for running 13B models, a CPU with at least 8 cores is recommended
- GPU (Optional): A GPU is not required but can enhance performance, especially for larger models.

### 2. Create a NEAR Account

NEAR Protocol 

#### 2.1 Go to [Mintbase Wallet](https://wallet.mintbase.xyz)

#### 2.2 Create a new private key

#### 2.3 Add private key to your account

https://wallet.mintbase.xyz/import/private-key#%7BaccountID%7D/%7BprivateKey%7D

### 3. Get your Autonomous Wallet

#### 3.1 Fork the [NEAR Autonomous Wallet](https://github.com/microchipgnu/near-autonomous-wallet) repo

The NEAR Autonomous Wallet is a wallet system built on top of [micro-agi](https://github.com/microchipgnu/micro-agi) a framework that aims to make it easy to orchestrate groups of AI agents.

#### 3.2 Install the project

```sh
bun i
```

#### 3.2 Setup .env

#### 3.3 Run your autonomous wallet

```sh
bun run start
```
