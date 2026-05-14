# LSB-Image-Steganography-in-C
Developed an Image Steganography project in C using LSB encoding and decoding to securely hide secret text inside BMP images. Implemented file handling, bitwise operations, and data extraction techniques to ensure secure and accurate message transmission without affecting image quality.


This project implements Image Steganography using the Least Significant Bit (LSB) technique in Embedded C.
The main objective of the project is to securely hide a secret text message inside a BMP image file without noticeably changing the image quality.

The project supports both:

Encoding → Hiding secret data inside an image
Decoding → Extracting hidden data from the encoded image


Features
Encode secret text inside a BMP image
Decode hidden text from encoded image
Uses LSB (Least Significant Bit) technique
Command-line based execution
Efficient bitwise manipulation
Simple and lightweight implementation
Secure text hiding mechanism

Technologies Used
Embedded C
File Handling
Bitwise Operations
Pointers
Functions
Structures
Command Line Arguments


Project Structure
├── encode.c
├── decode.c
├── common.c
├── encode.h
├── decode.h
├── common.h
├── types.h
├── test_encode.bmp
├── secret.txt
├── stego.bmp
├── output.txt
└── README.md


Working Principle

Encoding Process
Read the source BMP image
Read the secret text file
Encode:
Magic string
Secret file extension
Secret file size
Secret data
Store secret bits into image byte LSBs
Generate encoded output image

Decoding Process
Read encoded BMP image
Decode magic string
Extract file extension and file size
Decode hidden data bit by bit
Store recovered data into output file


Applications
Secure Communication
Digital Watermarking
Data Hiding
Cybersecurity Projects
Information Protection
