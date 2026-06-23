# Sami Ennedoui

Engineering student at ENSEEIHT, in the ModIA double diploma with INSA Toulouse, 2025 to 2028. ModIA stands for modelling, data and AI.

Two years of prépa MP, then a first year in electrical engineering. Most of what I know I picked up by building things. Signal processing and embedded systems first, low level C next, and applied AI and data more recently. The projects below run in that order.

Looking for a 2 to 3 year AI and Data apprenticeship from September 2026. Based in Toulouse, open to the rest of France.

## Projects

**[TIPE, Space-Filling Curves and Image Compression](https://github.com/sami-ennedoui/TIPE-SpaceFillingCurves)** · 2023 to 2025
My prépa research project. I reordered image traversal with Hilbert, Morton and Peano curves before dithering, which helps lossless compression. Up to 89% size reduction on a 1 bit image, and about 3.2% better than a linear scan for the same dithering method. Python, NumPy, SciPy.

**[CHIP-8 interpreter in C](https://github.com/sami-ennedoui/chip8-c)**
A working CHIP-8 emulator on SDL3. Opcode decoding, a 4 KB memory map, display and timer handling. Sound is the last piece left to add.

**N7 Racing Team, battery management** · since 2025
Embedded work on the BMS pole: STM32 firmware, CAN, and system modelling in Capella. I also wrote a tool that reads component datasheets from PDF and outputs strict JSON and C headers for the firmware.

**[Battery cycle-life prediction](https://github.com/sami-ennedoui/battery-cycle-life)** · 2026
Early prediction of Li-ion cycle life from the first 100 cycles on the A123 dataset. A reproduction of the Severson 2019 benchmark with a leakage-safe per-cell split and elastic-net against XGBoost, around 15% MAPE. Served behind a FastAPI endpoint with Docker and CI. I owned the framing, the split policy and the evaluation.

**[STM32 datasheet assistant](https://sami-ennedoui-stm32-datasheet-rag.hf.space)** · [code](https://github.com/sami-ennedoui/stm32-datasheet-rag) · 2026
Question answering over the 3000 page STM32H7 manual, where every answer cites its source page. Sentence-transformer embeddings, a Chroma vector store, and a smolagents agent that writes register headers with the address arithmetic kept in Python, never the model. Built for the racing team.

## Currently
- ModIA at ENSEEIHT and INSA Toulouse. First year done, moving into the data and AI core.
- N7 Racing Team, BMS and telemetry.
- Co-founded N7 IA, the school's AI club.

## Stack
Python, C, C++, NumPy, SciPy, scikit-learn, SQL. Git, GitHub Actions, Docker, Podman, Linux Fedora. RAG, embeddings, vector stores, LLM tooling. PyTorch and TensorFlow at a basics level.
