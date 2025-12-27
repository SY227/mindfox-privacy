# MindFox Privacy Policy

**Effective date:** December 27, 2025

This Privacy Policy explains how **MindFox** (“the App”) handles information when you use it. MindFox is designed to keep your thoughts private and **stores your data locally on your device**.

If you have questions, contact: **Simon Yam** — **Simon.Yam227@gmail.com**

---

## Summary (plain English)

- MindFox lets you **record or type** a thought, then uses AI to generate a **summary, tags, action items, and sentiment**.
- Your saved “Memories” and “Digests” are **stored locally on your iPhone/iPad** (in Apple’s on-device app storage).
- When you use AI features, the text of your thought (and selected note summaries for digests) is sent to **Google’s Gemini API** for processing.
- MindFox does **not** create user accounts, does **not** sell your data, and does **not** use ad tracking.

---

## Information the App uses

### 1) Microphone & speech recognition (optional)
If you choose voice capture, MindFox requests access to:
- **Microphone** (to record your speech)
- **Speech Recognition** (to transcribe speech into text)

**What happens to the audio:**  
MindFox uses Apple’s Speech framework to convert speech to text. Depending on your device and iOS settings, speech recognition may be processed **on-device** or may be processed by Apple to return a transcript. MindFox’s AI features use the **transcribed text**, not the raw audio.

### 2) Text you provide (“Thoughts”)
MindFox processes:
- Typed text you enter
- Transcripts produced from your voice capture

This text is used to generate:
- A short **summary**
- **Tags**
- **Action items**
- **Sentiment**
- Optional multi-note **Digests**

### 3) App data stored on your device
MindFox stores the following **locally on your device**:
- Your original transcript/text
- AI-generated summary/tags/action items/sentiment
- Digests you generate (content + key insights)
- Task completion status (done/not done)

This information remains on your device until you delete it in the App or remove the App from your device.

### 4) Diagnostic data
MindFox does not include analytics SDKs. The App may write basic error messages to the device console for debugging.

---

## How AI processing works (Gemini)

When you tap **Capture**, **Re-run AI**, or **Generate Digest**, the App sends the relevant **text** to Google’s Gemini API using the GoogleGenerativeAI SDK.

**Sent to Gemini:**
- For a single thought: the thought transcript/text
- For digests: a list of note summaries/tags within the selected range (or selected notes)

**Not sent to Gemini:**
- Your microphone audio (raw audio is not uploaded by MindFox for AI)
- Your contacts, photos, precise location, or other device data

Google processes the request and returns structured results (JSON) used to populate the App.

**Third-party processing:**  
Your use of Gemini is subject to Google’s applicable terms and privacy policy.

---

## Data sharing

MindFox shares data only in these situations:
1) **AI processing:** text is sent to Google Gemini when you request AI output.
2) **Speech recognition:** speech-to-text is handled by Apple’s Speech framework (processing may be on-device or by Apple depending on configuration).

MindFox does **not** sell your data. MindFox does **not** share data with advertisers. MindFox does **not** perform cross-app tracking.

---

## Data retention & deletion

- **On-device storage:** Your saved notes and digests stay on your device until you delete them inside the App.
- **Deleting in the App:** When you delete a memory, it is removed from local storage.
- **Deleting the App:** Removing the App from your device removes locally stored data in the App sandbox.
- **Third parties:** Text sent to Apple (speech recognition) or Google (Gemini) is handled under their policies.

---

## Security

MindFox uses Apple’s standard app sandboxing. Data is stored in the App’s private container on your device. No method of storage or transmission is 100% secure, but MindFox is designed to minimize data collection and keep your data local by default.

---

## Children’s privacy

MindFox is not directed to children under 13. If you believe a child has provided personal information through the App, contact the email above.

---

## Your choices

- You can use **typing mode** instead of voice capture.
- You can delete individual notes or digests at any time.
- You can avoid AI processing by not using features that call Gemini.

---

## Changes to this policy

We may update this Privacy Policy from time to time. The “Effective date” above will reflect the latest version.

---

## Contact

For questions or requests, contact: **Simon.Yam227@gmail.com**
