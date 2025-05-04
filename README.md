# Prompt3D
# Photo/Text to Simple 3D Model Generator (Prototype)

## 🔧 What It Does:
- Accepts an image (.jpg/.png) or a short text prompt.
- Generates a basic 3D model (.obj or .stl).
- Displays a visualization of the 3D output.

## 🧠 My Approach:
- Used OpenAI’s `Point-E` for text-to-3D and image-to-3D point cloud generation.
- Cleaned photo input using `rembg` for better 3D model generation.
- Converted point clouds to mesh using `trimesh`.

## 🛠️ Libraries Used:
- `point-e`, `rembg`, `trimesh`, `pyrender`, `matplotlib`

## ▶️ How to Run:

# Create environment and activate
python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the script
python main.py --input_type text --input_data "a toy car"
# or
python main.py --input_type image --input_data inputs/toy.jpg
