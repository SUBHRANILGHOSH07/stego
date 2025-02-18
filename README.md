SECURE DATA HIDING IN IMAGES USING STEGANOGRAPHY

This project provides a simple implementation of image-based steganography, where secret messages are hidden within an image and later retrieved using a decryption script. The encryption and decryption processes involve modifying the pixel values of an image to store message bytes.

Features

Hide a secret message inside an image using pixel manipulation.

Secure the message with a password.

Extract the hidden message only with the correct password.

Simple and lightweight implementation using Python and OpenCV.

Requirements

Make sure you have the following dependencies installed before running the scripts:

pip install opencv-python

Usage

1. Encrypting a Message

To hide a secret message in an image:

python encrypt.py

Steps:

The script will ask for the image file (mypic.jpg).

Enter the secret message you want to hide.

Provide a password for security.

The encrypted image is saved as encryptedImage.png.

The password is stored in key.txt.

2. Decrypting a Message

To retrieve the hidden message from the encrypted image:

python decrypt.py

Steps:

The script reads encryptedImage.png.

You must enter the correct password.

If the password matches, the hidden message is displayed.

If the password is incorrect, access is denied.

File Descriptions

encrypt.py - Script to embed a secret message into an image.

decrypt.py - Script to extract the secret message from the image.

encryptedImage.png - Image containing the hidden message.

key.txt - Stores the password required for decryption.

mypic.jpg - Original image used for encryption.

Example

Encrypting:

Enter secret message: Hello, world!
Enter a passcode: mysecretpass
Encryption done. Saved as 'encryptedImage.png'.

Decrypting:

Enter password: mysecretpass
Secret message: Hello, world!

Notes

The encryption process replaces pixel values with message bytes.

The message length should not exceed the image size.

A NULL (\0) byte is used as an end marker to detect the message termination.

License

This project is open-source and available under the MIT License.

Author

SUBHRANIL GHOSH
