🦊 RS Safe Saturation Node for ComfyUI

Professional image saturation control with artifact and highlight protection.

Demo
🔥 Features

    Smooth adjustment with 0.05 steps

    Smart boosting without overexposure

    Artifact protection even at extreme values

    Optimized for batch image processing

    Supports Windows/Linux, Python 3.11+, PyTorch 2.0+

🛠 Installation

    Copy the RaykoStudio_Nodes folder to:
    Copy

    ComfyUI/custom_nodes/

    Restart ComfyUI

🎛 Usage
Copy

[ 🦊 RS Safe Saturation ]
├── Image: [Connect image]
├── Intensity: 1.0 (0.0-3.0)
│   ├── 0.0 = Full desaturation
│   ├── 1.0 = Original saturation
│   ├── 1.5 = Safe boost
│   └── 3.0 = Maximum saturation (protected)
└── Output: [Processed image]

⚙️ Technical Details
Algorithm:

    Conversion to luminance space

    Non-linear saturation adjustment:

        Values <1.0: Linear interpolation

        Values >1.0: Adaptive S-curve boosting

    Automatic highlight correction

Recommended values:

    0.0-0.9: Toning/reduced saturation

    1.0-1.3: Natural enhancement (recommended)

    1.3-2.0: Vibrant colors for artistic effects

    2.0-3.0: Max saturation (for special FX)

📜 License

MIT License. Free for commercial and non-commercial use.
🤝 Support

Found a bug or have suggestions?
[Create a GitHub issue](https://github.com/Raykosan/RaykoStudio-SaturationNode/issues)

---

> "The best saturation is the one you don’t notice" © RaykoStudio 2025
