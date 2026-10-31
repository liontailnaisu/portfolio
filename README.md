# Technical Project Portfolio: Machine Learning & Data Engineering
**Peter Emebo** | Python • SQL • PyTorch • Data Pipelines • Hardware Optimization

## Feature Project: Edge AI Cassava Leaf Disease Classifier (ARM Target)
![Image 1](Screenshot%202026-03-15%20224224.png) ![Image 2](Screenshot%202026-03-16%20085536.png) ![Image 3](Screenshot%202026-03-28%20221856.png) 
![Image 4](Screenshot%202026-04-18%20160609.png) ![Image 5](Screenshot%2026-04-15%153727.png) 
**Project Type:** Machine Learning & Internet of Things (ML/IoT) | **Timeline:** Apr 2026 – Jun 2026

*   **Architecture:** Developed a localized, hardware-optimized edge computer vision pipeline utilizing a MobileNetV2 framework trained on the Kaggle dataset.
*   **Optimization:** Applied static INT8 Post-Training Quantization (PTQ) to convert parameters from FP32 to 8-bit integers, minimizing raw model storage overhead.
*   **Hardware Insight:** Evaluated strict TinyML module hardware constraints. While the isolated runtime shell compiled successfully, integrating the full static data arrays and `#include` image dependencies pushed the cumulative tensor activation memory past the microcontroller unit's volatile storage capacity (SRAM), resulting in a runtime memory ceiling failure.
*   **Key Takeaway (Raw-to-Refined Ingestion):** Provided a definitive case study in embedded ML constraints, proving that edge-device deployment requires upfront input data downsampling and strict pipeline engineering to prevent raw ingestion pipelines from exhausting localized chip memory.

## Core Engineering Project: Real-Time Telemetric Data Ingestion Engine
### Architecture: Bare-Metal Microcontroller Data Stream Monitoring

*   **Pipeline Execution:** Programmed a bare-metal, hardware-interrupt driven processing engine to ingest continuous environmental telemetric data streams.
*   **Analytical Verification:** Structured a dedicated data pipeline routing live telemetry straight from microcontrollers to a local PC validation environment, debugging bit-level data transmission constraints to achieve total architectural reliability.
