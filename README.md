# LockSphere File Tool
The LockSphere File Tool is a powerful and versatile utility for handling files with a custom .sphere extension. This tool provides encryption/decryption, keyword search, file metadata viewing, and batch processing capabilities.

# Features
  - Convert files to a custom .sphere extension
  - Read .sphere files and convert them back to their original format
  - Encrypt and decrypt files using Fernet or ChaCha20-Poly1305 encryption methods
  - Password protection for encrypted files
  - Keyword search within files
  - View file metadata
  - Batch process files for encryption, decryption, keyword search, and metadata viewing
  
  
 # Possible Use Cases
  - Securely store sensitive files by encrypting them with strong encryption algorithms
  - Protect confidential information by making files unreadable without the correct password
  - Search for specific keywords within multiple files
  - View file metadata to gain insights into file properties
  - Perform batch operations on multiple files at once, saving time and effort
  
  
 # Encryption Methods: Fernet vs ChaCha20-Poly1305
The LockSphere File Tool supports two encryption methods: Fernet and ChaCha20-Poly1305. Here's a brief overview of their strengths and weaknesses:

Fernet
  - Fernet is a high-level symmetric encryption recipe provided by the Python cryptography library. It uses AES-128 in CBC mode with PKCS7 padding for encryption and HMAC-SHA256 for authentication.

# Strengths:

  - Easy to use and understand
  - Provides strong encryption and authentication
  - Resistant to tampering
# Weaknesses:

  - Slightly slower than ChaCha20-Poly1305
  -Less suitable for systems with limited resources or performance constraints

# ChaCha20-Poly1305
ChaCha20-Poly1305 is a modern authenticated encryption scheme that combines the ChaCha20 stream cipher with the Poly1305 authenticator. It's designed to be fast and secure, even on systems with limited resources.

# Strengths:

  - Faster than Fernet (AES-128 in CBC mode)
  - Suitable for systems with limited resources or performance constraints
  - Offers strong encryption and authentication

# Weaknesses:

  - Slightly more complex to use and understand
  - Not as widely known or adopted as AES

# When deciding which encryption method to use for your specific use case, consider the following factors:

Batch processing vs single files: 
  - ChaCha20-Poly1305 might be a better option for batch processing, as it's faster and more suitable for systems with limited resources. Fernet can still be used for single files or smaller batches, where the performance difference may not be significant.

Ease of use vs performance: 
  - If ease of use and understanding are a priority, Fernet is a more straightforward option. However, if performance and resource constraints are essential factors, ChaCha20-Poly1305 may be more suitable.

Compatibility and adoption: 
  - Fernet (AES) is more widely known and adopted, which may be an essential factor if compatibility with other systems is required.
Consider these factors when choosing the appropriate encryption method for your needs.


# Comparison to Similar Products
  Compared to other file management tools, the LockSphere File Tool offers unique features, such as:
  - A custom .sphere file extension for added security and obscurity
  - Two encryption methods (Fernet and ChaCha20-Poly1305) to choose from
  - Keyword search functionality to quickly locate information within files
  - File metadata viewing for a better understanding of file properties
  - Batch processing capabilities for increased efficiency



# License
This project is licensed under the MIT License. See the LICENSE file for more information.
