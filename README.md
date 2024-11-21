Here's the updated README file with a mention of the three basic filters (Median, Gaussian, Box) added to the Features section:

---

# **Image Filtering and Noise Removal Using Adaptive Filters and Bilateral Filter**

This project demonstrates the implementation of various image filtering techniques for noise removal, including **adaptive median filtering**, **adaptive mean filtering**, and **bilateral filtering**. In addition to these, the project also includes the application of three basic filters: **Median**, **Gaussian**, and **Box filters**. The filters are evaluated based on their effectiveness in removing noise while preserving image quality, with performance metrics like **Mean Squared Error (MSE)** and **Signal-to-Quantization-Noise Ratio (SQNR)**.

### **Table of Contents**
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## **Introduction**

In this project, we explore the impact of different noise types (such as **salt-and-pepper** and **Gaussian noise**) on images, and we apply various image filters to mitigate the effects of these noise types. The project includes the implementation of the **bilateral filter**, **adaptive median filter**, **adaptive mean filter**, as well as the **basic filters**: **Median**, **Gaussian**, and **Box filters**. By calculating the **MSE** and **SQNR**, we analyze how effectively these filters preserve the image quality while removing the noise.

---

## **Features**

- **Noise Types**: Salt-and-pepper noise, Gaussian noise.
- **Image Filters**: 
  - **Basic Filters**: Median Filter, Gaussian Filter, Box Filter.
  - **Advanced Filters**: Adaptive Median Filter, Adaptive Mean Filter, Bilateral Filter.
- **Metrics**: MSE (Mean Squared Error), SQNR (Signal-to-Quantization-Noise Ratio) for evaluating filter effectiveness.
- **Performance Evaluation**: Comparison of filter run times and quality metrics (MSE, SQNR).
- **Image Visualizations**: Interactive visualizations of noisy images, filtered images, and performance metrics.

---

## **Requirements**

The following libraries are required to run the code:

- **Python 3.x**
- **NumPy**
- **OpenCV**
- **Matplotlib**
- **Numba** (for accelerated filtering)
- **scikit-image** (optional, for additional image processing tools)

You can install the required libraries using the provided `requirements.txt` file.

---

## **Installation**

### **Clone the Repository**
To get started, clone this repository to your local machine:

```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
```

### **Install Dependencies**
Create a virtual environment (optional but recommended):

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Then, install the dependencies from the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

---

## **Usage**

### **Running the Notebook**
After installing the dependencies, you can run the notebook file (`image_filtering_project.ipynb`) in your preferred Python environment. If you are using Jupyter Notebooks, run:

```bash
jupyter notebook image_filtering_project.ipynb
```

Alternatively, if you're working in a local IDE, you can execute the code as Python scripts, but note that the interactive elements and visualizations are optimized for Jupyter notebooks.

---

## **Results**

### **Filter Performance Comparison**
The project results include a performance comparison between the three filters based on their **MSE** and **SQNR** metrics, as well as the **execution time** required to process the images.

- **Bilateral Filter**: Significantly faster and more effective at removing Gaussian noise while maintaining image integrity.
- **Adaptive Median Filter**: Best at handling salt-and-pepper noise, with a very high **SQNR**.
- **Adaptive Mean Filter**: Slightly slower and less effective at removing Gaussian noise but performs well with lower noise levels.
- **Basic Filters**: 
  - **Median Filter**: Effective for removing salt-and-pepper noise.
  - **Gaussian Filter**: Works well for Gaussian noise but tends to blur images.
  - **Box Filter**: Simple filter that works similarly to Gaussian but without smoothing capabilities.

### **Visualizing the Results**
- The notebook generates **histograms** and **bar plots** to visualize the MSE and SQNR for each noise level and filter type.
- **Images before and after filtering** are displayed for easy comparison.

---

## **Acknowledgements**

- **NumPy**: For efficient numerical operations.
- **OpenCV**: For image processing and manipulation.
- **Matplotlib**: For creating plots and visualizations.
- **Numba**: For optimizing the performance of filtering functions.

---

### **Contributing**
If you would like to contribute to this project, feel free to fork the repository, make changes, and submit a pull request. Please follow the standard GitHub flow for contributions.

---
