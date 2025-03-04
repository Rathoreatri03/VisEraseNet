# **VisEraseNet: AI-Powered Object & Logo Removal** 🚀  

**VisEraseNet** is an advanced AI framework designed for **automatic logo and textual data  removal** from videos and images. It combines **YOLO-based detection, segmentation models, and inpainting techniques** to erase unwanted elements seamlessly while preserving visual integrity.  

---

## **🔹 Features**  
✅ **Video Input Object & Text Detection** using **YOLOv5/YOLOv8**  
✅ **Segmentation-Based Masking** using **Detectron2/Custom Models**  
✅ **Advanced Inpainting** for seamless object removal  
✅ **Frame-by-Frame Video Processing** with automatic mask generation  
✅ **Customizable Confidence & Masking Thresholds**  
✅ **Supports Image & Video Processing** (Batch & Live processing)  
✅ **Fast & Efficient** with optimizations for real-time applications  

---

## **📂 Models & Releases**  
All pre-trained models, including **YOLO models for logo/text detection** and **segmentation models**, are available in the **[Releases Tab](https://github.com/Rathoreatri03/VisEraseNet/releases)**.  

---

## **⚙️ How It Works**  

### **🔸 1. Object & Logo Detection (YOLOv5/YOLOv8)**
- Uses **YOLO-based models** to detect **logos, text, and objects** in images and videos.  
- Extracts bounding boxes (`bbox`) for detected objects.  

### **🔸 2. Segmentation Mask Generation (Detectron2)**
- Runs segmentation models to create a precise **mask** for detected objects.  
- Merges bounding boxes and segmentation masks into a **final mask**.  

### **🔸 3. Mask Refinement & Merging**
- Refines segmentation masks and ensures objects are **accurately removed**.  
- Merges **logo, text, and segmentation masks** into a single **final mask** for inpainting.  

### **🔸 4. Inpainting (Object Removal)**
- The **final mask** is used to **remove unwanted objects** using **AI-based inpainting**.  
- Ensures seamless reconstruction of the background.  

### **🔸 5. Video Processing**
- Processes videos **frame-by-frame** to detect, mask, and remove objects.  
- Generates an **inpainted video** with objects seamlessly erased.  

---

## **📥 Installation & Setup**  

### **🔹 Step 1: Clone the Repository**
```bash
git clone https://github.com/Rathoreatri03/VisEraseNet.git
cd VisEraseNet
```

### **🔹 Step 2: Install Dependencies**
```bash
pip install -r requirements.txt
```

### **🔹 Step 3: Download Pretrained Models**
- Go to the **[Releases Tab](https://github.com/Rathoreatri03/VisEraseNet/releases)** and download the models.  
- Place them inside the `models/` directory.  

---

## **🚀 Usage**  

### **🔹 Run on an Image**
```bash
python process_image.py --input example.jpg --output output_folder/
```

### **🔹 Run on a Video**
```bash
python process_video.py --input input_video.mp4 --output output_video.mp4
```

---

## **📜 Research & Development**  
This project is built using **state-of-the-art AI models** and **deep learning techniques**. It is designed to improve **automated content moderation, digital content enhancement, and forensic image reconstruction**.  

🔗 **[Paper (Coming Soon)]**  
📌 **Contributors:** [Atri Rathore]  
📢 **Contact:** [GitHub Issues / Email]  

---

## **🎯 Future Improvements**  
✅ **Optimize Inpainting** for better background reconstruction  
✅ **Speed Optimizations** using **TensorRT / ONNX**  
✅ **Dataset Expansion** for better generalization across logos & text  
✅ **Web API Deployment** for easy integration into real-world applications  

---

### **🚀 Ready to make unwanted objects disappear? Give it a try!** 🔥  
