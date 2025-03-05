### 1 **Create a Virtual Environment**

First, a virtual environment to manage dependencies need to be created:
```bash
python -m venv myenv
```

To activate the virtual environment:
- **Windows**:
  ```bash
  myenv\Scripts\activate
  ```
- **Mac/Linux**:
  ```bash
  source myenv/bin/activate
  ```

---

### 2 **Install required packages**

Using `requirements.txt` to install all the required Python packages:
```bash
pip install -r requirements.txt
```

---

### 3 **Prepare Input Images**

Place the images that need processing inside the `images/` folder. There are a few sample images already inside the folder

---

### 4 **Run the Script**

Run the Python script to process images and show the Histogram charts for each of them at each process:

```bash
python image_process.py
```

---

### 5 **Output Files**

Output will include processed images for each images inside the input folder, followed by their respective Histogram charts

Processed images will be saved in the `processed_images/` folder.

Each image will have:
- `enhanced_<filename>.jpg` → Histogram Equalization applied.
- `noisy_<filename>.jpg` → Gaussian noise added.
- `arithmetic_filtered_<filename>.jpg` → Denoised with Arithmetic Mean Filter.
- `geometric_filtered_<filename>.jpg` → Denoised with Geometric Mean Filter.
- `gaussian_filtered_<filename>.jpg` → Denoised with Gaussian Filter.
---
