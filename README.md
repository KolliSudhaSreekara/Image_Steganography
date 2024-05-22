# Image Steganography Application
## Overview
This project is an Image Steganography application that allows users to hide a secret message within an image and later retrieve the message using a password. It uses Tkinter for the graphical user interface (GUI) and OpenCV for image processing.

## Features
Encrypt a Message: Hide a secret message within an image.
Decrypt a Message: Retrieve the hidden message from an image using a password.
User-Friendly Interface: Easy-to-use GUI for both encryption and decryption processes.

## Requirements
1. Python 3.x
2. Tkinter
3. OpenCV
4. Numpy

## Installation
Install Python 3.x from the official website.
## Install the required libraries using pip:
      pip install opencv-python numpy
      
## How to Use
#Encrypt a Message:
1. Enter the path of the image file.
2. Enter the secret message you want to hide.
3. Enter a password for encryption.
4. Click the "Encrypt" button.
The application will save the encrypted image as Encryptedimg.jpeg and display it.

## Decrypt a Message:
1. Enter the password used during encryption.
2. Click the "Decrypt" button.
The application will display the hidden message if the correct password is provided.

## Code Explanation
The code is divided into several parts:

# Imports and Initialization:
Import necessary libraries: Tkinter, OpenCV, messagebox, and string.
Initialize the main window and global variables.

## Dictionaries for ASCII Conversions:
Create dictionaries for character-to-integer and integer-to-character conversions.

## Load Image:
Load an image to display in the GUI.

## Encrypt Function:
Get inputs from the user (image path, message, password).
Read the image and hide the message within the least significant bits (LSBs) of the image pixels.
Save and display the encrypted image.

## Decrypt Function:
Get the password from the user.
Check if the entered password matches the encryption password.
Retrieve the hidden message from the LSBs of the image pixels and display it.

## Clear Fields Function:
Clear the input fields after encryption.

## GUI Components:
Create labels, entry widgets, and buttons for user inputs and actions.
Pack the components in the window.

## Start the Tkinter Event Loop:
Start the Tkinter event loop to run the application.

## Example
Here is an example of how to use the application:

## Run the application:
    python image_steganography.py
In the GUI, enter the path to the image you want to use (e.g., image.png).

Enter the secret message you want to hide (e.g., Hello, World!).

Enter a password for encryption (e.g., mypassword).

Click the "Encrypt" button to hide the message in the image.

To retrieve the message, enter the password used during encryption and click the "Decrypt" button.

## Notes
Ensure that the image file path is correct.
The application currently supports only ASCII characters for the secret message.

## Acknowledgements
The Tkinter library for the GUI.
The OpenCV library for image processing.
