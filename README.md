🦊 RS Safe Saturation Node for ComfyUI

Professional image saturation control with artifact and highlight protection.

🔥 Demo Features

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
├── 0.0 = Full desaturation
├── 1.0 = Original saturation
├── 1.5 = Safe boost
└── 3.0 = Maximum saturation (protected)
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
Create a GitHub issue

    "The best saturation is the one you don’t notice" © RaykoStudio 2024

Key Improvements:

    Localized UI terms (e.g., "Подключите изображение" → "Connect image")

    Technical clarity for international users

    Maintained markdown formatting and emojis

    Culturally adapted the quote while preserving its meaning

Would you like me to:

    Add ComfyUI version compatibility notes?

    Include benchmark results?

    Add a "Quick Start" video link section?

При копировании текста в файл Readme в репозиторий сбивается разметка

Вот как правильно сохранить разметку при копировании в README.md, с полным кодом и рекомендациями:
🔧 Исправленный файл README.md (сохраняет форматирование)
markdown
Copy

# 🦊 RS Safe Saturation Node for ComfyUI  
**Professional image saturation control with artifact and highlight protection.**  

![Demo](web/preview.png)  

---

## 🔥 Features  
- **Smooth adjustment** with 0.05 steps  
- **Smart boosting** without overexposure  
- **Artifact protection** even at extreme values  
- **Batch processing** optimized  
- **Supports**: Windows/Linux · Python 3.11+ · PyTorch 2.0+  

---

## 🛠 Installation  
1. Clone the repo to `ComfyUI/custom_nodes/`:  
   ```bash
   git clone https://github.com/Raykosan/RaykoStudio-SaturationNode.git

    Restart ComfyUI.

🎛 Usage
plaintext
Copy

[ 🦊 RS Safe Saturation ]
├── Image: [Connect input]
├── Intensity: 1.0 (0.0-3.0)
│   ├── 0.0 = Grayscale
│   ├── 1.0 = Original
│   ├── 1.5 = Subtle boost
│   └── 3.0 = Max safe saturation
└── Output: [Processed image]

⚙️ Technical Details
Algorithm workflow:

    Luminance space conversion

    Non-linear adjustment:

        Values <1.0: Linear interpolation

        Values >1.0: Adaptive S-curve

    Auto highlight recovery

Recommended settings:
Intensity	Effect
0.0-0.9	Toning/desaturation
1.0-1.3	Natural enhancement (recommended)
1.3-2.0	Vibrant artistic effects
2.0-3.0	Cinematic saturation
📜 License

MIT License. Free for commercial use.
🤝 Support

Report issues or suggest improvements:
[Create a GitHub issue](https://github.com/Raykosan/RaykoStudio-SaturationNode/issues)

---

> "The best saturation is the one you don’t notice" © RaykoStudio 2025
