# 🗜️ Huffman Compression & Decompression Tool

A simple file compression and decompression utility using **Huffman Coding** in C++.  
This project demonstrates lossless compression where text files become smaller using variable-length coding based on character frequency.

---

## 🚀 Features

- Compress any ASCII file into a compact `.huf` file
- Decompress `.huf` files back to the original content
- Command-line interface for quick usage
- Encodes Huffman tree and meta-data within the output file
- Works efficiently for large and small text files

---

## 🗂️ Project Structure

| File              | Purpose                                      |
|-------------------|----------------------------------------------|
| huffman.hpp       | Header file: classes and function declarations |
| huffman.cpp       | Huffman function implementations               |
| compress.cpp      | Main file for compression                      |
| decompress.cpp    | Main file for decompression                    |
| input.txt         | Example input file (user-provided)             |
| compressed.huf    | Generated Huffman encoded file                 |
| output.txt        | Decoded file after decompression               |

---

## 📦 Tech Stack

- **Language**: C++ (C++11 or newer)
- **Compiler**: g++
- **File I/O**: Standard C++ streams (fstream)
- **Data Structures**: Priority Queue, Binary Trees

---

## ⚡ How to Run Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/sohamsanap07/ByteShrink.git
   cd ByteShrink
2. **Compile the source files:**
    ```bash
    g++ compress.cpp huffman.cpp -o compress

    g++ decompress.cpp huffman.cpp -o decompress
3. **Compress an input file:**
    ```bash
    ./compress input.txt compressed.huf
4. **Decompress the compressed file:**
    ```bash
    ./decompress compressed.huf output.txt
5. **Verify integrity:**
    ```bash
    diff input.txt output.txt
->No output means Files are identical


---

## 📝 Example Usage

**Compile**
    ```bash

    g++ compress.cpp huffman.cpp -o compress

    g++ decompress.cpp huffman.cpp -o decompress

**Compress file**

    ./compress input.txt compressed.huf

**Decompress file**

    ./decompress compressed.huf output.txt

**Check if decompressed file matches original**

    diff input.txt output.txt


---

## 🗒️ Notes

- Input files should be ASCII text for best results.
- Compressed files (`.huf`) include the codebook so decompression needs no external data.
- The project uses binary file read/write for efficient storage.
- Output messages indicate success; compare file sizes and contents to verify.

---

## 🙋 Author

Soham Sanap  
GitHub: sohamsanap07

---
