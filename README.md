# Janani-Setu

## The Problem
Maternal and infant health outcomes in rural India remain a critical challenge. Millions of pregnant women lack consistent access to basic prenatal care, nutritional guidance, and emergency diagnostics due to isolated geography, severe shortage of specialist doctors, and unreliable infrastructure. Furthermore, frontline health workers (ASHA workers) are overburdened, under-equipped, and reliant on manual paper-based tracking, which often leads to delayed interventions in life-threatening pregnancy complications.

## Our Solution
**Janani-Setu (Maa App)** is an offline-first, AI-powered maternal health ecosystem built explicitly for the realities of rural India. It acts as an intelligent bridge ("Setu") between pregnant mothers, ASHA workers, and healthcare infrastructure. By providing predictive risk analysis, real-time nutritional diagnostics, and actionable health insights directly on mobile devices, Janani-Setu democratizes life-saving maternal care.

## Core Features
- **Offline-First AI Diagnostics:** Rule-based and on-device machine learning models for early detection of complications, such as automated swelling/edema checks and gestational diabetes risk assessments.
- **On-Device Food & Nutrition Analysis:** Real-time dietary scanning and nutritional tracking using an optimized AI pipeline and local file-system caching, delivering immediate feedback.
- **ASHA Multi-Modal Field Notebook:** Voice-to-text transcription, local OCR for medical documents, and context-aware report generation to drastically reduce the administrative burden on health workers.
- **Predictive Risk Dashboard:** Advanced risk assessment engine that synthesizes patient data and flags high-risk pregnancies, enabling doctors and supervisors to proactively direct ASHA interventions.
- **Interactive Pregnancy Education:** Highly accessible learning modules, including 3D fetal models, baby care guides, and danger sign alerts, delivered in local languages.
- **Smart SOS & Emergency Routing:** One-tap offline emergency alerts and smart route mapping to the nearest available healthcare facility.

## Built for Rural India: Low-End Hardware & Zero Connectivity
Janani-Setu is engineered specifically to conquer the technological constraints of rural deployments:
- **Zero Internet Dependency:** The core experience—including visual diagnostics, clinical risk assessments, and educational content—runs entirely **offline**. By leveraging an advanced local caching architecture, the app functions flawlessly in dead zones. Data seamlessly, asynchronously syncs in the background only when a connection is briefly established.
- **Optimized for Low-Grade Phones:** We utilize highly compressed, quantized local models and single-pass processing pipelines. The application avoids heavy CPU overhead and memory leaks, ensuring it runs smoothly on older, low-memory Android devices without aggressively draining the battery.
- **Accessible to All Literacy Levels:** Utilizing voice-first interfaces, text-to-speech services, and intuitive visual indicators (like color-coded health scores), the platform ensures that users of all literacy, language, and education levels can benefit effortlessly.

## Business Model & Scalability (< $1 per User)
To serve the bottom of the pyramid, Janani-Setu operates on a highly frugal B2G (Business-to-Government) and B2NGO model, structurally designed to cost **less than $1 per user per year**:
- **Edge AI Eliminates Cloud Costs:** By shifting 90% of processing—computer vision, risk calculations, and language processing—directly onto the user's smartphone hardware, we completely bypass expensive cloud compute costs and API quotas.
- **Micro-Data Syncing:** By utilizing deferred batch processing and aggressive local data compression, our cloud sync payloads are incredibly lightweight (mere kilobytes), minimizing bandwidth and backend database operational costs.
- **Leveraging Existing Infrastructure:** We deploy via existing ASHA worker smartphone networks, meaning there are zero hardware distribution costs.
- **Economies of Scale:** At scale, backend infrastructure is strictly relegated to lightweight data aggregations for the risk dashboard. The cost of adding a new user approaches zero, enabling state-wide deployments with minimal financial friction.
