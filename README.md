Multimodal Gradio Application
![image](https://github.com/user-attachments/assets/1d7ea183-c510-4d2b-bed7-7f378ee847fa)

A user-friendly Gradio interface combining image analysis and code generation capabilities using state-of-the-art AI models.
🚀 Features

Dual-Mode Interface: Image description and code generation in one application
Advanced AI Models: Integration of DeepSeek-R1-Distill-Qwen-1.5B and llava-1.5-7b-hf
Adjustable Parameters: Fine-tune temperature, top-p, and max tokens for optimal results
Real-Time Feedback: Immediate parameter tuning with live results
GPU Optimized: Designed for Google Colab T4 GPU environment
User-Friendly: Intuitive interface with example prompts

🖼️ Image Description
Generate detailed textual descriptions from uploaded images with customizable prompts and parameters.
💻 Code Generation
Produce functional code snippets from natural language prompts with best practices integration.
📋 Prerequisites

Google Colab account (recommended) or local environment with GPU
Python 3.8+
CUDA-compatible GPU (T4 recommended, 12GB VRAM)

🛠️ Installation
Google Colab Setup (Recommended)

Open a new Google Colab notebook
Select GPU runtime:
Runtime → Change runtime type → Hardware accelerator → GPU (T4)

Install dependencies:
python!pip install transformers==4.36.0 gradio==4.8.0 torch torchvision pillow


Local Installation
bashgit clone https://github.com/yourusername/multimodal-gradio-app.git
cd multimodal-gradio-app
pip install -r requirements.txt
🚀 Usage
Starting the Application
pythonpython Objects_Task.py
Live Demo
Try the application on Hugging Face Spaces
(Note: CPU-based, slower than GPU setup)
📖 User Guide
Image Description Tab

Upload Image: Support for JPG, PNG, and other common formats
Custom Prompt: Modify description prompts (optional)
Adjust Parameters:

Temperature (0.1-1.0): Controls creativity vs consistency
Top-p (0.1-1.0): Nucleus sampling parameter
Max Tokens (50-500): Maximum description length


Generate: Process and analyze the image

Code Generation Tab

Enter Prompt: Describe the desired code functionality
Set Parameters: Same controls as image description
Generate: Create functional code snippets

💡 Example Prompts
Image Description
✅ Good prompts:
- "Describe this image in detail, including objects, colors, and scene composition"
- "Analyze this image and explain what's happening in the scene"
- "Provide a comprehensive description of all visual elements in this image"

🎛️ Recommended parameters:
- Temperature: 0.3-0.7 (balanced creativity)
- Top-p: 0.8-0.9 (diverse but coherent)
- Max tokens: 100-200 (detailed descriptions)
Code Generation
✅ Good prompts:
- "Create a Python function to calculate the factorial of a number"
- "Write a JavaScript function to validate email addresses using regex"
- "Generate a Python function for bubble sort algorithm"

🎛️ Recommended parameters:
- Temperature: 0.1-0.3 (precise, functional code)
- Top-p: 0.7-0.8 (focused generation)
- Max tokens: 300-400 (complete functions)
🔧 Troubleshooting
Slow Generation

⚡ Reduce max_new_tokens
🖼️ Use lower resolution images
🔥 Ensure GPU is properly utilized

Poor Image Recognition

✅ Verify supported image format
📏 Check image quality and resolution
📝 Try different prompt formulations

Inconsistent Code Generation

🌡️ Lower temperature (0.1-0.3)
🎯 Be more specific in prompts
🏷️ Include programming language specification

🛠️ Parameter Guide
ParameterRangeImage DescriptionCode GenerationTemperature0.1-1.00.3-0.7 (balanced)0.1-0.3 (precise)Top-p0.1-1.00.8-0.9 (diverse)0.7-0.8 (focused)Max Tokens50-500100-200 (detailed)300-400 (complete)
