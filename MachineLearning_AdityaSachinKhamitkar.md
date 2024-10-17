## Aditya Sachin Khamitkar
`22MIP10006`
#### GDGC 2024
Here are the short versions of my two projects. Most of them taken directly from the README.md of the repository.
---

# 🌾 **AgriSatAI**: Revolutionizing Agriculture with AI and Satellite Data

[![Repo Visits](https://badges.pufler.dev/visits/TechieSamosa/AgriSatAI)](https://github.com/TechieSamosa/AgriSatAI)
[![GitHub Stars](https://img.shields.io/github/stars/TechieSamosa/AgriSatAI?style=social)](https://github.com/TechieSamosa/AgriSatAI/stargazers)
[![Forks](https://img.shields.io/github/forks/TechieSamosa/AgriSatAI?style=social)](https://github.com/TechieSamosa/AgriSatAI/network/members)

## 🚀 **Project Overview**

AgriSatAI is an innovative project aimed at transforming agriculture by utilizing AI and real-time satellite data provided by ISRO’s NRSC. By combining machine learning algorithms with satellite imagery, AgriSatAI tackles critical challenges in agriculture, such as water optimization, crop health monitoring, and yield prediction. It provides farmers and stakeholders with actionable insights to promote sustainable farming.

---

### 🧠 **Problem Solving & ML Applications**

- **Water Optimization**: AgriSatAI uses real-time environmental data, such as soil moisture and weather conditions, to recommend irrigation schedules. Machine learning models predict water needs, reducing wastage and enhancing resource use efficiency.
- **Crop Health Monitoring**: By analyzing vegetation indices (like NDVI), the project detects potential crop health issues and provides recommendations for timely interventions.
- **Yield Prediction**: Historical and real-time data are fed into ML algorithms to forecast crop yields. This helps in resource management, better planning, and increased productivity.

In AgriSatAI, machine learning is used to analyze satellite imagery and environmental data to monitor crop health, optimize water usage, and predict crop yields. The project integrates various AI models to process vegetation indices such as the Normalized Difference Vegetation Index (NDVI), which helps in detecting crop stress early by analyzing patterns in satellite images. Machine learning algorithms then generate insights about crop health, irrigation needs, and forecast yields based on historical and real-time data. The models adaptively learn from weather patterns, soil moisture levels, and crop growth stages to recommend precise interventions, ensuring sustainable water use and maximizing crop productivity. By automating these tasks, the system helps farmers make data-driven decisions that improve resource efficiency and agricultural outcomes.

---

### 💻 **How to Integrate AgriSatAI Into a Web Project**

To help a web developer integrate the AgriSatAI model into a web application:

1. **Backend Integration (Flask/Django)**:
   - Develop a REST API using Flask or Django to interact with the trained ML models. 
   - For example, the `/predict` endpoint can accept POST requests with data (such as satellite imagery or environmental metrics) and return irrigation schedules, health reports, or yield predictions as responses.
   - Use `data_processing.py` for input preprocessing, and call the trained models from `model_training.py`.


2. **Frontend Integration**:
   - Design an interactive dashboard that visualizes the insights from the API. Technologies like React.js or Angular.js can be used to build an intuitive UI for farmers.
   - Use Mapbox or Google Maps API to display real-time satellite imagery, overlaying it with information on crop health, water optimization areas, and predicted yields.



---

## 🏗️ **Current Status**

This repository is currently private due to ongoing work and approval processes with ISRO NRSC. It will be made public once all necessary permissions are obtained.

---

# 🌕 **LunaVision-PSR-ImageLab**: Enhancing Lunar Exploration with GANs and Retinex Theory

![Project Status](https://img.shields.io/badge/Project%20Status-Active-brightgreen) ![Hackathon](https://img.shields.io/badge/Smart%20India%20Hackathon-2024-ff69b4)

## 🚀 **Project Overview**

**LunaVision-PSR-ImageLab** is a cutting-edge solution for improving low-light images captured from the **Permanently Shadowed Regions (PSRs)** of the lunar surface. The project employs **Generative Adversarial Networks (GANs)** combined with **Retinex Theory** to enhance the visibility and clarity of these images, aiding lunar exploration and landing site selection.

---

### 🧠 **Problem Solving & ML Applications**

- **Low-Light Image Enhancement**: GAN models are trained to enhance extremely low-light images, producing high-resolution outputs that reveal surface features previously hidden in shadow.
- **Retinex Theory**: This theory simulates human vision under low-light conditions, allowing us to balance the color and light of lunar images for better perceptual quality.
- **Applications**: The generated PSR image maps are crucial for selecting safe landing sites, conducting geomorphological studies, and assisting future lunar missions.

In LunaVision-PSR-ImageLab, machine learning is applied to enhance low-light images captured from the Permanently Shadowed Regions (PSR) of the Moon. The project utilizes Generative Adversarial Networks (GANs), a cutting-edge machine learning technique designed to generate high-quality images from noisy or incomplete data. GANs are particularly effective in this scenario, where raw images from lunar craters contain minimal light and substantial noise. The AI model is trained on large datasets of lunar images to reconstruct and enhance the faint details from the shadowed regions, enabling clearer visualization of the lunar surface. Additionally, Retinex Theory is applied alongside these machine learning models to simulate human visual perception in low-light conditions, balancing light and color for a more natural representation. This innovative combination of machine learning and domain-specific techniques not only improves image clarity but also provides valuable data for lunar mission planning, such as selecting potential landing sites and conducting geomorphological studies.

---

### 💻 **How to Integrate LunaVision-PSR-ImageLab Into a Web Project**

To help a web developer integrate the LunaVision model into a web application:

1. **Backend Integration (Flask/Django)**:
   - Create a REST API that handles requests for image enhancement using the GAN model. Developers can upload raw lunar images, and the API will return enhanced versions.
   - Implement image preprocessing and postprocessing within the backend using OpenCV and the trained GAN model from `model_training.py`.


2. **Frontend Integration**:
   - Use a frontend framework (React.js/Angular.js) to build an intuitive interface where users can upload lunar images for enhancement and view the resulting PSR maps.
   - Display the enhanced images alongside original low-light versions for comparison, using a slider or before/after interface.
   

---

## 🏗️ **Current Status**

This repository is currently private due to ongoing development and ISRO NRSC’s approval processes. It will be made public as soon as the work is complete and official permissions are granted.

---

## 🤝 **Contributing**

If you are a web developer or machine learning enthusiast, your contributions to improving these models and building user-friendly interfaces are welcome. Follow the steps in each repository’s `CONTRIBUTING.md` for details on how to get involved.

---
Both projects demonstrate how machine learning can be adapted to solve real-world challenges by extracting actionable insights from large-scale data, improving decision-making, and advancing technological innovation in their respective fields.


---
Both repositories are private for now and will be made public soon as I will be receiving clearance from ISRO NRSC. Thank you for your understanding! Let's work together to bring these innovative solutions to life.