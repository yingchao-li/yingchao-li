# Hi, I'm Yingchao Li 👋

**M.Sc. Data Science @ FAU · Applied AI · Scientific Computing · Engineering Software**

Based in Nürnberg, Germany, I work across machine learning, computer vision, mathematical optimization, scientific computing and software engineering.

I enjoy transferring computational methods across different engineering domains and building complete systems — from mathematical modelling and algorithm implementation to numerical experiments, software architecture, automated testing, interactive interfaces and hardware integration.

[Portfolio](https://yingchao-li.github.io/) · [CV](https://yingchao-li.github.io/assets/Yingchao-Li-CV.pdf) · [LinkedIn](https://www.linkedin.com/in/yingchao-li-722071397/) · [Email](mailto:yingchao.li@fau.de)

## About me

- Pursuing an **M.Sc. in Data Science** at Friedrich-Alexander-Universität Erlangen-Nürnberg (FAU).
- Background in **Computer Science and Technology** at China University of Geosciences (Wuhan).
- Interested in applied machine learning, computer vision, mathematical optimization, scientific computing and industrial software development.
- Exploring interdisciplinary applications in quantum computing, electroacoustics, embedded intelligence and engineering automation.
- Passionate about connecting mathematical principles with practical implementations, reproducible experiments and reliable software systems.

## Technology Stack

| Area | Technologies & interests |
| --- | --- |
| Programming | Python, C, C++17, MATLAB, JavaScript, TypeScript, SQL |
| Machine Learning & Computer Vision | PyTorch, scikit-learn, OpenCV, CNNs, GRUs, Transformers, YOLO, object detection, image restoration |
| Mathematical Optimization | SciPy, HiGHS, OR-Tools, LP, MILP, CP-SAT, genetic algorithms, simulated annealing |
| Scientific Computing | NumPy, SciPy, pandas, MATLAB, numerical modelling, statistical analysis, reproducible benchmarking |
| Digital Signal Processing | FFT, STFT, Welch PSD, FIR/IIR filters, frequency response, RMS, SNR, THD, acoustic measurements |
| Quantum Computing | Stim, PyMatching, surface codes, quantum error correction, MWPM, neural decoding |
| Industrial Software | C++17, CMake, SCPI/TCP, virtual instruments, measurement automation, firmware regression testing |
| AI Applications | LLMs, Agentic RAG, FAISS, prompt engineering, workflow automation |
| Full-Stack Development | React, TypeScript, Vite, Tailwind CSS, FastAPI, REST APIs, SSE, SQLite |
| Data Visualization | Recharts, Plotly, Matplotlib, Streamlit, Gradio |
| Embedded Systems | C/C++, ESP32-S3, FreeRTOS, ESP-DL, camera interfacing, GPIO |
| Software Quality | Git, Pytest, Catch2, Vitest, Playwright, ASan, UBSan, GitHub Actions |

## Selected Projects

### Computer Vision & Embedded Intelligence

#### [CVKit — Computer Vision & Algorithm Benchmarking Platform](https://github.com/yingchao-li/CV-Tool-Platform)

A modular computer vision toolkit covering **3D geometry, RAW/HDR imaging, image retrieval, object detection and face analysis**, exposed through a unified Python package, CLI and interactive research studio.

Developed as a **10-ECTS academic project at FAU (grade: 1.0)**.

- Robust plane fitting with RANSAC, MLESAC and Preemptive RANSAC, followed by PCA-based 3D box measurement.
- RAW demosaicing, camera-response calibration, HDR tone mapping and image retrieval using RootSIFT, VLAD and Exemplar SVM.
- Selective Search and HOG/SVM object detection, open-set face recognition and unknown-identity rejection.
- Reproducible numerical experiments and algorithm benchmarking.

**Stack:** Python · OpenCV · scikit-learn · Streamlit · Gradio

#### [ESP32-S3 Vision Alert](https://github.com/yingchao-li/esp32-s3-vision-alert)

An embedded computer vision prototype for **on-device object detection and intelligent proximity alerts**.

- Integrates the official YOLO11n COCO 320 INT8 model through ESP-DL.
- FreeRTOS pipeline connecting camera capture, inference, ROI tracking and graded buzzer alerts.
- Wi-Fi monitoring interface, model integrity checks and tensor-contract validation.

**Status:** In development. Firmware build and host tests are documented; on-device inference validation remains pending. Research prototype, not a navigation-safety product.

**Stack:** C++ · ESP32-S3 · FreeRTOS · ESP-DL · YOLO11n INT8

### Industrial Software & Scientific Computing

#### [MeasureFlow — Automated Instrument Control & Testing Platform](https://github.com/yingchao-li/MeasureFlow-Automated-Instrument-Testing-Platform)

A full-stack **electroacoustic measurement and test automation platform**, combining a C++17 backend, React frontend and Python-based virtual instruments.

- SCPI/TCP communication, instrument management, calibration tracking, timeout handling, automatic reconnection and fault recovery.
- Seven configurable test sequences covering RMS, Gain, THD, SNR, Noise Floor and Frequency Response.
- Real-time waveform and spectrum visualization, firmware regression analysis and automated CSV/HTML/PDF reporting.
- Ten reproducible engineering experiments, including 1,200 communication queries and 500 batch testing cases.
- **1,187 passing test cases**, with **90.7% C++ backend line coverage** and **99% Python simulator coverage**.

**Validation:** Simulated instruments only; no physical instrument or medical-device certification testing.

**Stack:** C++17 · Python · React · TypeScript · SCPI/TCP · CMake · Catch2 · Pytest · Playwright

#### [AcousticBench — Electroacoustic Measurement & Validation Toolkit](https://github.com/yingchao-li/AcousticBench-Electroacoustic-Measurement-Toolkit)

A scientific computing toolkit for **hearing aid measurement analysis, digital signal processing, numerical validation and automated engineering reporting**.

- Analysis of real-world hearing aid transmission data, including frequency response, acoustic feedback, real-ear gain and probe-tube measurement bias.
- FFT, STFT, Welch PSD, FIR/IIR filtering, H1 transfer-function estimation, SNR and THD analysis.
- Virtual hearing aid simulation, multiband dynamic compression and 1,000 deterministic synthetic validation cases.
- Sixteen experiment modules, interactive scientific visualization and automated PDF/Excel/HTML reporting.
- **557 passing Python tests**, with **93.9% core package test coverage**.

**Validation:** Python implementation tested; independent MATLAB implementation authored but not yet executed. Not a clinically validated measurement system.

**Stack:** Python · MATLAB · NumPy · SciPy · Streamlit · Plotly · Pytest

### Mathematical Optimization & Quantum Computing

#### [AdaptiveQEC — Deep Learning for Fault-Tolerant Quantum Computing](https://github.com/yingchao-li/AdaptiveQEC-Deep-Learning-for-FTQC)

A surface-code decoding framework for **quantum error correction**, combining classical and neural decoders with experimental data from Google's Willow quantum processor.

- Five neural decoder architectures: MLP, ResMLP, 3D CNN, GRU and Transformer, benchmarked against classical MWPM decoding.
- Thirty training experiments with reproducible evaluation protocols.
- **20.79% relative reduction in logical error rate (9.07% → 7.18%)** using the Transformer decoder on 90,000 distance-3, 10-round test samples.
- Confidence-aware hybrid decoding combining neural predictions, probability calibration and adaptive MWPM routing.

**Stack:** Python · PyTorch · Stim · PyMatching · NumPy

#### [OptiFactory — Mathematical Optimization for Industrial Production & Machine Scheduling](https://github.com/yingchao-li/OptiFactory-Mathematical-Optimization)

A mathematical optimization framework for **job shop and flexible job shop scheduling (JSSP/FJSP)**, supporting numerical benchmarking and interactive schedule visualization.

- LP relaxation, MILP, CP-SAT, genetic algorithms and simulated annealing; 492 successfully parsed benchmark instances.
- Heuristic-guided hybrid optimization improved feasible-solution coverage from **85.7% to 100%** and proven-optimal coverage from **71.4% to 85.7%**, relative to standard CP-SAT across seven instances under identical two-second configured budgets.
- CP-SAT warm-start optimization achieved a **2.87× geometric-mean speedup** across five matched, proven-optimal benchmark pairs.
- Seventy algorithm–instance evaluations; all 59 returned schedules passed independent constraint validation.

**Stack:** Python · SciPy · HiGHS · OR-Tools · NumPy · pandas · Streamlit

### Applied AI & Digital Transformation

#### [GridPilot — Agentic Engineering Copilot](https://github.com/yingchao-li/GridPilot-Agentic-Engineering-Copilot)

An AI-powered engineering platform integrating **LLMs, hybrid RAG, document intelligence and industrial workflow automation**.

- Engineering document analysis, specification verification and anomaly detection.
- Configurable workflow engine for document review, compliance checks and automated reporting.
- Role-based access control, structured API services and automated software testing.

**Stack:** Python · FastAPI · React · TypeScript · LLMs · RAG · Pytest

#### [UseCasePilot — AI Portfolio Optimization](https://github.com/yingchao-li/UseCasePilot-AI-Portfolio-Optimization)

A decision-support platform for **AI use-case assessment, investment prioritization and digital transformation planning**.

- Structured assessment of business value, implementation feasibility and investment risk.
- AI use-case prioritization, proof-of-concept planning and portfolio evaluation.
- Mathematical decision-support methods and interactive analytical dashboards.

**Stack:** Python · Mathematical Optimization · Data Analytics · React

#### [DeepSeek Multi-Mode Chat](https://github.com/yingchao-li/DeepSeek-Multi-Mode-Chat)

A multilingual AI application for **document RAG, agentic retrieval, academic paper reading and tabular data analysis**.

- Document chunking, embeddings, FAISS retrieval, query rewriting, response generation and verification.
- PDF text and figure extraction, structured paper summaries and document Q&A.
- CSV/Excel analysis, interactive visualization, multi-table joins and machine learning baselines.

**Stack:** Python · Streamlit · FAISS · DeepSeek · Plotly · scikit-learn

### Human Movement & Connected Systems

#### [6-DoF Explorer — Human Movement Exploration Analytics](https://github.com/yingchao-li/6-DoF-Explorer-Human-Movement-Exploration-Analytics)

An interactive scientific analysis platform for **six-degrees-of-freedom motion trajectories and human exploration behaviour**.

- 3D trajectory visualization, quaternion-based orientation analysis, velocity and acceleration estimation.
- Exploration entropy, spatial coverage, density maps and unsupervised clustering.
- DBSCAN, K-Means, PCA, statistical hypothesis testing and numerical result export.

**Stack:** Python · NumPy · SciPy · scikit-learn · Plotly · Streamlit

#### [EV Reservation & Smart Parking Lock](https://github.com/yingchao-li/ev-charging-reservation-v2)

A Munich hackathon prototype connecting **map-based discovery, reservations, driver and operator dashboards, and ECURIOUS parking-lock integration**.

- React/Leaflet interfaces and a FastAPI/SQLite backend for accounts, vehicles, reservations, waitlisting and reallocation.
- REST/SSE integration with plate-based check-in, event deduplication, state synchronization and failure recovery.
- Separate Mock and Live modes; charging, cost and revenue figures are simulated or estimated.

**Validation:** Physical hardware validation remains pending.

**Stack:** React · Leaflet · FastAPI · SQLite · REST · SSE

The [original EV charging prototype](https://github.com/yingchao-li/ev-charging-reservation) validates the reservation-to-release business flow using an explicit Mock API.

## Research

### Master's Thesis Research — Small-Object Detection

Exploring multi-scale feature representations, high-resolution detection layers and coarse-to-fine region refinement for small-object detection.

Research interests include:

- Multi-scale feature learning and feature-pyramid architectures.
- High-resolution feature representations for small and tiny objects.
- Region-of-interest selection and coarse-to-fine detection.
- Accuracy–efficiency trade-offs and reproducible experimental evaluation.

**Status:** Ongoing research; experimental findings are subject to further validation.

### Bachelor's Thesis — Prior-Enhanced Image Restoration

December 2024 – June 2025

Designed **PriAda-U-Net for dehazing** and **GRS-U-Net for deraining**, integrating dark-channel and gradient-map priors. Evaluated adaptive loss weighting through comparative experiments and ablation studies.

Reported dehazing performance: **PSNR 34.13 dB · SSIM 0.8325**.

See my [CV](https://yingchao-li.github.io/assets/Yingchao-Li-CV.pdf) for further context.

## Education & Experience

| Period | Role | Institution / Organization |
| --- | --- | --- |
| Oct 2025 – Present | M.Sc. Data Science | Friedrich-Alexander-Universität Erlangen-Nürnberg |
| Sep 2024 – Mar 2025 | Software Development Intern | Guanghong · Retail business |
| Sep 2021 – Jun 2025 | B.Sc. Computer Science and Technology | China University of Geosciences (Wuhan) |

During my internship, I independently developed and deployed a **WeChat Mini Program** for product browsing and online orders, with a Python backend and AI customer support, and managed testing and maintenance.

## Engineering Principles

- Mathematical understanding before implementation.
- Reproducible experiments and measurable results.
- Modular, maintainable and testable software.
- Transparent validation status and documented limitations.
- Connecting scientific research with practical engineering.

## Get in Touch

Open to working student positions, research collaborations and engineering opportunities in applied AI, scientific computing, computer vision and software development.

- **Email:** [yingchao.li@fau.de](mailto:yingchao.li@fau.de)
- **Portfolio:** [yingchao-li.github.io](https://yingchao-li.github.io/)
- **LinkedIn:** [Yingchao Li](https://www.linkedin.com/in/yingchao-li-722071397/)

---

*Understand the principles. Build the whole system. Validate the results.*
