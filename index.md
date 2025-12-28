# MindFox Privacy Policy

**Effective date:** December 28, 2025

This Privacy Policy explains how **MindFox** (“the App”) handles information when you use it. MindFox is designed to keep your thoughts private and **stores your data locally on your device by default**.

If you have questions, contact: **Simon Yam** — **Simon.Yam227@gmail.com**

---

## Summary (plain English)

- MindFox lets you **record or type** a thought, then uses AI to generate a **summary, tags, action items, and sentiment**.
- Your saved notes (“Memories”) and “Digests” are **stored locally on your iPhone/iPad** (in Apple’s on-device app storage).
- When you use AI features, the text you submit (and the model’s output) is sent to **Google’s Gemini API** for processing.
- MindFox does **not** create user accounts, does **not** sell your data, and does **not** use ad tracking.

---

## Information MindFox uses

### 1) Microphone & speech recognition (optional)
If you choose voice capture, MindFox requests access to:
- **Microphone** (to record your speech)
- **Speech Recognition** (to transcribe speech into text)

MindFox uses Apple’s Speech framework to convert speech to text. Depending on your device and iOS settings, speech recognition may be processed **on-device** or may be processed by Apple to return a transcript. MindFox’s AI features use the **transcribed text**, not the raw audio.

### 2) Text you provide (“Thoughts”)
MindFox processes:
- Typed text you enter
- Transcripts produced from voice capture

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

### 4) Diagnostics
MindFox does not include third-party analytics SDKs. The App may write basic error messages to the device console for debugging.

---

## How AI processing works (Google Gemini)

When you tap **Capture**, **Re-run AI**, or **Generate Digest**, MindFox sends the relevant **text** to Google’s Gemini API using the GoogleGenerativeAI SDK.

**Sent to Gemini:**
- For a single thought: the thought transcript/text
- For digests: a list of note summaries/tags within the selected range (or selected notes)

**Not sent to Gemini:**
- Your microphone audio (raw audio is not uploaded by MindFox for AI)
- Your contacts, photos, precise location, or other device data

### Gemini retention (55 days)
When you use AI features, the text you submit (prompts/context) and the model’s output **may be retained by Google for up to 55 days** for abuse monitoring and policy enforcement, per Gemini API policies.  
References:
- https://ai.google.dev/gemini-api/docs/usage-policies
- https://ai.google.dev/gemini-api/docs/logs-policy

Your use of Gemini is also subject to Google’s terms and privacy policy:
- https://policies.google.com/privacy

---

## Data sharing

MindFox shares data only in these situations:
1) **AI processing:** text is sent to Google Gemini when you request AI output (and may be retained by Google as described above).
2) **Speech recognition:** speech-to-text is handled by Apple’s Speech framework (processing may be on-device or by Apple depending on configuration).

MindFox does **not** sell your data. MindFox does **not** share data with advertisers. MindFox does **not** perform cross-app tracking.

---

## Data retention & deletion

### On-device retention (MindFox)
- **On-device storage:** Your saved notes and digests stay on your device until you delete them inside the App.
- **Deleting in the App:** When you delete a memory or digest, it is removed from local storage.
- **Deleting the App:** Removing the App from your device removes locally stored data in the App sandbox.

### Third-party retention (Apple / Google)
- **Google Gemini:** may retain prompts/context/output for up to **55 days** for abuse monitoring (see links above).
- **Apple Speech:** speech recognition may be processed on-device or by Apple depending on device settings. For Apple’s disclosure about Siri/Dictation processing and retention, see:
  - https://www.apple.com/legal/privacy/data/en/ask-siri-dictation/
  - https://www.apple.com/legal/privacy/data/en/improve-siri-dictation/

---

## Revoke consent & request deletion

### Revoke consent (stop off-device processing)
You can stop off-device AI processing at any time by:
- **Not using** AI-triggering actions (**Capture**, **Re-run AI**, **Generate Digest**).
- Using **typing** without voice capture (voice is optional).
- Disabling permissions in iOS Settings:
  - **Settings → Privacy & Security → Microphone** (turn off for MindFox)
  - **Settings → Privacy & Security → Speech Recognition** (turn off for MindFox)

### Request deletion
- **MindFox can delete on-device data**: delete notes/digests in the App, or delete the App to remove local storage.
- **Third-party deletion requests**: MindFox cannot directly delete data that Apple or Google may retain as part of speech recognition or AI processing. Requests are governed by their policies:
  - Apple: https://www.apple.com/legal/privacy/
  - Google: https://policies.google.com/privacy

---

## Security

MindFox uses Apple’s standard app sandboxing. Data is stored in the App’s private container on your device. No method of storage or transmission is 100% secure, but MindFox is designed to minimize data collection and keep your data local by default.

---

## Children’s privacy

MindFox is not directed to children under 13.

---

## Changes to this policy

We may update this Privacy Policy from time to time. The “Effective date” above will reflect the latest version.

---

## Contact

For questions or requests, contact: **Simon.Yam227@gmail.com**
