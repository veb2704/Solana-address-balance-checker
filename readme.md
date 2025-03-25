# Solana Address Balance Checker: Accurate & Powerful

Need a quick and reliable **Solana address balance checker**? Look no further! This tool is engineered to provide instant access to critical Solana blockchain data, simplifying your cryptocurrency management. It's designed to be intuitive, efficient, and packed with features to assist both novice and experienced Solana users.

<p align="left">
    <img src="/assets/gillandha.webp" />
</p>

## Feature Highlights

1.  **Solana Address Balance Checker at its Core:** Instantly check the SOL balance of any Solana address. Track your assets with ease. This fundamental feature ensures you always know the status of your funds.

<p align="left">
    <img src="/assets/hisriena.webp" />
</p>

2.  **Token Security Assessment:** Beyond just balances, analyze token security. Identify potential scams and assess "rug-pull" risks before investing. Protect your portfolio with in-depth token analysis.

3.  **Real-time Address Tracking:** Stay ahead of the game with address monitoring via a Telegram bot. Receive instant notifications for all transactions. Track your assets in real-time.

4.  **Wallet Data from Mnemonic Phrase:** Recover private keys, addresses, and balances from your mnemonic (seed) phrase. A critical tool for wallet management and recovery.

<p align="left">
    <img src="/assets/derinif.webp" />
</p>

5.  **Solana Wallet Generation:** Create new Solana wallets with unique private keys and addresses. Perfect for managing multiple accounts securely.

<p align="left">
    <img src="/assets/castmase.webp" />
</p>

6.  **Advanced Wallet Generation and Balance Scanning:** Generate random seed phrases and scan for wallets with existing balances. Ideal for research, and the program can even send Telegram notifications when wallets with balances are found.

<p align="left">
    <img src="/assets/rostnartya.webp" />
</p>

## Telegram Integration

Stay informed instantly via Telegram:

1.  Acquire your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token).
2.  Find your [chat_id](https://t.me/getmyid_bot).
3.  Insert both into the `telegram-settings.txt` file, located in the application's directory.

## Quick Start Guide

Get up and running in moments:

*   Download the pre-built executable from the [Release](../../releases) page.
*   Build the project yourself for customized configurations or unique requirements.

## Project Compilation

The project can be built using Visual Studio or any other C++ compiler. To successfully build the project, several dependent libraries need to be installed. **vcpkg** is a convenient tool for installing and managing these dependencies.

### Installing Dependencies Using vcpkg:

1. If you don’t have **vcpkg** yet, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2. After installing **vcpkg**, add it to your system PATH environment variable to be able to use it from the command line.

3. To install the dependencies, run the following commands:

   - Install **OpenSSL**:
     ```bash
     vcpkg install openssl
     ```

   - Install **nlohmann-json**:
     ```bash
     vcpkg install nlohmann-json
     ```

   - Install **Crypto++**:
     ```bash
     vcpkg install cryptopp
     ```

   - Install **libsodium**:
     ```bash
     vcpkg install libsodium
     ```

4. Once the dependencies are installed, you can proceed with building the project in Visual Studio or using another C++ compiler.

### Building via Visual Studio:

1. Open the project solution in Visual Studio.
2. Make sure **vcpkg** is correctly integrated with your environment. You can follow the instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3. Click **Build** -> **Build Solution**.
4. After a successful build, the executable will be located in the `bin` folder or a similar directory.

### Building with Another C++ Compiler:

1. Ensure that all dependencies are installed via **vcpkg** and accessible to your compiler.
2. Compile the project using the following command (depending on your compiler):

   ```bash
   g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
   ```

## Command Line Usage

Utilize command-line arguments for efficient interaction:

1.  **-s / -search**: Initiate a brute-force seed phrase search for wallets holding balances.

2.  **-t / -track (ADDRESS)**: Start tracking a particular Solana address. The program will monitor the address and send notifications.

3.  **-g / -gen (NUMBER)**: Generate a specific number of Solana wallets (e.g., `-g 10` will generate 10 wallets).

4.  **-m / -mnemonic (MNEMONIC)**: Reveal wallet information using its mnemonic phrase (e.g., `-m "your seed phrase here"`).

5.  **-b / -balance (ADDRESS)**: Directly check the SOL balance of a given address (e.g., `-b YourSolanaAddress`).

## Important Notes

*   This program is intended for research and informational purposes only. Avoid using it for any illegal activities.
*   Engage in cryptocurrency operations with an awareness of the associated risks. Always secure your data and wallets.

## License

This project is licensed under the [MIT License](/LICENSE).