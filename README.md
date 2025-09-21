# Multimodal LLMs for Phishing Detection: A Comprehensive Benchmark

This repository contains the Google Colab notebooks used in our research on evaluating the performance of open-source multimodal Large Language Models (LLMs) in detecting phishing websites. The notebooks are publicly available to allow for the reproduction of our experiments and to serve as a resource for the cybersecurity community.

To use the notebooks, you must **download the file** from this repository and then **upload it to your Google Drive** to open it with Google Colab.

---

### 💻 Getting Started

Before running the notebooks, you need to download the dataset and place it in your Google Drive.

To run the notebooks, please follow these steps:

1.  **Download the Dataset**: The required dataset is hosted on Hugging Face. You can download it from the following link: [https://huggingface.co/datasets/seirin16/Dataset_Phising](https://huggingface.co/datasets/seirin16/Dataset_Phising).
2.  **Upload to Google Drive**: Once downloaded, upload the dataset to your Google Drive. The notebooks are configured to access the data from there.
3.  **Run the Notebooks**: Download the desired notebook (.ipynb file) from this repository and upload it to your Google Drive to open it with Google Colab.

---

### 📂 Repository Contents

The repository includes five distinct notebooks, each designed to test a specific input modality or a unique model configuration:

* **Multimodales_Pipeline.ipynb**: This notebook is designed for a full multimodal analysis. It processes the URL, HTML content, and a screenshot of a website to determine if it is a phishing threat. This notebook includes all models from the benchmark, but the `phi3.5` model will encounter an error due to its specific `chat_template` requirements.

* **Multimodales_Pipeline_HTML.ipynb**: This notebook focuses on HTML-only analysis. It processes only the HTML content of a website.

* **Multimodales_Pipeline_SCREENSHOT.ipynb**: This notebook focuses on image-only analysis. It processes only a screenshot of the website.

* **Multimodales_Pipeline_URL.ipynb**: This notebook focuses on URL-only analysis. It processes only the URL of the website.

* **Phi3.5.ipynb**: This notebook is exclusive to the `phi3.5` model. It is designed to work with the model's unique `chat_template`, which is different from the other models included in the pipeline notebooks.

---

### ⚠️ Important Note on Model Execution

Each `Multimodales_Pipeline_*.ipynb` notebook is pre-configured to run all models from the benchmark. However, please be aware that the `phi3.5` model will fail in these notebooks due to its unique `chat_template`. If you want to use the `phi3.5` model, you must use the dedicated **Phi3.5.ipynb** notebook, which is specifically tailored for it.
