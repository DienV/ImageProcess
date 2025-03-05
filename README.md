### 1️⃣ **Create a Virtual Environment**
Before running the project, create a virtual environment to manage dependencies:
```bash
python -m venv myenv
```

Activate the virtual environment:
- **Windows**:
  ```bash
  myenv\Scripts\activate
  ```
- **Mac/Linux**:
  ```bash
  source myenv/bin/activate
  ```

---

### 2️⃣ **Install Dependencies**
Install all required Python packages using `requirements.txt`:
```bash
pip install -r requirements.txt
```

---

### 3️⃣ **Prepare Input Images**
Place your images inside the `images/` folder. There are a few sample images in the `/images` folder

---

### 4️⃣ **Run the Script**
Run the Python script to process images:
```bash
python image_process.py
```

---

### 5️⃣ **Output Files**
Output will include processed images for each images inside the input folder, followed by their respective Histogram charts

Processed images will be saved in the `processed_images/` folder.

Each image will have:
- `enhanced_<filename>.jpg` → Histogram Equalization applied.
- `noisy_<filename>.jpg` → Gaussian noise added.
- `arithmetic_filtered_<filename>.jpg` → Denoised with Arithmetic Mean Filter.
- `geometric_filtered_<filename>.jpg` → Denoised with Geometric Mean Filter.
- `gaussian_filtered_<filename>.jpg` → Denoised with Gaussian Filter.
---
