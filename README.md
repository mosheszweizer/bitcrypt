# bitcrypt
Encryption that hides text in pictures 

Bitcrypt is easy to use. There are only two objectives. The first is to put some text into a picture. The second is to retrieve it. Thus, to operate the program, one needs a picture, some text to be encoded, and an encryption key. The steps are as follows:

To encrypt:
1) Select a bitmap image (it must be either 24 or 32 bits deep)
2) Either upload from a file or type into the editor some text you wish to hide in the image
3) Type an encryption key you wish to use (it needs to be at least eight characters long)
4) Press the encrypt button

The program takes your text and processes it with the Rijndael cipher. The outcome of this process is shown in the editor. The thus encrypted text is 'written' into the picture you have selected. At the completion of the process, a popup message asks you to save the encrypted image, which you need to do as a last step.

To decrypt:
1) Select an encrypted image
2) Type the encryption key
3) Press the decrypt button
The decrypted text is shown in the editor. You can export it if you wish using the provided button.

Notes:
a) The image must be a bitmap. If you have a different format, you can use any image editor (for example, GIMP) to convert it/export it to this format. 
b) The key may be any combination of ASCII characters. That is, the program should be able to accept anything that you can type on the keyboard
c) The Rijndael cipher enlarges text. Therefore, you may need a larger image to accommodate this. If the image is too small, a popup message tells you by how much. You may take this into account when selecting a larger picture.

BitCrypt is written in Pascal and the file stored here was compiled on an AMD® Ryzen processor running Ubuntu 20.04.5 LTS.
You can download the file and test if it runs on your Linux installation.

INSTALL
Bitcrypt has been compiled with FPC compiler which staticly links all dependancies. Therefore one should not need to import any additional components to run bitcrypt. 

To install, 
Download the compressed bitcrypt-install file from this directory and decompress it.
Examine install.sh file to see the intended installation destinations. Then run
sudo ./install.sh

