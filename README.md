# AI Future Directions — Assignment Submission

**Student:** Jason Chiagozie  
**Course:** AI Future Directions  
**Assignment:** Pioneering Tomorrow’s AI Innovations  
**Submitted:** November, 2025

---

## Repo structure
(see top-level files and folders)

## Part 1: Theoretical Analysis
**Q1 — Edge AI vs Cloud AI (summary)**  
Edge AI reduces latency by processing inference close to the data source (on-device), reduces network dependence and bandwidth, and enhances privacy because raw data does not need to be sent to remote servers. Example: autonomous drones process camera frames on-board for real-time obstacle avoidance, so decisions happen within milliseconds and sensitive footage never leaves the drone.

**Q2 — Quantum AI vs Classical AI (summary)**  
Quantum AI leverages quantum algorithms (quantum annealing, QAOA) to explore large combinatorial search spaces more efficiently for certain optimization problems. Classical AI uses heuristic and gradient-based methods. Industries likely to benefit earliest: logistics & routing, financial portfolio optimization, materials discovery, and drug design.

(Full essay responses are in `docs/`)

---

## Part 2: Practical Implementation

### Task 1 — Edge AI Prototype
**Goal:** lightweight image classifier for recyclable items.

Files:
- `notebooks/edge_image_classifier.ipynb` — Colab-ready notebook: dataset loading, training, evaluation, TFLite conversion, and sample inference.
- `src/train.py` — script to reproduce training (if running locally).
- `src/convert_to_tflite.py` — conversion & quantization.
- `src/pi_test.py` — simple inference script for Raspberry Pi (simulation).

Key results (fill after you train):
- Model: MobileNetV2 (transfer learning)
- Test accuracy: **XX.XX%**
- TFLite size: **XX KB/MB**
- Quantized TFLite size: **XX KB/MB**

Deployment steps (short):
1. Train in notebook or Colab.
2. Convert model to `.tflite` using `convert_to_tflite.py` (with representative dataset for quantization).
3. Copy `.tflite` file to device (Raspberry Pi).
4. Run `pi_test.py` to perform inference with TensorFlow Lite Interpreter.

### Task 2 — AI-Driven IoT Concept (Smart Agriculture)
See `docs/diagrams.md` for sensors list, proposed model, and data flow diagram.

---

## How to reproduce (Colab)
1. Open `notebooks/edge_image_classifier.ipynb` in Colab.
2. Run cells (install `tensorflow`/`tensorflow-lite` if needed).
3. Upload `data/` (if you want to use your own sample images).
4. Run training cell; then run TFLite conversion cell.
5. Download `.tflite` model from Colab.

---

## What to submit for grading
1. Public GitHub repository URL — must point to the root of this repo.
2. Ensure the notebook runs in Colab (tested).
3. Fill in final accuracy metrics in README before submission.

---

## License
MIT

