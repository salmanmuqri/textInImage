# TextInImage

**TextInImage** is a web-based tool that allows users to hide and extract text within an image using steganography techniques. It provides two main functionalities:

1. **Encoding**: Users can encode a secret message into an image and download the modified image with the hidden text.
2. **Decoding**: Users can upload an encoded image to extract the hidden message.

---

## Features

- Encode text into an image with minimal distortion.
- Decode hidden messages from encoded images.
- User-friendly interface with live previews for encoding images.
- Support for PNG format for encoded images.

---

## Demo

You can try out the tool by accessing the hosted version of **TextInImage**. Simply visit the live demo link (if provided), or you can set it up locally.

---

## Installation

To run **TextInImage** locally, follow these steps:

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- No server-side dependencies are needed (it's a client-side web app)

### Steps

1. **Download the repository**:
   - Clone or download the repository to your local machine.

   ```bash
   git clone https://github.com/salmanmuqri/textInImage.git
   ```

2. **Open the project**:
   - Open the `index.html` file directly in a web browser.

3. **Start using**:
   - Once the file is opened in your browser, you can immediately begin encoding or decoding images.

---

## Usage

### Encode Text into Image

1. Go to the **Encode** tab.
2. Select an image to encode by clicking on the **Select Image** button.
3. Enter the text you want to hide inside the **Text to Hide** text area.
4. Click the **Encode and Download** button.
   - The image will be encoded with the hidden message and automatically downloaded in PNG format.

### Decode Text from Encoded Image

1. Go to the **Decode** tab.
2. Select an encoded image by clicking on the **Select Encoded Image** button.
3. Click the **Decode** button.
   - The hidden message will be displayed below.

---

## How It Works

1. **Encoding**: 
   - The input text is converted into binary.
   - The binary message is embedded into the image's pixel data (least significant bit of each color channel).
   - The image is saved with the hidden message, which can later be decoded.

2. **Decoding**: 
   - The uploaded image is analyzed pixel-by-pixel.
   - The least significant bits of each color channel are extracted to reconstruct the binary message.
   - The binary is then converted back to text and displayed.

---

## Technologies Used

- HTML
- CSS
- JavaScript
- Canvas API (for image manipulation)
- FileReader API (for handling image files)

---
# Ai help was taken in this project (for readme file..)