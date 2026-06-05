# SoftVault 🛡️ — Media Authenticity & Ownership Protection

SoftVault is a security-first platform designed to protect digital creators by proving content origin and detecting unauthorized re-distribution. By combining **Google's Gemini AI** for forensic analysis with **Cryptographic Hash Chains** for provenance, SoftVault ensures your digital assets remain uniquely yours.

---

## 🚀 The SoftVault Workflow

SoftVault follows a structured security protocol to ensure every piece of media is analyzed, anchored, and monitored.

### 1. Media Ingestion & Neural Sweep
When you upload an image, the platform initiates a technical deconstruction:
- **Neural Forensic Analysis**: Powered by **Gemini 1.5 Flash**, the system inspects the image for signs of AI generation, digital tampering, or pixel-level manipulation.
- **Metadata Harvesting**: Extracts deep EXIF data (Camera model, GPS, software used, timestamps) to build a "DNA" profile of the media.

### 2. Verification & Verdict
You are presented with a **Neural Validation Report**:
- **Integrity Coefficient**: A percentage score representing the AI's confidence in the content's authenticity.
- **Scene Semantics**: Detailed AI-generated description of objects and context used for cross-registry searching.

### 3. Cryptographic Anchoring
Once verified, the media is finalized through a three-tier hashing process:
- **SHA-256 Fingerprint**: A unique cryptographic ID based on the file's raw data.
- **Perceptual Hash (pHash)**: A visual fingerprint that allows the system to recognize the image even if it has been resized or compressed.
- **Hash Chaining**: Each registration is linked to the previous record in the global registry (similar to a blockchain), creating an immutable history of provenance.

### 4. Sentinel Surveillance (Theft Detection)
The "Surveillance" portal allows you to scan any public media fragment:
- **Collision Detection**: The platform cross-references the scanned file against its global database.
- **Conflict Identification**: If a similar pHash or visual label set is found, the system flags the collision, identifying potential theft or unauthorized re-uploads.

### 5. Secure Governance & Transfer
- **Digital Vault**: Manage all your anchored assets in a central, encrypted dashboard.
- **Asset Transfer**: Safely move ownership of an asset to another node (user) using a cryptographic handshake, updating the provenance chain instantly.

---

## 🛠️ Technical Architecture

- **Neural Engine**: `gemini-3-flash-preview` — Provides high-speed visual reasoning and forensic analysis.
- **Frontend Stack**: 
  - **React 18** with **Vite** for high-performance rendering.
  - **Tailwind CSS** for a "Brutalist Security" aesthetic.
  - **Framer Motion** for tactical interface animations.
- **Backend Infrastructure**: 
  - **Cloud Firestore**: Stores the anchored provenance chain.
  - **Firebase Auth**: Secure Google-node authentication.
- **Crypto Library**: Custom implementation of SHA-256 and perceptual hashing.

---


## Run Locally

### Prerequisites

Make sure you have **Node.js** installed (v16 or above recommended).

---

### Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/Abhishek-x23/SoftVault.git
   cd SoftVault
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment variables**

   Create a `.env` file in the root directory and add:

   ```bash
   VITE_FIREBASE_API_KEY=your_firebase_api_key
   VITE_GEMINI_API_KEY=your_gemini_api_key
   GEMINI_API_KEY=your_gemini_api_key
   ```

   > You can refer to `.env.example` for the required format.

4. **Run the development server**

   ```bash
   npm run dev
   ```

5. Open your browser and go to:

   ```
   http://localhost:3000
   ```

   (or the port shown in your terminal)

---

### Notes

* Make sure your Firebase project is properly configured.
* Add `localhost` to **Authorized Domains** in Firebase Authentication settings.
* Never commit your `.env` file.
