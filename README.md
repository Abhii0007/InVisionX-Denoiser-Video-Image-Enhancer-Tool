📋 Overview

InvisionX Denoiser, is an User-friendly feature-rich & Responsive App-Tool that leverages the power of GFPGAN (Generative Facial Prior Generative Adversarial Network) and RealESRGAN Generative AutoEncoder Models as backend to restore and enhance facial images. Regenerate high-quality image and upscale videos locally with AI-driven denoising. 



Interface Built with QT Framework for a modern GUI experience, this tool provides an intuitive interface for AI-powered image restoration with professional-grade features.
high-quality image and video upscaling locally with AI-driven denoising.


![home](images/Home.jpg)

✨ Features:-

🖼️ Advanced Image Display

🖱️ Zoom & Pan: Smooth mouse wheel zooming and drag-to-pan functionality

🖼️ Dual View: Side-by-side comparison of original and restored images

🎛️ View Controls: Reset view and fit-to-screen options

🔢 Real-time Zoom Info: Live display of current zoom percentage

🚀 AI-based Upscaling: Powered by Real-ESRGAN backend

🎥 Image & Video Support: Works seamlessly with both formats

🔍 Zoom Preview: Zoom in/out and preview results before saving

🖥️ Desktop Interface: Clean and easy-to-use GUI

⚡ GPU Acceleration: Faster processing using dedicated hardware

📂 One-click Save: Export results in high-quality formats





## 📸 Project Insights

| Face Restoration Window | Video Upscaling Window |
|--------------|---------------|
| ![home](images/face_restore.jpg) | ![video section](images/Home_video_section.jpg) |


| Image Enhancement with Inbuilt Overlay Markup | Project Log |
|--------------|---------------|
| ![Overlay markup](images/inbuilt_overlay_markup.jpg) | ![Model log](images/model_log.jpg) |



🔧 Tech Stack
    
    Backend AI Model: Real-ESRGAN
    Frontend: PySide6 (Qt for Python)
    Languages: Python
    Dependencies: OpenCV, Ffmpeg
    Ffmpeg should intalled in computer and set as System-Env-path
    
📌 Use Cases
    
    Enhance old or low-resolution images
    Restore noisy/compressed pictures
    Upscale anime, artwork, or photos for printing
    Improve video clarity and sharpness
    


Basic Workflow
    
    Select Image: Click "Select Image" to choose your input photo
    Choose Enhancement: Select upscale factor (2x, 4x, or 8x)
    Restore Image: Click "Start Restoration" to begin AI processing
    Compare Results: Use zoom and pan to compare original vs restored
    Save Output: Auto-saved to results_gui/ or use manual save option


Supported Image Formats
    
    Input: PNG, JPG, JPEG, BMP, TIFF
    Output: PNG, JPG, JPEG



Key Components
    
    ZoomableLabel: Custom widget for advanced image interaction
    RestorationWorker: QThread-based processing for non-blocking operations
    GFPGANApp: Main application class with professional UI
    GFPGANer: Backend AI model interface

Performance Notes
    
    GPU Acceleration: Recommended for optimal performance
    Memory Usage: Higher upscale factors require more VRAM
    Processing Time: Varies based on image size and hardware


🚀 Getting Started
Clone this repository
Install dependencies (requirements.txt)
Run main.py to start the desktop application

### 🔧 Installation Requirements
This project requires **FFmpeg** (for video processing) and **OpenCV** (for image and video handling). Please follow the steps below to install them.

Prerequisites
    
    Python 3.8 or higher
    GPU with CUDA support (recommended for faster processing)


# Dependencies:

    PySide6>=6.4.0
    opencv-python>=4.5.0
    numpy>=1.21.0
    torch>=1.9.0
    torchvision>=0.10.0
    gfpgan>=1.3.0
    basicsr>=1.4.0
    facexlib>=0.3.0




#### 📥 Install FFmpeg (Windows)
First install Pyside6 in python using:

    pip install PySide6
    

1. Download FFmpeg from the official builds:
   👉 [FFmpeg Download Page](https://www.ffmpeg.org/download.html)

2. Download the file: **ffmpeg-release-essentials.zip**.

3. Extract the ZIP to a folder, e.g. `C:\ffmpeg`.

4. Add FFmpeg to your **PATH**:

   * Press `Win + R`, type `sysdm.cpl`.
   * Go to **Advanced > Environment Variables**.
   * Under **System variables**, select `Path` → **Edit** → **New**.
   * Add:

         C:\ffmpeg\bin
     
           * Save and close.

5. Verify installation in Cmd:

       ffmpeg -version

   If you see version info, FFmpeg is installed successfully ✅


#### 📥 Install OpenCV (Python)

Run the following in your terminal (cmd, PowerShell, or VS Code terminal):
  
    pip install opencv-python


#### ✅ Quick Test

Check that both dependencies are working:

```bash
# Test OpenCV
import cv2
print(cv2.__version__)

# Test FFmpeg
# Run in command prompt:
ffmpeg -version
```

If both return version info, your setup is complete 🚀



🧠 About Real-ESRGAN
This project uses the public **Real-ESRGAN** trained model as backend for image and video-Frames upscaling and denoising.  
You can find the model repository here: [Real-ESRGAN GitHub](https://github.com/xinntao/Real-ESRGAN)


Real-ESRGAN (Real-Enhanced Super-Resolution Generative Adversarial Network) is an AI model designed for real-world image enhancement, capable of removing noise, restoring details, and producing natural high-resolution outputs.
Bring your images and videos back to life no need to prompt or genreate frames and extract then manuallu upscale and build etc, do this in just single button easliy and quickly with our InVisionX Denoiser user friendly Interface Tool.




📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
    
    Tencent ARC for GFPGAN
    PySide6 for the GUI framework
    BasicSR for image restoration utilities

📞 Support
If you encounter any issues or have questions:

Check the Issues page

Create a new issue with detailed information

Include system specifications and error logs

🚀 Future Enhancevements

    Batch processing multiple images
    Additional AI models support
    Video restoration capabilities
    Advanced image filters and adjustments
    Plugin system for extensibility



🤝 Contributing
We welcome contributions!





