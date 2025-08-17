<!-- Improved compatibility of back to top link: See: https://github.com/dhmnr/skipr/pull/73 -->
<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h3 align="center">🔐 Cryptography Toolkit with GUI</h3>

  <p align="center">
    A comprehensive collection of cryptographic algorithms implemented in Python with user-friendly Tkinter graphical interfaces for encryption, decryption, and key management.
    <br />
    <a href="https://github.com/virtual457/Cryptography-with-GUI-tkinter-"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/virtual457/Cryptography-with-GUI-tkinter-">View Demo</a>
    ·
    <a href="https://github.com/virtual457/Cryptography-with-GUI-tkinter-/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    ·
    <a href="https://github.com/virtual457/Cryptography-with-GUI-tkinter-/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

Cryptography Toolkit with GUI is an educational and practical implementation of various cryptographic algorithms, providing both command-line and graphical user interfaces. This project demonstrates fundamental concepts in cryptography and network security while offering an intuitive way to understand encryption and decryption processes.

The toolkit includes implementations of classical ciphers, modern cryptographic algorithms, and key exchange protocols, making it an excellent resource for learning cryptography concepts and practical applications.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Features

- **RSA Encryption**: Complete implementation of RSA public-key cryptography
- **Caesar Cipher**: Classical substitution cipher with customizable shift values
- **Playfair Cipher**: Digraphic substitution cipher implementation
- **Hill Cipher**: Matrix-based polygraphic substitution cipher
- **Diffie-Hellman**: Key exchange protocol for secure communication
- **GUI Interface**: User-friendly Tkinter-based graphical interfaces
- **Key Generation**: Automatic generation of cryptographic keys
- **Educational Value**: Clear implementation for learning purposes

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Cryptographic Algorithms Implemented

#### 1. RSA (Rivest-Shamir-Adleman)
- **Type**: Asymmetric encryption
- **Key Features**: Public/private key pair generation
- **Security**: Based on the difficulty of factoring large prime numbers
- **Use Cases**: Digital signatures, secure key exchange

#### 2. Caesar Cipher
- **Type**: Substitution cipher
- **Key Features**: Simple shift-based encryption
- **Security**: Basic (educational purposes)
- **Use Cases**: Learning cryptography fundamentals

#### 3. Playfair Cipher
- **Type**: Digraphic substitution cipher
- **Key Features**: Uses a 5x5 matrix based on a keyword
- **Security**: More secure than simple substitution
- **Use Cases**: Historical cryptography, educational purposes

#### 4. Hill Cipher
- **Type**: Polygraphic substitution cipher
- **Key Features**: Matrix-based encryption using linear algebra
- **Security**: Vulnerable to known-plaintext attacks
- **Use Cases**: Educational cryptography, matrix operations

#### 5. Diffie-Hellman Key Exchange
- **Type**: Key exchange protocol
- **Key Features**: Secure key exchange over insecure channels
- **Security**: Based on discrete logarithm problem
- **Use Cases**: Establishing shared secret keys

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

