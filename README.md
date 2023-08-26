# Image Steganography Program

This Python program allows you to hide one image within another image using a basic form of steganography. Steganography is the practice of concealing data within another piece of data to keep it hidden from prying eyes. In this case, you can hide an image (referred to as the encrypting image) within another image (referred to as the target image) using a simple technique.

## Prerequisites

- Python 3.x
- OpenCV library (cv2)

## Installation

1. Make sure you have Python 3.x installed on your system. You can download it from the official website: [Python Downloads](https://www.python.org/downloads/)

2. Install the OpenCV library using the following command:
   ```
   pip install opencv-python
   ```

## Usage

1. Clone or download this repository to your local machine.

2. Import the OpenCV library and the functions `encrypt` and `decrypt` from the provided Python script.

3. **Encryption**:
   The `encrypt` function takes three parameters:
   - `targetpath`: Path to the target image (the image in which the other image will be hidden).
   - `encryptingimgpath`: Path to the image you want to hide within the target image.
   - `outpath`: Path to save the resulting encrypted image.

   Example usage:
   ```python
   import cv2
   from steganography_program import encrypt

   target_image_path = 'path/to/target/image.jpg'
   encrypting_image_path = 'path/to/encrypting/image.jpg'
   output_path = 'path/to/save/encrypted/image.jpg'

   encrypt(target_image_path, encrypting_image_path, output_path)
   ```

4. **Decryption**:
   The `decrypt` function takes two parameters:
   - `encryptedimg`: Path to the encrypted image (resulting from the encryption process).
   - `outpath`: Path to save the decrypted image.

   Example usage:
   ```python
   import cv2
   from steganography_program import decrypt

   encrypted_image_path = 'path/to/encrypted/image.jpg'
   decrypted_output_path = 'path/to/save/decrypted/image.jpg'

   decrypt(encrypted_image_path, decrypted_output_path)
   ```

## Important Notes

- The images used for encryption and decryption should ideally have the same dimensions.
- This program uses a basic steganography technique that might not be suitable for secure data transmission.

## Legal Disclaimer

This program is provided for educational and informational purposes only. The developers are not responsible for any misuse or illegal activities that may arise from using this program. Always ensure that you have the right to manipulate and use the images involved.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request to this repository.

