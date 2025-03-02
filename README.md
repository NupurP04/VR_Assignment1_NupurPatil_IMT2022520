
# **VR_Assignment1_NupurPatil_IMT2022520**  
## **Coin Detection and Segmentation**  

### **1. Overview**  
This project performs **coin detection and segmentation** using **image processing techniques** in Python. It detects circular objects (coins), outlines them, and segments them individually for further analysis.  

### **2. Features**  
 **Preprocessing:** Converts the image to grayscale and applies Gaussian blur.  
 **Thresholding:** Uses Adaptive Gaussian Thresholding to enhance coin regions.  
 **Contour Detection:** Extracts external contours of objects in the image.  
 **Coin Filtering:** Filters valid coins based on area and circularity.  
 **Visualization:** Draws circles around detected coins and displays intermediate outputs.  
 **Segmentation:** Isolates each detected coin and removes the background.  

---

### **3. Installation & Dependencies**  
Ensure you have **Python 3.x** installed along with the following dependencies:  
```bash
pip install opencv-python numpy matplotlib
```

---

### **4. How to Run**  
1. Clone the repository:  
```bash
git clone https://github.com/NupurP04/VR_Assignment1_NupurPatil_IMT2022520.git  
cd VR_Assignment1_NupurPatil_IMT2022520
```

2. Inside the input_image directory, coins.jpg is the input_image used in the script, copy the path accordingly.  

3️. Go to the coin_detection_and_segmentation folder - execute the cells in VR_ass1_coin.ipynb. 

---

### **5. Methodology**  
####  Step 1: Image Preprocessing  
- Convert the image to grayscale.  
- Apply **Gaussian Blur** to remove noise.  
- Display intermediate outputs.  

####  Step 2: Thresholding 
- Use **Adaptive Gaussian Thresholding** to highlight coins.  

####  Step 3: Contour Detection 
- Extract contours from the thresholded image.  

####  Step 4: Filtering & Drawing Coins  
- Filter coins based on **area and circularity** constraints.  
- Draw circles around valid coins.  

####  Step 5: Segmentation  
- Apply **region-based segmentation** using contour bounding boxes.  
- Create a mask to remove the background.  

---

### 6. Results & Observations  
- The algorithm successfully detects coins in the image and segments them individually.  
- **Intermediate results** (grayscale, blurred, thresholded, detected, and segmented images) are displayed.  
- The total number of detected coins is printed.  

**Example Output (Visualization)**  
| **Original Image** | **Thresholded Image** | **Detected Coins** |  
|-----------------|-----------------|-----------------|  
| ![Original](coin_detection_and_segmentation/output_images/original_image.png) | ![Thresholded](coin_detection_and_segmentation/output_images/thresholded_image.png) | ![Detected](coin_detection_and_segmentation/output_images/detected_coin_border_image.png) |  

---