- [Python 3.x](https://www.python.org/) - Core programming language
- [Tkinter](https://docs.python.org/3/library/tkinter.html) - GUI framework
- [NumPy](https://numpy.org/) - Mathematical operations and matrix handling
- [Random](https://docs.python.org/3/library/random.html) - Cryptographically secure random number generation
- [Math](https://docs.python.org/3/library/math.html) - Mathematical functions for cryptographic operations

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

- Python 3.7 or higher
- pip package manager
- Basic understanding of cryptography concepts (optional but recommended)

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/virtual457/Cryptography-with-GUI-tkinter-.git
   ```
2. Navigate to the project directory
   ```sh
   cd Cryptography-with-GUI-tkinter-
   ```
3. Install required dependencies
   ```sh
   pip install numpy tkinter
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

### RSA Encryption/Decryption

```python
python cns/rsa.py
```

**Features:**
- Generate public/private key pairs
- Encrypt messages using private key
- Decrypt messages using public key
- Interactive command-line interface

**Example Usage:**
```
RSA Encrypter/ Decrypter
Enter a prime number (17, 19, 23, etc): 17
Enter another prime number (Not one you entered above): 19
Generating your public/private keypairs now . . .
Your public key is (5, 323) and your private key is (77, 323)
Enter a message to encrypt with your private key: Hello World
Your encrypted message is: [list of encrypted values]
Decrypting message with public key (5, 323) . . .
Your message is: Hello World
```

### Caesar Cipher

```python
python cns/ceaser/caesar.py
```

**Features:**
- Customizable shift values
- Encrypt/decrypt text messages
- GUI interface for easy interaction

### Playfair Cipher

```python
python cns/playfair/playfair.py
```

**Features:**
- Keyword-based matrix generation
- Digraphic encryption (pairs of letters)
- Handles special cases and padding

### Hill Cipher

```python
python cns/hill/hill.py
```

**Features:**
- Matrix-based encryption
- Configurable matrix sizes
- Linear algebra operations

### Diffie-Hellman Key Exchange

```python
python cns/deffie/diffie_hellman.py
```

**Features:**
- Secure key exchange simulation
- Prime number and primitive root selection
- Shared secret key generation

### GUI Applications

The project includes Tkinter-based graphical interfaces for each cipher:

```python
python cns/ctk.py
```

**GUI Features:**
- Intuitive user interface
- Real-time encryption/decryption
- Key management tools
- File input/output support

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [ ] Add AES (Advanced Encryption Standard) implementation
- [ ] Implement SHA-256 hash function
- [ ] Add digital signature functionality
- [ ] Create web-based interface using Flask
- [ ] Add support for file encryption/decryption
- [ ] Implement elliptic curve cryptography (ECC)
- [ ] Add password-based key derivation (PBKDF2)
- [ ] Create comprehensive documentation for each algorithm
- [ ] Add unit tests for all cryptographic functions
- [ ] Implement secure random number generation improvements

See the [open issues](https://github.com/virtual457/Cryptography-with-GUI-tkinter-/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Chandan Gowda K S - chandan.keelara@gmail.com

Project Link: [https://github.com/virtual457/Cryptography-with-GUI-tkinter-](https://github.com/virtual457/Cryptography-with-GUI-tkinter-)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Cryptography Documentation](https://cryptography.io/) - Python cryptography library
* [Applied Cryptography by Bruce Schneier](https://www.schneier.com/books/applied-cryptography/) - Essential cryptography reference
* [Python Documentation](https://docs.python.org/) - Official Python documentation
* [Tkinter Tutorial](https://docs.python.org/3/library/tkinter.html) - GUI development guide
* [NumPy Documentation](https://numpy.org/doc/) - Numerical computing library

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/virtual457/Cryptography-with-GUI-tkinter-.svg?style=for-the-badge
[contributors-url]: https://github.com/virtual457/Cryptography-with-GUI-tkinter-/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/virtual457/Cryptography-with-GUI-tkinter-.svg?style=for-the-badge
[forks-url]: https://github.com/virtual457/Cryptography-with-GUI-tkinter-/network/members
[stars-shield]: https://img.shields.io/github/stars/virtual457/Cryptography-with-GUI-tkinter-.svg?style=for-the-badge
[stars-url]: https://github.com/virtual457/Cryptography-with-GUI-tkinter-/stargazers
[issues-shield]: https://img.shields.io/github/issues/virtual457/Cryptography-with-GUI-tkinter-.svg?style=for-the-badge
[issues-url]: https://github.com/virtual457/Cryptography-with-GUI-tkinter-/issues
[license-shield]: https://img.shields.io/github/license/virtual457/Cryptography-with-GUI-tkinter-.svg?style=for-the-badge
[license-url]: https://github.com/virtual457/Cryptography-with-GUI-tkinter-/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/chandan-gowda-k-s-765194186/
