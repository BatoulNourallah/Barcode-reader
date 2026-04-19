# Smart Barcode & QR Code Scanner with Nutritional Analysis

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.x-blue" />
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-green" />
  <img src="https://img.shields.io/badge/Platform-Google%20Colab-orange" />
  <img src="https://img.shields.io/badge/API-Open%20Food%20Facts-lightgrey" />
  <img src="https://img.shields.io/badge/License-MIT-black" />
</p>

---

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [System Architecture](#system-architecture)
- [Technologies Used](#technologies-used)
- [Data Source](#data-source)
- [Project Structure](#project-structure)
- [Setup](#setup)
- [Usage](#usage)
- [Example Output](#example-output)
- [Visual Demonstration](#visual-demonstration)
- [Team Members](#team-members)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## Overview
This project implements a real-time barcode and QR code scanner using computer vision techniques in Python within a Google Colab environment.

The system detects and decodes barcodes and QR codes using OpenCV and Pyzbar, and extends functionality by integrating with the Open Food Facts API. When a food product barcode is scanned, the system retrieves and displays detailed product information, including nutritional values and ingredients.

---

## Features
- Hybrid decoding of QR codes and barcodes (EAN-13, UPC)  
- Real-time webcam-based scanning in Google Colab  
- Integration with Open Food Facts API for live product data  
- Grayscale image preprocessing for improved detection accuracy  
- Automatic display of product metadata and nutritional information  

---

## System Architecture
<img width="500" height="750" alt="mermaid-diagram" src="https://github.com/user-attachments/assets/71fc1485-4437-4cab-a0a5-7133f69c01ce" />

---

## Technologies Used
- Python 3.x  
- OpenCV (cv2)  
- Pyzbar  
- Requests  
- NumPy  
- Matplotlib  
- Google Colab  

---

## Data Source
This project uses a live API instead of a static dataset.

- **Source:** Open Food Facts  
- **Method:** REST API (HTTP GET)  
- **Data Retrieved:**
  - Product name  
  - Brand  
  - Ingredients  
  - Nutritional values  
  - Product images  

---

## Project Structure
<img width="450" height="550" alt="mermaid-diagram (1)" src="https://github.com/user-attachments/assets/e4430664-5915-4885-a62d-69014d838502" />

---

## Setup

### Run in Google Colab
Open the notebook and run the following installation commands:

```bash
!pip install pyzbar
!apt-get install -y libzbar0
```

---

## Usage
1. Run the setup cell  
2. Execute the main scanning code  
3. Allow webcam access  
4. Capture an image containing:
   - A QR code → decoded content will be shown  
   - A product barcode → product details will be retrieved  

---

## Example Output

### QR Code Detection
```
Decoded Data: https://example.com
```

### Barcode Detection
```
Product Name: Coca-Cola
Brand: Coca-Cola Company

Nutritional Values (per 100g):
Energy: 42 kcal
Fat: 0 g
Carbohydrates: 10.6 g
Proteins: 0 g
```

---

## Visual Demonstration

### Scanner Interface  
(Add screenshot here)

### Example Output  
(Add screenshot here)

> Note: Add screenshots to the `assets/` folder for proper rendering.

---

## Team Members

| Name | ID | Contribution |
|------|----|-------------|
| Arwa Alqassab | 202101531 | Implementation, API integration, repository management |
| Ghala Alshahrani | 202101402 | Abstract and introduction |
| Renad Alnitaifi | 202200262 | Theory and methodology |
| Shahad Alshowaikhat | 202101791 | Results and analysis |
| Batoul Nourallah | 202300946 | Conclusion and future work |

---

## Future Improvements
- Mobile or web-based user interface  
- Offline product database support  
- AI-based food recognition (without barcodes)  
- Personalized dietary tracking  

---

## License
This project is licensed under the MIT License.
