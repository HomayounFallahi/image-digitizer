## Image Digitizer

**Image Digitizer** is a high-precision, browser-based tool designed to extract numeric data points from images of graphs and plots. This application simplifies the process of converting visual data in research papers, legacy documents, or screenshots back into usable datasets like CSV or JSON.

**Developed by:** [Homayoun Fallahi](https://ir.linkedin.com/in/homayoun-fallahi)

---
## Video Tutorial

[![Watch the tutorial](https://github.com/HomayounFallahi/image-digitizer/blob/main/Tutorial_Image_Digitizer.mp4)


---

## ⚙️ Installation & Usage

### Single-File Application

1. [Download](https://github.com/HomayounFallahi/image-digitizer/releases/download/releases/Image.Digitizer.html) `Image.Digitizer.html` from the from the Releases page.
2. Open the file in any modern web browser (Chrome, Edge, Firefox).
3. No installation, internet connection, or server setup is required.

---

### ✨ Key Features

- **Multi-Scale Support**: Accurately handles Linear, Logarithmic (Log_{10}), Natural Log (ln), and Inverse (1/x) axes.
  
- **4-Point Calibration**: Uses a robust coordinate transformation system based on four user-defined reference points (C1-C4) to ensure spatial accuracy.
  
- **Data Visualization**: Offers a "Line Trace" mode to connect digitized points and visualize trends directly on the image.
  
- **Sorting**: Automatically sort extracted data by click order or by X/Y values (ascending/descending).
  
- **Session Management**: Save your entire workspace (including the image, calibration, and points) to a `.json` file to resume work later.
  
- **Export Options**: One-click export of digitized data to **CSV** or **JSON** formats.
  

---

### 🚀 Getting Started

Since this is a client-side web application, **no installation** is required.

1. **Open the App**: Simply open the html file in any modern web browser.
  
2. **Upload Image**: Drag and drop your graph image (PNG/JPEG) or use the "Upload Image" button.
  
3. **Calibrate**:
  
  - Stay in **Calibration Mode**.
    
  - Click four points on your graph (e.g., origin, axis limits) to set C1, C2, C3, and C4.
    
  - Enter the "Real Values" for these points in the sidebar.
    
  - Select the correct Axis Type for X and Y, then click **Calibrate**.
    
4. **Digitize**:
  
  - Switch to **Digitize Mode**.
    
  - Click on the data series to extract points (P1, P2, etc.).
    
5. **Export**: Review your data in the table and click **Export CSV** or **Export JSON**.
  

---

### 🛠️ Technical Overview

- **Core Logic**: The app uses 3x3 matrix determinants to solve for affine transformation coefficients, mapping pixel coordinates to a linearized coordinate system.
  
- **Privacy**: All processing is done locally in your browser. No image or data is ever uploaded to a server.
