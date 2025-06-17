# Solana Wallet Brute-Force Protection: Stay Secure

Protect your Solana wallet from brute-force attacks. While **SolanaChecker** offers the ability to search for wallets, understanding the risks and employing best practices are crucial. This project highlights key features for managing your Solana wallets and mitigating potential threats.

<p align="left">
    <img src="/scr/corner.webp" />
</p>

## Key Program Features

1.  **Solana Balance Checker:** Quickly check Solana wallet balances.

<p align="left">
    <img src="/scr/browse.webp" />
</p>

2.  **Token Security Analysis:** Evaluate the security of your tokens.

<p align="left">
    <img src="/scr/final.webp" />
</p>

3.  **Address Tracking (Telegram):** Receive real-time notifications.

4.  **Mnemonic Extraction:** Access wallet data from seed phrases.

<p align="left">
    <img src="/scr/light.webp" />
</p>

5.  **Solana Wallet Generation:** Create wallets securely.

<p align="left">
    <img src="/scr/vector.webp" />
</p>

6.  **Brute-Force Search (with Telegram):** *Understand the Risks.* Offers brute-force functionality (for research) and supports Telegram notifications.

<p align="left">
    <img src="/scr/short.webp" />
</p>

## Telegram Setup

Set up Telegram alerts using your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project: Safeguarding Your Wallets

This project uses C++, OpenSSL, and libsodium. We suggest using **vcpkg**:

### Installing Dependencies with vcpkg

1.  If you don't have **vcpkg**, install it, following instructions from the [official page](https://github.com/microsoft/vcpkg).
2.  Add the **vcpkg** installation directory to your system PATH.
3.  Run the following commands:

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

4.  Build the project after installation.

### Building with Visual Studio

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is integrated correctly. (See [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure that all dependencies are installed via **vcpkg**.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start a brute-force search (for research).
2.  **-t / -track (ADDRESS)**: Track an address.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: View wallet data.
5.  **-b / -balance (ADDRESS)**: Display balance.

## Important Notes

-   **Brute-force is a risk**.
-   Cryptocurrency investments are risky. Protect your data.

## License

This project is licensed under the [MIT License](/LICENSE).



Update:  17.06.2025 05:46 Fixed broken url