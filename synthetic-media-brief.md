# Portfolio Project 2: Synthetic Media & Deepfake Biometric Guardrails
**File Name:** synthetic-media-brief.md  
**Target Enterprise:** ZetaMobile Group (Digital Fintech & Mobile Money Operator)  
**System Under Review:** Biometric Facial Recognition & KYC Onboarding Pipeline  
**Frameworks Applied:** CBN Instant Payment Baseline Mandate (July 2026 Update), Nigeria Data Protection Act (NDPA) 2023, ISO/IEC 42001, EU AI Act (Article 50)

---

## 1. Executive Summary & Objective
This framework governs the digital identity and onboarding pipeline of **ZetaMobile Group**, a high-transaction pan-African fintech provider. 

As generative AI models scale globally, automated financial applications face an aggressive, highly sophisticated threat vector: **Synthetic Identity Fraud**. Cybercriminals repurpose open-source Image Translation Algorithms (such as CycleGANs) to clone customer faces and video feeds in real-time. This completely bypasses traditional automated facial authentication checks to execute unauthorized account access and asset draining.

**The Objective:** This project establishes a robust, "Governance-by-Design" technical policy framework. It ensures that ZetaMobile's engineering team moves away from passive, reactive security postures and builds proactive, programmatic validation gates directly into the biometric data ingestion layer to comply with local CBN directives and global data protection standards.

---

## 2. The Technical Risk Profile (The Descriptive "Is")
When a user attempts a high-value transfer or registers a new digital wallet, the mobile application requests a live camera video selfie to match against registered national identity databases (NIN/BVN).

### The Vulnerability Pipeline:
1. **The Ingestion Flaw:** The raw software application logic verifies incoming pixel data solely on static facial geometry matching and contour tracking. 
2. **The Synthetic Exploit:** Bad actors intercept the device's camera feed using automated virtual camera emulators, injecting a real-time, AI-translated deepfake video generated from the victim’s public social media images.
3. **The Result:** The system reads the mathematical facial parameters as a valid match, incorrectly granting access to a synthetic asset, which triggers an automated data breach and immediate asset theft.

---

## 3. The Normative Mandate (The Policy "Ought")
Under the **NDPA 2023**, biometric facial templates are legally classified as *Sensitive Personal Data*, mandating maximum security accountability. 

Furthermore, under the **July 2026 CBN Instant Payment Baseline Mandate**, all licensed payment operators are legally required to deploy verifiable anti-fraud automation. Therefore, ZetaMobile **ought** to treat all incoming media streams as hostile until verified. 

The software **ought** to run programmatic checks to inspect files for structural liveness indicators, cryptographic metadata signatures (C2PA international standards), and frame-rate compression errors before granting access to personal financial dashboards. By building these product-safety gates, the company satisfies global **ISO/IEC 42001** standards and insulates itself from severe regulatory data breach penalties.

