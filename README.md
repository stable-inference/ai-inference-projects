# LLM Local Test

## Goal
Run a local LLM on my machine

---

## Hardware

- CPU: Ryzen 5 3600 / Ryzen 7 3700
- GPU: RX470 (x3), RX570 (x1)
- RAM: ...

---

## Setup

Custom multi-GPU setup using risers.

![GPU rig](../assets/setup/GPU-rig-1.jpg)
![GPU rig 2](../assets/setup/GPU-rig-2.jpg)

Riser connections:

![Riser](../assets/setup/riser.jpg)
![Connection](../assets/setup/Connection.jpg)

---

## Issue: 3 GPU instability

When using 3 GPUs on the initial setup, the system became unstable.

Observed behavior:
- System freezes during model loading
- Random crashes
- Unstable inference

With 1–2 GPUs everything worked fine.

---

## Result

After hardware adjustments (SlimSAS risers), the system became stable.

Inference running:

![Inference](../assets/results/Inference.png)
![Running](../assets/results/Inference-running.png)

GPU load:

![HWiNFO](../assets/results/HWiNFO-GPU.png)

---

## Models Tested

- Qwen
- DeepSeek
- Various GGUF models

---

## Notes

- Multi-GPU on consumer hardware is tricky
- Stability depends heavily on risers and connections
- Real-world testing is required
