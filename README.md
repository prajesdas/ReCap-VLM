# ReCap-VLM: Vision-Language Model for Image Captioning and Restoration

ReCap-VLM is a deep learning project integrating **image captioning** and **image restoration** through modern **vision-language models (VLMs)**. It leverages pretrained architectures like **InceptionV3**, **CLIP**, and **Transformer-based decoders** to generate high-quality captions from images while enhancing degraded visuals before captioning.  

---

##  Features
- Automatic image caption generation using attention-based encoder-decoder architecture  
- Image restoration (denoising, deblurring, enhancement) before caption generation  
- Utilizes pretrained CNN and Transformer layers for robust multimodal learning  
- Supports **MS COCO**, **Flickr8k**, and custom datasets  
- Modular and extensible structure for research and real-world applications  

---

##  Model Architecture
The architecture includes:
1. **Encoder (InceptionV3 / ResNet)** for feature extraction  
2. **Attention Mechanism** for spatial focus  
3. **LSTM/GRU Decoder** for sequence generation  
4. **Vision-Language Fusion Layer** integrating textual and visual embeddings  
5. Optional **Diffusion/Restoration Module** for image quality improvement  

---

## Workflow

```text
Input Image → Preprocessing → Restoration → Feature Extraction → 
Attention Module → Text Decoder → Generated Caption
````

---

## 🗂 Dataset

* **MS COCO** (Common Objects in Context)
* **Flickr8k / Flickr30k**
* Each image is paired with five human-written captions for linguistic diversity.

---

## Installation

```bash
git clone https://github.com/prajesdas/ReCap-VLM.git
cd ReCap-VLM
pip install -r requirements.txt
```

---

## Usage

```bash
python main.py
```

Upload or load an image, and the model will restore and generate a descriptive caption automatically.

---

## 📊 Results

| Task             | Metric | Score   |
| ---------------- | ------ | ------- |
| Image Captioning | BLEU-4 | 0.247   |
| Restoration      | PSNR   | 33.5 dB |
| Restoration      | SSIM   | 0.92    |

> Results are based on the Flickr8k dataset and benchmark restoration models like MPRNet and SwinIR.

---

## 🧰 Technologies Used

* Python, TensorFlow / PyTorch
* NumPy, OpenCV, Matplotlib
* Pretrained models: InceptionV3, CLIP, SwinIR, MPRNet

---

## 📈 Future Improvements

* Add multilingual caption generation
* Extend restoration for real-time streaming input
* Integrate with diffusion models for enhanced realism

---

## 📚 References

This work builds upon major contributions in multimodal AI, including:

* CLIP (Radford et al., 2021)
* MPRNet (Zamir et al., 2021)
* SwinIR (Liang et al., 2021)
* Res-Captioner (Sun et al., 2023)

---

## 🧑‍💻 Author

**Prajes Das**
Student | AI & Computer Vision Research Enthusiast
GitHub: [prajesdas](https://github.com/prajesdas)

---

## 🪪 License

This project is released under the **MIT License**.

---

⭐ **If you like this project, please star the repo!**

