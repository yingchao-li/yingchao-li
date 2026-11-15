# Hi, I'm Yingchao Li 👋

**M.Sc. Data Science @ FAU · Applied AI · Mathematical Optimization · Scientific Computing · Computer Vision**

Based in Nürnberg, Germany, I work across machine learning, computer vision, mathematical optimization and software engineering. I enjoy transferring computational methods across different domains and building complete systems—from mathematical modelling and algorithm implementation to numerical experiments, evaluation, interfaces and hardware integration.

[Portfolio](https://yingchao-li.github.io/) · [CV](https://yingchao-li.github.io/assets/Yingchao-Li-CV.pdf) · [LinkedIn](https://www.linkedin.com/in/yingchao-li-722071397/) · [Email](mailto:yingchao.li@fau.de)

## About me

- Pursuing an **M.Sc. in Data Science** at Friedrich-Alexander-Universität Erlangen-Nürnberg (FAU).
- Background in **Computer Science and Technology** at China University of Geosciences (Wuhan).
- Interested in **applied machine learning, computer vision, mathematical optimization and scientific computing**, with recent projects exploring quantum error correction.
- I enjoy connecting mathematical principles with practical implementations and evaluating solutions through reproducible experiments.

## Technology stack

| Area | Technologies & interests |
| --- | --- |
| AI & computer vision | PyTorch, scikit-learn, OpenCV, CNNs, GRUs, Transformers; object detection, image restoration, feature extraction |
| Mathematical optimization | SciPy, HiGHS, OR-Tools; LP, MILP, CP-SAT, genetic algorithms, simulated annealing |
| Quantum computing | Stim, PyMatching; quantum error correction, surface codes, MWPM, neural decoding |
| Scientific computing & data | Python, NumPy, pandas, SQL, SQLite, Plotly; numerical benchmarking and statistical evaluation |
| AI applications & web | JavaScript, React, FastAPI, REST APIs, SSE, Gradio, Streamlit, FAISS, Agentic RAG |
| Embedded systems | C / C++, ESP32-S3, FreeRTOS, ESP-DL, camera interfacing, GPIO |
| Development & testing | Git, pytest |

## Selected projects

### [AdaptiveQEC — Deep Learning for Fault-Tolerant Quantum Computing](https://github.com/yingchao-li/AdaptiveQEC-Deep-Learning-for-FTQC)

A surface-code decoding framework for **quantum error correction**, combining classical and neural decoders with experimental data from Google's Willow quantum processor.

- Five neural decoder architectures (MLP, ResMLP, 3D CNN, GRU and Transformer), benchmarked against classical MWPM decoding across 30 training experiments.
- **20.79% relative reduction in logical error rate (9.07% → 7.18%)** with the Transformer decoder on 90,000 distance-3, 10-round test samples.
- Confidence-aware hybrid decoding combining neural predictions, probability calibration and adaptive MWPM routing.

**Stack:** Python · PyTorch · Stim · PyMatching · NumPy

### [OptiFactory — Mathematical Optimization for Industrial Production & Machine Scheduling](https://github.com/yingchao-li/OptiFactory-Mathematical-Optimization)

A mathematical optimization framework for **job shop and flexible job shop scheduling (JSSP/FJSP)**, supporting numerical benchmarking and interactive schedule visualization.

- LP relaxation, MILP (Big-M), CP-SAT, genetic algorithms and simulated annealing; 492 successfully parsed benchmark instances.
- Heuristic-guided hybrid optimization (HGMO) improved feasible-solution coverage from **85.7% to 100%** and proven-optimal coverage from **71.4% to 85.7%**, relative to standard CP-SAT across seven instances under identical two-second configured budgets.
- A separate CP-SAT warm-start strategy achieved a **2.87× geometric-mean speedup** across five matched, proven-optimal benchmark pairs.
- 70 algorithm–instance evaluations; all 59 returned schedules passed independent constraint validation.

**Stack:** Python · SciPy · HiGHS · OR-Tools · NumPy · pandas · Streamlit

### [CVKit — Computer Vision & Algorithm Benchmarking Platform](https://github.com/yingchao-li/CV-Tool-Platform)

A modular vision toolkit covering **3D geometry, RAW / HDR imaging, image retrieval, object detection and face analysis**, exposed through one Python package, a unified CLI and a Streamlit studio. Developed as a **10-ECTS project at FAU (grade: 1.0)**.

- Robust plane fitting with RANSAC, MLESAC and Preemptive RANSAC, followed by PCA-based 3D box measurement.
- RAW demosaicing, camera-response calibration and HDR tone mapping; image retrieval with RootSIFT → VLAD → Exemplar SVM.
- Selective Search + HOG / SVM detection, open-set face recognition and unknown-identity rejection, with reproducible benchmarks.

**Stack:** Python · Streamlit · Gradio · OpenCV · scikit-learn

### [EV Reservation & Smart Parking Lock](https://github.com/yingchao-li/ev-charging-reservation-v2)

A Munich hackathon prototype connecting **map-based discovery, reservations, driver and operator dashboards, and ECURIOUS parking-lock integration**.

- React / Leaflet interfaces and a FastAPI / SQLite backend for accounts, vehicles, reservations, waitlisting and reallocation.
- Official REST / SSE integration with plate-based check-in, event deduplication, state synchronization and failure recovery.
- Separate Mock and Live modes; charging, cost and revenue figures are simulated or estimated. Physical hardware validation remains pending as documented on the portfolio.

**Stack:** React · Leaflet · FastAPI · SQLite · REST · SSE

### [ESP32-S3 Vision Alert](https://github.com/yingchao-li/esp32-s3-vision-alert)

On-device vision firmware designed for **person, bicycle and car detection**, with ROI tracking, graded buzzer alerts and a Wi-Fi dashboard.

- Integrates the official YOLO11n COCO 320 INT8 model through ESP-DL for inference on ESP32-S3.
- A bounded FreeRTOS pipeline connects camera capture, inference, tracking and alerts.
- Includes model SHA and tensor-contract checks, host tests and guarded flashing; traffic-cone detection is an extension in progress.

**Status:** In development. Firmware builds pass; on-board hardware testing is pending. No measured FPS or accuracy is claimed. A research prototype, not a navigation-safety product.

**Stack:** C++ · ESP32-S3 · ESP-DL · FreeRTOS · YOLO11n INT8

### [DeepSeek Multi-Mode Chat](https://github.com/yingchao-li/DeepSeek-Multi-Mode-Chat)

A Streamlit application for **document RAG, agentic retrieval, paper reading and tabular analysis**, with English, Chinese, German and French interfaces.

- Document upload, chunking, embeddings and FAISS retrieval; an agentic pipeline adds routing, grading, query rewriting, generation and verification.
- PDF text and figure extraction, structured paper summaries, and retrieval-based or full-text Q&A.
- CSV / Excel cleaning, natural-language analysis, Plotly charts, multi-table joins and scikit-learn baseline models.

**Stack:** Python · Streamlit · FAISS · DeepSeek · Plotly · scikit-learn

<details>
<summary><strong>EV Charging — First Prototype</strong></summary>

The [original EV charging repository](https://github.com/yingchao-li/ev-charging-reservation) validates the reservation-to-release business flow using an explicit Mock API.

- Separate React frontend, FastAPI application backend and Mock Server.
- Reservation conflicts, cancellation, role permissions, automatic check-in, incorrect plates, No-Show handling and blocked-bay alerts.
- The v2 project extends this architecture with official parking-lock REST / SSE adapters.

The original ECURIOUS API is a fictional hackathon mock; charging and revenue figures are simulations.

</details>

## Research

**Master's thesis research direction: Small-object detection**

Exploring multi-scale feature representations and coarse-to-fine region refinement for small-object detection. Ongoing research; experimental findings are subject to further validation.

**Bachelor's thesis: Prior-enhanced image restoration** · December 2024 – June 2025

Designed **PriAda-U-Net for dehazing** and **GRS-U-Net for deraining**, integrating dark-channel and gradient-map priors. Evaluated adaptive loss weighting through comparative experiments and ablation studies.

Reported dehazing experiment: **PSNR 34.13 dB · SSIM 0.8325**. See my [CV](https://yingchao-li.github.io/assets/Yingchao-Li-CV.pdf) for context.

## Education & experience

| Period | Role | Institution / organization |
| --- | --- | --- |
| Oct 2025 – Present | M.Sc. Data Science | Friedrich-Alexander-Universität Erlangen-Nürnberg |
| Sep 2024 – Mar 2025 | Software Development Intern | Guanghong · Retail business |
| Sep 2021 – Jun 2025 | B.Sc. Computer Science and Technology | China University of Geosciences (Wuhan) |

During my internship, I independently developed and deployed a **WeChat Mini Program** for product browsing and online orders, with a Python backend and AI customer support, and managed testing and maintenance.

## Get in touch

Happy to talk about applied AI, scientific computing, mathematical optimization, computer vision and software development.

- **Email:** [yingchao.li@fau.de](mailto:yingchao.li@fau.de)
- **Portfolio:** [yingchao-li.github.io](https://yingchao-li.github.io/)
- **LinkedIn:** [Yingchao Li](https://www.linkedin.com/in/yingchao-li-722071397/)

---

*Understand the principles. Build the whole system.*
