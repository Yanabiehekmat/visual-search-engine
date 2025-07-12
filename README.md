# 🔍 Visual Image Search Engine using CLIP + FAISS + Gradio

This is a final project for the **Advanced Computer Vision Course**, aiming to design and implement an intelligent **Visual Search Engine** using pretrained vision-language models and similarity-based retrieval methods.

> **By:** Sadegh Zarei  
> **File Name:** `COMPUTERVISION_LASTPR_Sadegh_Zarei.ipynb`  
> **Score:** 🏆 8000 points

---

## 📌 What is a Visual Search Engine?

A **visual search engine** allows users to find similar images by simply uploading one. Instead of using text-based queries, it uses **visual features** extracted from the image and finds the most similar images from a database or image folder.

---

## 🎯 Project Goals

- ✅ Image-Based Retrieval using visual similarity
- ✅ Feature extraction with pretrained models: **CLIP (ViT-B/32)**
- ✅ Fast search using **FAISS**
- ✅ Web interface via **Gradio**
- ✅ Deployment-ready, documented, and open-source on GitHub

---

## 🧠 Use Cases

- 🛍️ E-commerce: Find similar products (e.g., Amazon, Pinterest, Basalam)
- 🏥 Medical: Retrieve similar X-ray/MRI images for diagnostics
- 🔒 Surveillance: Detect similar faces/objects in video feeds
- 🎨 Design: Find visually similar art, sketches, or parts

---

## ⚙️ Technologies Used

| Component        | Tool/Library     |
|------------------|------------------|
| Feature Extractor| OpenAI **CLIP** (ViT-B/32) |
| Search Index     | **FAISS** (Facebook AI)   |
| UI               | **Gradio** Web App        |
| Data Format      | Local folder of images    |
| Language         | Python (Jupyter Notebook) |

---

## 🧪 Demo

🔗 [Live Gradio Demo (expires in 7 days)](https://c0666a8fc1f1196ff8.gradio.live)

<img src="https://i.imgur.com/0r6PRzP.png" width="500">

---

## 📁 Folder Structure

```

project/
│
├── dataset\_images/           # Image database (local)
│   ├── image\_0.jpg
│   ├── ...
│
├── COMPUTERVISION\_LASTPR\_Sadegh\_Zarei.ipynb  # Main code
├── README.md

````

---

## 🚀 How to Run (Step by Step)

1. ✅ Clone the repo or upload `.ipynb` to Colab
2. 📦 Install required libraries:
```bash
pip install torch torchvision faiss-cpu gradio ftfy regex tqdm
````

3. 📥 The code automatically downloads 4 sample images
4. 🤖 CLIP model loads and extracts features
5. 🔍 FAISS index is built for fast similarity search
6. 🖼️ Upload any image and see similar results via Gradio interface

---

## 🧠 How It Works

* **CLIP** converts each image to a high-dimensional feature vector (512-D)
* **FAISS** performs fast similarity search over these vectors using L2 distance
* **Gradio** provides a simple interface to upload image and see top-4 similar results with similarity scores

---

## 🤖 Model Used

* [CLIP: Contrastive Language-Image Pre-training](https://openai.com/research/clip)
* Variant: `ViT-B/32` from OpenAI (via `clip` PyTorch package)

---

## 💡 Example Result

**Query Image:** A cat
**Returned:** 4 most visually similar animals with similarity scores.

---

## ❓ FAQ

**Q:** Can I use my own dataset?
**A:** Yes. Replace images in `dataset_images/` folder with your own.

**Q:** Can I deploy this on HuggingFace Spaces?
**A:** Yes. Add `gradio deploy` and push the repo to HuggingFace.

**Q:** Is this usable offline?
**A:** Yes, after downloading the model and sample images.

---

## 📜 License

This project is for educational purposes. Open-source libraries are used under their respective licenses.

---

## ✨ Credits

* Developed by **Sadegh Zarei** as final project for **Advanced Computer Vision**
* Inspired by OpenAI CLIP and Facebook FAISS
* Course Instructor: \[Instructor Name Here]

---

## 📎 References

* [CLIP Paper](https://arxiv.org/abs/2103.00020)
* [FAISS GitHub](https://github.com/facebookresearch/faiss)
* [Gradio Docs](https://gradio.app)
* [Basalam Visual Search](https://basalam.com/blog/image-search)

```
