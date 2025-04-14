# Hill Cipher Web Application

A modern web application for encrypting and decrypting text using the Hill Cipher algorithm. This tool provides an intuitive interface for matrix-based cryptography operations.

## Features

### Encryption

- Text to number conversion using A=0, B=1, ..., Z=25 mapping
- Support for variable size key matrices (2x2 to 5x5)
- Automatic padding with 'X' for incomplete blocks
- Real-time matrix validation
- Modular arithmetic operations (mod 26)
- Visual feedback for successful encryption

### Decryption

- Support for decrypting Hill Cipher encrypted text
- Automatic matrix inverse calculation
- Matrix invertibility checking
- Error handling for non-invertible matrices
- Input validation for matrix dimensions
- Clear visual feedback for results

## How It Works

### Encryption Process

1. Enter your plaintext (only letters A-Z are accepted)

2. Select matrix size (2-5)
3. Enter your key matrix values row by row
4. Click "Encrypt" to get your ciphertext

### Decryption Process

1. Enter the ciphertext
2. Select the same matrix size used for encryption
3. Enter the same key matrix used for encryption
4. Click "Decrypt" to recover the plaintext

## Installation and Setup

1. Clone the repository:

```bash
git clone https://github.com/yourusername/hill-cipher-app.git
cd hill-cipher-app
```

1. Install dependencies:

```bash
pip install -r requirements.txt
```

1. Run the application:

```bash
python app.py
```

1. Open your browser and navigate to:

```plaintext
http://localhost:5000
```

## Requirements

- Python 3.x
- Flask
- NumPy

## Technical Details

### Matrix Operations

- The application uses NumPy for efficient matrix operations
- Modular arithmetic is implemented for all operations (mod 26)
- Matrix invertibility is checked before processing
- Determinant calculations are performed with proper modular arithmetic

### Error Handling

- Invalid matrix dimensions
- Non-invertible matrices
- Invalid input characters
- Matrix parsing errors
- Server communication errors

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
