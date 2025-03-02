
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
1️⃣ Clone the repository:  
```bash
git clone https://github.com/NupurP04/VR_Assignment1_NupurPatil_IMT2022520.git  
cd VR_Assignment1_NupurPatil_IMT2022520
```

2️⃣ Place the image file inside the repository folder.  

3️⃣ Run the script:  
```bash
python coin_detection.py
```

---

### **5. Methodology**  
#### **🔹 Step 1: Image Preprocessing**  
- Convert the image to grayscale.  
- Apply **Gaussian Blur** to remove noise.  
- Display intermediate outputs.  

#### **🔹 Step 2: Thresholding**  
- Use **Adaptive Gaussian Thresholding** to highlight coins.  

#### **🔹 Step 3: Contour Detection**  
- Extract contours from the thresholded image.  

#### **🔹 Step 4: Filtering & Drawing Coins**  
- Filter coins based on **area and circularity** constraints.  
- Draw circles around valid coins.  

#### **🔹 Step 5: Segmentation**  
- Apply **region-based segmentation** using contour bounding boxes.  
- Create a mask to remove the background.  

---

### **6. Results & Observations**  
- The algorithm successfully detects coins in the image and segments them individually.  
- **Intermediate results** (grayscale, blurred, thresholded, detected, and segmented images) are displayed.  
- The total number of detected coins is printed.  

📌 **Example Output (Visualization)**  
| **Original Image** | **Thresholded Image** | **Detected Coins** |  
|-----------------|-----------------|-----------------|  
| ![Original](outputs/original.jpg) | ![Thresholded](outputs/thresholded.jpg) | ![Detected](outputs/detected.jpg) |  

📌 **Segmented Coins:**  
![Segmented](outputs/segmented.jpg)  

---

### **7. Repository Structure**  
```
VR_Assignment1_[YourName]_[YourRollNo]/
│── coin_detection.py          # Main Python script  
│── README.md                  # Project documentation  
│── /images                    # Folder containing input images  
│── /outputs                   # Folder containing result images  
```

