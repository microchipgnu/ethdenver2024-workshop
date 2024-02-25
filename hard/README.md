# Autonomous Wallet

This document outlines the steps to set up your local development environment, create a NEAR account, and get your Autonomous Wallet ready.

## Prerequisites

Before you start, ensure you have the following:

- A modern CPU with at least 4 cores (8 cores recommended for running 13B models).
- At least 8GB of RAM for 3B models, 16GB for 7B models.
- Internet connection for downloading necessary tools and models.
- (Optional) A GPU to enhance performance for larger models.

## Setup Guide

### Step 1: Local Development Environment Setup

#### 1.1 Install Ollama

Ollama allows you to download and run LLMs (Large Language Models) locally.

- Visit [Ollama's website](https://ollama.com/) and follow the installation instructions.

#### 1.2 Install the OpenHermes Model

- Run the following command in your terminal:

```sh
ollama pull openhermes
```

- For more information, visit [OpenHermes](https://ollama.com/library/openhermes).

#### 1.3 Install Bun

Bun is used for project dependencies management and execution.

- Installation instructions for different operating systems can be found at [Bun's documentation](https://bun.sh/docs/installation#installing).

### Step 2: Create a NEAR Account

NEAR Protocol is a scalable, developer-friendly blockchain network.

#### 2.1 Create an Account

- Navigate to [My NEAR Wallet](https://testnet.mynearwallet.com/) and follow the steps to create a new account.

#### 2.2 Fund Your Account

- Obtain initial funds for your account at the [NEAR Faucet](https://near-faucet.io).

#### 2.3 Export Your Private Key

- Export your private key from [My NEAR Wallet](https://testnet.mynearwallet.com/profile) for later use.

### Step 3: Autonomous Wallet Setup

The NEAR Autonomous Wallet leverages AI agents for advanced wallet functionalities.

#### 3.1 Fork the Repository

- Fork the [NEAR Autonomous Wallet](https://github.com/microchipgnu/near-autonomous-wallet) repository from GitHub.

#### 3.2 Project Installation

- Navigate to your project directory and install dependencies:

```sh
bun i
```

#### 3.3 Setup Environment Variables

- Create a `.env` file in your project root and add the following configurations:

```env
OPENAI_API_BASE=http://127.0.0.1:11434/v1
OPENAI_API_KEY=ollama-no-need-api-key

NEAR_ACCOUNT_ID=<YOUR_ACCOUNT_ID>
NEAR_ACCOUNT_FULL_ACCESS_KEY=<YOUR_PRIVATE_KEY>
```

#### 3.4 Run Your Autonomous Wallet

- Start your autonomous wallet with Bun:

```sh
bun run start
```
