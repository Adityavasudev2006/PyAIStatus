![Logo](pictures/logo.png)

# 🚀 PyAIStatus

PyAIStatus is a **cutting-edge evaluation and reporting library** designed to streamline the complete lifecycle of model assessment in **machine learning competitions, research, and enterprise deployments**.

Built with **clarity**, **reproducibility**, and **rigor** in mind, PyAIStatus transforms the typically fragmented evaluation process into a **single-command solution** that delivers a comprehensive interactive report (`report.html`) 📊 packed with actionable insights.

## Visit : https://lovable.dev/projects/b36b7437-4fd6-47da-8422-cd90c3a80412

## ✨ Key Highlights

- ✅ **Plug-and-Play Evaluation** – Run the entire evaluation pipeline with one function call.
- 🔁 **Reproducibility First** – Captures environment details, seeds, and library versions for exact replication.
- 📈 **Rich Analytics** – Generates all required KPIs _(Accuracy, F1, ROC AUC, PR AUC, Calibration, Brier score, etc.)_ with confidence intervals.
- 🎨 **Visual Explanations** – Produces confusion matrices, ROC/PR curves, calibration plots, robustness degradation charts, and explainability heatmaps _(Grad-CAM, Integrated Gradients)._
- 🛡 **Robustness & Reliability** – Evaluates models under Gaussian noise, blur, occlusion, and compression to assess real-world resilience.
- 📊 **Statistical Rigor** – Performs baseline comparisons, bootstrapped confidence intervals, and significance testing.
- ⚡ **Efficiency Insights** – Reports model size, parameter count, inference time, and memory usage for deployment readiness.
- 📑 **Automated Reporting** – Delivers a polished, self-contained **HTML report** for stakeholders to review instantly—no extra steps required.

---

## 📦 Installation

1.Clone the Repo to local system  
2.Type the following commands to run the library: 
 -pip install -e .  
 -python scripts/evaluate_model.py "./models/model_name.h5" "./data/dataset_name/train" "./evaluation_results" 

```bash
  pip install -e .
  python scripts/evaluate_model.py models/Dogs-vs-Cats_model.h5 data/cats_and_dogs_dataset/train evaluation_results
```

## 📝 Requirements

-tensorflow>=2.9,<2.10

-scikit-learn

-pandas

-matplotlib

-seaborn

-numpy<2.0

-opencv-python-headless

-tqdm

-tf-keras-vis

## 🚀 Usage - Quick Run (.py file/.ipynb file)

1.Open the code file where you wanna use the PyAIStatus
2.Import the PyAIStatus library and use the functions in the code (.py or .ipynb)
3.Example:

```bash
import os
from PyAIStatus import evaluate

#Defining Location
model_location = os.path.join("models", "Dogs-vs-Cats_model.h5")
data_location = os.path.join("data", "cats_and_dogs_dataset", "train")
output_location = os.path.join("evaluation_results")

#Calling the evaluate function
if not os.path.exists(model_location):
    print(f"Error: Model file not found at '{model_location}'")
elif not os.path.exists(data_location):
    print(f"Error: Dataset directory not found at '{data_location}'")
else:
    evaluate(
        model_path=model_location,
        dataset_dir=data_location,
        output_dir=output_location
    )
```

## 🚀 Demo Pictures

<p align="center">
  <img src="pictures/report_pic_1.png" alt="Report Picture 1" width="45%">
  <img src="pictures/website_pic_1.png" alt="Website Picture 1" width="45%">
</p>

<p align="center">
  <img src="pictures/website_pic_2.png" alt="Website Picture 2" width="45%">
  <img src="pictures/report_pic_2.png" alt="Report Picture 2" width="45%">
</p>

<p align="center">
  <img src="pictures/report_pic_3.png" alt="Report Picture 3" width="45%">
  <img src="pictures/report_pic_4.png" alt="Report Picture 4" width="45%">
</p>

## ✨ Project Contributors  

👨‍💻 **Library Creator:** Aditya Vasudev K  
🌐 **Website Creators:** Ananya Vinay, Anusriya Sreedhar, and Shreya Mahajan  
🔬 **Research:** Sai Satya Pranav  

---

## 📜 License

[MIT](https://choosealicense.com/licenses/mit/)

## 🏷️ Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
