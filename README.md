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
git clone https://github.com/Raykosan/RaykoStudio-SaturationNode.git  
Restart ComfyUI.

2. Copy the RaykoStudio_Nodes folder to: ComfyUI/custom_nodes/  
Restart ComfyUI

## 🎛 Usage

🦊 RS Safe Saturation  
| Диапазон    | Тип обработки                  | Применение                  |
|-------------|--------------------------------|----------------------------|
| 0.0-0.9     | Тонирование/уменьшение насыщенности | Плавное обесцвечивание |
| 1.0-1.3     | Естественное усиление          | Рекомендуемый диапазон  |
| 1.3-2.0     | Яркие художественные эффекты   | Стилизация              |
| 2.0-3.0     | Максимальная насыщенность      | Спецэффекты             |

## ⚙️ Technical Details  

Algorithm workflow:

Luminance space conversion

Non-linear adjustment:
Values <1.0: Linear interpolation
Values >1.0: Adaptive S-curve

Auto highlight recovery

Recommended settings:  
| Intensity  | Effect                          |
|------------|---------------------------------|
| 0.0-0.9    | Toning/desaturation             |
| 1.0-1.3    | Natural enhancement (recommended) |
| 1.3-2.0    | Vibrant artistic effects        |
| 2.0-3.0    | Cinematic saturation           |
	
## 📜 License

MIT License. Free for commercial use.

## 🤝 Support

Report issues or suggest improvements:  
[Create a GitHub issue](https://github.com/Raykosan/RaykoStudio-SaturationNode/issues)

---

  > "The best saturation is the one you don’t notice" © RaykoStudio 2025
