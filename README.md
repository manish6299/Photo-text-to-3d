# 🧠 PhotoTextTo3D

A Python prototype that converts either a **photo** or a **text prompt** into a simple 3D model (`.obj` or `.stl`). Designed for 3D viewing or 3D printing. The goal is to demonstrate AI-assisted geometry generation and basic mesh processing using open-source tools.

---

## 🔧 Features

- Accepts `.jpg`, `.png` image or short text prompt
- Removes background from images using AI
- Generates basic 3D mesh using open-source models or approximations
- Saves output as `.obj` or `.stl`
- Displays the model using `pyrender` or `open3d`

---

## 🧠 Thought Process

This project was designed as a prototype to bridge simple 2D inputs and 3D outputs using AI:

- **Image input**: isolate object → create voxel/mesh → export as 3D model
- **Text input**: describe object → use AI to estimate shape → convert to 3D mesh
- 3D models are kept basic to demonstrate working pipeline
- Components are modular and easy to extend

---

## 🧾 Libraries Used

| Library      | Purpose                                  |
|--------------|------------------------------------------|
| `rembg`      | Removes background from image            |
| `torch`      | Runs AI models for 3D generation         |
| `trimesh`    | 3D mesh manipulation                     |
| `pyrender`   | Mesh visualization in 3D window          |
| `open3d`     | Alternate viewer for .obj/.stl files     |
| `Pillow`     | Image loading and processing             |
| `numpy`      | Numerical array operations               |
| `matplotlib` | (Optional) static 3D plots               |

---

## 🗂️ Project Structure

## ✅ Step 2: Create Virtual Environment
## python -m venv venv
### venv\Scripts\activate        # On Windows
### # or
### source venv/bin/activate     # On Mac/Linux

## ✅ Step 3: Install Dependencies
## pip install -r requirements.txt
pip install onnxruntime

## ✅ Step 4: Run the Application
### python main.py --image assets/toy_car.jpg
### python main.py --text "a small red toy car"



