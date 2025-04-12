# Particle Shape Classification using ML-Based Techniques

This project, part of the **Mineral Processing and Plant Design Course**, aims to classify particle shapes using **Machine Learning (ML)**. The dataset used is the **NASA 2DS Probe's cloud particle dataset**, which closely resembles mineral particles in structure.

### Team Members
- **Kumar Snehal** (22CS02009)
- **Aditya Dhananjay Singh** (22CS02001)
- **Atharva Atul Penkar** (22CS02011)
- **Harshil Singh** (22CS01015)
- **Monjit Das** (22EE01059)

### Project Objective
Develop an unsupervised ML pipeline to classify particles based on shape using **K-Means clustering** and **Vision Transformer (ViT)**. This method has potential applications in mineral processing, including optimization in ball mills.

### Methodology
1. **Image Extraction**: Blue mask is applied to detect particles and extract valid contours.
2. **Preprocessing**: Images are padded, resized, converted to grayscale, and sharpened.
3. **ViT Preprocessing**: Images are resized to 224x224, normalized to [-1, 1], and passed to ViT.
4. **K-Means Clustering**: Particles are grouped based on shape, yielding 7 distinct clusters.

### Clusters Identified
- **Linear**
- **Aggregate**
- **Graupel**
- **Dendrite**
- **Irregular**
- **Plate**
- **Spherical**

### Evaluation Metrics
- **Silhouette Score**: 0.4309 (measure of cluster separation)
- **Davies-Bouldin Index**: 0.8073 (lower is better)
- **Calinski-Harabasz Score**: 29,874.83 (higher is better)

### Technologies Used
- **Machine Learning**: K-Means Clustering
- **Deep Learning**: Vision Transformer (ViT)
- **Libraries**: `numpy`, `pandas`, `torch`, `timm`, `torchvision`, `PIL`, `sklearn`, `cv2`, `umap`, `matplotlib`, `tqdm`

### Conclusion
This project demonstrates the application of **ML** and **ViT** for particle classification. The pipeline can be adapted for mineral processing applications, improving particle classification for operations like grinding and separation.

---
