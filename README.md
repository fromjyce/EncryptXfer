# EncryptXfer: A Secure File Transfer Application

## Overview
The **Secure File Transfer Application** is designed to provide a secure method for transferring files over the internet. The application implements a protocol that ensures confidentiality and integrity during file uploads and downloads, using cryptographic techniques to protect against unauthorized access and data tampering.

## Supported Functionality
- **File Upload**: Clients can securely upload files to the server.
- **File Download**: Clients can securely download files from the server.
- **File Integrity**: Uploaded and downloaded files retain their original features. For example:
  - Executable files remain executable.
  - Image files remain unchanged and can be displayed as intended.

## Security Requirements
The application adheres to the following security requirements:

1. **Authentication**: 
   - Clients authenticate the server using the server’s RSA public key.

2. **Confidentiality**: 
   - Messages exchanged between the client and server are protected from unauthorized access. The only technology used for securing communication is keyed hashing, specifically **SHA-256**.
   - The application is designed to maintain confidentiality against well-known attacks.

3. **Integrity**: 
   - Any alteration of messages in transit is detected by both the client and server. The only mechanism used to achieve message integrity is a keyed hash function (SHA-256).

## Technical Specifications
- **Programming Language**: Python 3
- **Hashing Algorithm**: SHA-256
- **Encryption**: RSA Key Generation and usage

## Prerequisites
To run the application, ensure you have the following installed:

- Python 3
- Libraries for Multi-threading and Socket Programming
- Libraries for Cryptographic Hash Functions
- Libraries for Public Key Cryptography

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/fromjyce/EncryptXfer.git encryptxfer
   cd encryptxfer
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Start the server:
   ```bash
   python server.py
   ```

2. Start the client:
   ```bash
   python client.py
   ```

3. Follow the prompts in the client application to upload or download files securely.

## Example
To upload a file:
- Use the upload command and provide the file path.

To download a file:
- Use the download command and specify the file name.

## Running the Project

The programs have been tested on the Visual Studio Code IDE in Windows 11. You are free to choose any IDE that suits your needs.

## Contact

If you come across any issues, have suggestions for improvement, or want to discuss further enhancements, feel free to contact me at [jaya2004kra@gmail.com](mailto:jaya2004kra@gmail.com). Your feedback is greatly appreciated.

## License

All the code in this repository is licensed under the GNU GENERAL PUBLIC License. You are free to use and modify it for educational purposes. However, I do not take any responsibility for the accuracy or reliability of the code.

## My Social Profiles:

- [**LINKEDIN**](https://www.linkedin.com/in/jayashrek/)
