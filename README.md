# SHA-256 Encryption Implementation

This repository contains a Python implementation of the SHA-256 encryption algorithm. SHA-256 (Secure Hash Algorithm 256-bit) is one of the cryptographic hash functions designed by the National Security Agency (NSA) and is widely used in various security applications and protocols.

## Usage

### Prerequisites

- Python 3.x

### Getting Started

1. Clone this repository:

    ```bash
    git clone https://github.com/sayantancodex/SHA-256-Encryption-Implementation
    ```

2. Navigate to the project directory:

    ```bash
    cd SHA-256-Encryption-Implementation
    ```

3. Run the script with a string input:

    ```bash
    python sha256.py "your_message_here"
    ```

## Implementation Details

The `sha256.py` script provides an implementation of the SHA-256 hash function. Here's a brief overview of the key components:

- **Padding**: The input message is padded to ensure its length is a multiple of 512 bits.
- **Parsing**: The padded message is divided into 512-bit blocks.
- **Initial Hash Value**: Initial hash values (`h0` to `h7`) are set as per the SHA-256 specification.
- **Message Schedule**: For each message block, a message schedule is prepared based on the previous message block.
- **Compression Function**: The compression function iterates over the message blocks, updating the hash values based on the current block and the message schedule.

## Contributors

- [Sayantan Patra](https://github.com/sayantancodex)

## License

This project is licensed under the [MIT License](LICENSE).
