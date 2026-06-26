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
Embedded work on the BMS pole: STM32 firmware, CAN, and system modelling in Capella.

**[Battery cycle-life prediction](https://github.com/sami-ennedoui/battery-cycle-life)** · 2026
Early prediction of Li-ion cycle life from the first 100 cycles on the A123 dataset. A reproduction of the Severson 2019 benchmark with a leakage-safe per-cell split and elastic-net against XGBoost, around 15% MAPE. Served behind a FastAPI endpoint with Docker and CI. I owned the framing, the split policy and the evaluation.

**[STM32 datasheet assistant](https://sami-ennedoui-stm32-datasheet-rag.hf.space)** · [code](https://github.com/sami-ennedoui/stm32-datasheet-rag) · 2026
Question answering over the 3000 page STM32H7 manual, where every answer cites its source page. Sentence-transformer embeddings, a Chroma vector store, and a smolagents agent that writes register headers with the address arithmetic kept in Python, never the model. Built for the racing team.

**[Hilbert-RAG, CPU retrieval with a space-filling-curve index](https://github.com/sami-ennedoui/hilbert-rag)** · 2026
I took the Hilbert curves from my TIPE and tried them as a retrieval index. A FastAPI search and answer service with sentence-transformer embeddings and a PyTorch projection head, trained with a contrastive loss to feed the curve, benchmarked against FAISS Flat and HNSW. The result is negative and I report it as one. At this corpus size HNSW wins unfiltered search and an exact pre-filter wins under selective filters, so the curve index wins no regime. The trained projection still beats PCA as the index key, and the real value of the project is a benchmark I can defend.

**[malaigue-from-space, testing a foundation model on a real crisis](https://github.com/sami-ennedoui/malaigue-from-space)** · 2026
A geospatial pipeline that asks whether the Clay foundation model, used frozen and zero-shot, can see the 2018 malaïgue in the étang de Thau, an anoxic crisis that killed most of the lagoon's shellfish. Sentinel-2 imagery from a STAC API, a geopandas core for masking and reprojection, an NDCI chlorophyll index, and IFREMER in-situ records as ground truth. The answer is no. Clay's embeddings do not track the crisis, and I report that as a clean negative, with the in-situ oxygen as the measurement that does mark it. Python, geopandas, rasterio, PyTorch on CPU.

**[AI tech watch with n8n](https://github.com/sami-ennedoui/veille-ia-n8n)** · 2026
An n8n workflow that follows AI news on its own. It reads RSS feeds from Hugging Face, arXiv and MIT Technology Review every few hours, summarizes each new article with a language model, deduplicates against a state file, and appends the results to Markdown and CSV. Runs in a container.

## Currently
- ModIA at ENSEEIHT and INSA Toulouse. First year done, moving into the data and AI core.
- N7 Racing Team, BMS and telemetry.
- Co-founded N7 IA, the school's AI club.

## Stack
Python, C, C++, NumPy, SciPy, scikit-learn, pandas, SQL. PyTorch, including a small model I trained with a contrastive loss. RAG, embeddings and vector stores with FAISS and Chroma. geopandas, rasterio and STAC for geospatial work. n8n for workflow automation. Git, GitHub Actions, Docker, Podman, Linux Fedora. TensorFlow at a basics level.
