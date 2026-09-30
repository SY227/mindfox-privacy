# MindFox Privacy Policy

**Last updated:** September 30, 2026

MindFox (“MindFox”, “we”, “us”) is a local-first thought-capture and organization app that lets users record or type thoughts, keep memories and tasks, optionally use AI to organize saved text, generate reviews, ask questions about saved memories, set local task reminders, and export or back up their data.

This policy explains what data MindFox processes, how it is used, where it is stored, when information is sent to third parties, and the choices available to you.

---

## Summary

- **Your library is stored on your device.** MindFox stores saved thoughts, transcripts, AI-generated organization, tasks, digests, drafts, and preferences in the app's local storage.
- **Voice capture is optional.** MindFox uses the microphone and Apple Speech Recognition to create transcripts.
- **Speech Recognition and Google AI are separate.** Apple may process speech when server-based speech recognition is required. Google Gemini receives transcript text only when you have enabled MindFox AI.
- **Audio is not sent to Gemini.**
- **Google AI is optional.** MindFox asks for permission before enabling automatic AI organization.
- **Turning AI off stops future Google AI requests.** Your locally saved thoughts remain available.
- **Ask My Mind and Digest use relevant saved text and task context.**
- **Local search does not use AI or web search.**
- **Task reminders are local iOS notifications.**
- **Mind Packs and backups are prepared on your device.**
- **MindFox does not require a MindFox account.**
- **No advertising, no sale of personal data, and no cross-app advertising tracking.**

---

## Data MindFox processes

### 1) Typed thoughts

You may type a thought directly into MindFox.

Typed content may be stored locally as:

- a temporary draft before you save;
- an original saved transcript;
- a memory;
- task source material; or
- part of a locally created export or backup.

Typing and saving a thought does not require Google AI.

If Google AI is disabled, the thought is saved locally without being sent to Google.

---

### 2) Microphone and voice recordings

If you choose voice capture, MindFox requests microphone permission.

During voice capture, MindFox records audio and stores recording segments in its private application storage.

Recordings have a 20-minute safety limit.

Audio may be retained differently depending on the recording state and your settings:

- if transcription is complete and **Keep audio after transcription** is off, MindFox normally removes the completed local audio after the thought is saved;
- if **Keep audio after transcription** is on, the recording may remain locally so you can replay or share it;
- incomplete or interrupted recordings may be retained locally so transcription recovery can be attempted; and
- deleting the associated memory or using **Delete all data** also attempts to remove its locally stored recording.

**MindFox does not send the raw audio recording to Google Gemini.**

---

### 3) Apple Speech Recognition

MindFox uses Apple's Speech framework to convert recorded speech into transcript text.

MindFox requests Speech Recognition permission separately from microphone permission.

When supported by the selected language and device, MindFox requests on-device speech recognition.

MindFox also provides an **On-device speech only** preference. If you require on-device-only recognition and the selected recognizer does not support it, MindFox does not intentionally fall back to server-based speech recognition for that capture.

When server-based Apple Speech Recognition is used, recorded speech may be transmitted to Apple for transcription.

Apple's processing and retention of speech-recognition data are governed by Apple's applicable privacy policies and system settings.

Google Gemini is not used to transcribe the audio.

---

### 4) Saved memories

A saved MindFox memory may contain:

- original typed text or voice transcript;
- creation date and time;
- time-zone information;
- title;
- summary;
- takeaways;
- decisions;
- ideas;
- questions;
- commitments;
- people or topics mentioned;
- tags;
- sentiment label;
- pinned or favorite status;
- AI-processing state;
- source quotations used to support AI output;
- recording reference information when local audio is retained; and
- information needed to identify whether an AI interpretation still corresponds to the current transcript.

MindFox stores this information locally using Apple's SwiftData framework and related local application storage.

---

### 5) Tasks

Tasks may be:

- manually created by you; or
- proposed by AI from a saved thought.

Task information may include:

- task text;
- source memory identifier;
- supporting source quotation;
- open, later, or completed status;
- priority;
- creation date;
- completion date;
- due date;
- optional due-time information;
- optional reminder time;
- time zone;
- AI-suggested timing words; and
- information showing whether the task was manually edited.

Manually adding or editing a task does not itself require Google AI.

AI-created tasks are generated only when AI processing has been enabled.

---

### 6) Digests and reviews

MindFox can create source-grounded reviews from selected saved memories.

When AI review is requested and Google AI is enabled, MindFox may send relevant saved information to Google Gemini, including:

- transcript text or excerpts;
- memory identifiers;
- memory titles;
- capture dates;
- relevant current task text;
- task status;
- due dates;
- completion dates; and
- instructions for producing the requested review.

The app may limit or excerpt source material to fit processing limits.

Generated reviews may contain themes, progress, decisions, open items, possible next steps, source references, and coverage information.

Saved Digests are stored locally.

---

### 7) Ask My Mind

Ask My Mind lets you ask questions about your saved MindFox memories.

MindFox first selects relevant candidate memories from your local library.

When Google AI is enabled and you submit an Ask My Mind question, MindFox may send to Google Gemini:

- your question;
- relevant saved transcript text or excerpts;
- memory identifiers;
- memory titles;
- capture dates;
- relevant task text;
- task status;
- due dates;
- completion dates;
- current date/time; and
- time-zone information.

The model is instructed to answer only from supplied MindFox source material.

MindFox does not perform a general web search for Ask My Mind.

---

### 8) Local search and related-memory suggestions

Ordinary Memories search is performed locally on the device.

Search may inspect locally stored information such as:

- original transcript text;
- titles;
- current task text;
- saved tags;
- saved people;
- saved topics; and
- current AI-generated memory information.

Related-memory suggestions are also calculated locally from shared saved people, topics, or tags.

These local search and related-memory operations do not create a new Gemini request.

---

## Google Gemini and Firebase AI Logic

### 9) Explicit AI permission

Google AI is optional.

Before automatic AI organization is enabled, MindFox presents an AI and privacy disclosure.

The disclosure explains that:

- transcript text is sent to Google Gemini through Firebase;
- audio is not sent to Gemini;
- Ask My Mind and Digest may send relevant saved text and current task information; and
- disabling AI stops future AI requests but cannot recall information already transmitted.

Only after you choose **Enable Automatic Organization** is automatic AI processing enabled.

If AI is not enabled, new thoughts remain usable as local memories without Google AI.

---

### 10) Automatic organization

When AI is enabled, a newly saved thought may be sent to Google Gemini through Firebase AI Logic for organization.

Information sent may include:

- the original transcript text;
- capture date/time;
- time zone; and
- instructions describing how the thought should be organized.

Gemini may return:

- title;
- summary;
- key takeaways;
- decisions;
- ideas;
- questions;
- commitments;
- proposed tasks;
- people;
- topics;
- tags; and
- a content-tone label.

MindFox validates AI-provided source quotations against the locally stored transcript before presenting supported evidence.

AI output can be incorrect. MindFox preserves the original transcript so you can compare generated information with your own words.

---

### 11) Re-running AI after transcript edits

You can edit an original transcript.

When a transcript changes, MindFox does not present an older AI interpretation as though it necessarily describes the new text.

If you choose **Re-run AI** or **Organize with AI**, the current saved transcript may be sent to Gemini again.

---

### 12) Information not sent to Gemini

MindFox does **not** send the original voice audio file to Gemini.

MindFox also does not need to send an entire export file or Mind Pack to Gemini simply because you export or share it.

Mind Packs are assembled locally from already saved content and do not make a new AI request.

---

## Local storage

### 13) SwiftData library

MindFox stores memories, tasks, and digests in local SwiftData storage.

This includes:

- original transcripts;
- AI-generated organization;
- tasks;
- task state;
- source references;
- digests; and
- related metadata.

MindFox does not require a separate MindFox login or developer-hosted user account to access the local library.

---

### 14) Drafts

MindFox keeps unfinished text and editing drafts locally so that accidental navigation, keyboard dismissal, or app interruption does not immediately discard your work.

Drafts may include:

- an unfinished typed capture;
- unsaved transcript edits; and
- unfinished manually entered tasks.

Draft files are stored in MindFox's local application storage.

---

### 15) Local audio storage

Voice recordings are stored separately from the SwiftData text library.

MindFox uses iOS file-protection options for local recording files and recording metadata.

Depending on your settings and transcription status, audio may be deleted after a successful save or retained for replay, recovery, or manual sharing.

---

## Reminders and notifications

### 16) Task reminders

MindFox can schedule optional task reminders using Apple's local notification system.

MindFox requests notification permission when you choose to save a reminder.

A reminder may include:

- a MindFox notification title;
- the task identifier used to open the correct saved task; and
- either generic reminder text or the task text, depending on your notification privacy preference.

By default, MindFox provides a **Hide task text in notifications** privacy preference.

When that preference is enabled, the notification body uses generic text rather than displaying the task itself.

Reminders are local iOS notifications.

MindFox does not sync tasks with Apple Reminders.

No task reminder is created merely because AI suggested a date. You choose and save reminder timing yourself.

---

## Exports, backups, and sharing

### 17) Mind Packs

MindFox can create Mind Pack documents in:

- PDF;
- Markdown; or
- plain text.

A Mind Pack may contain:

- saved summaries;
- decisions;
- ideas;
- questions;
- current task states;
- original transcripts; and
- source information.

Mind Packs are assembled on your device from saved content.

Creating a Mind Pack does not make a new Gemini request.

Audio files are not embedded in Mind Packs.

Temporary files used for iOS sharing are removed by MindFox after the applicable share workflow is finished where supported.

---

### 18) Individual exports and copying

You may deliberately:

- share saved text;
- copy generated or saved text to the clipboard;
- export text;
- export Markdown; or
- share locally retained recording audio.

These actions occur only when you choose them.

A destination app or service selected through iOS may retain the information according to its own privacy policy.

---

### 19) Full library backup

MindFox provides a restorable JSON backup containing text/data from the local library.

A backup may include:

- memories;
- original transcripts;
- AI-generated memory information;
- tasks; and
- digests.

Audio files are separate and are **not included** in the standard text/data backup.

Restorable JSON backups are limited by the app to **30 MB**.

MindFox backup and text-export files are **not password-protected by MindFox**.

Store exported files only in locations you trust.

---

### 20) Original-transcript export

MindFox can create a plain-text export containing all saved original transcripts.

This export is assembled locally and does not require AI processing.

---

### 21) Importing a backup

You may select a MindFox JSON backup for import.

MindFox validates the backup before importing it.

Import is designed to:

- add new memories;
- avoid replacing existing memory IDs;
- reject certain conflicting or malformed records;
- avoid restoring local audio-file references; and
- avoid automatically scheduling reminders contained in an imported file.

Importing a backup does not create device synchronization.

---

## Delete and retention controls

### 22) Delete individual memories

You can delete individual memories from MindFox.

Deleting a memory also removes associated local tasks and reminders and may remove saved digests that explicitly reference that memory.

Previously exported copies are not automatically deleted.

Older unlinked digest records may remain when they do not reference the deleted memory.

If a local recording belongs to the deleted memory, MindFox attempts to remove the recording as part of the deletion process.

---

### 23) Delete individual tasks and digests

You can delete tasks and digests separately.

Deleting a task cancels its local notification reminder.

Deleting a digest does not delete the original memories used to create it.

---

### 24) Delete all MindFox data

MindFox provides **Delete all data on this device**.

This operation is designed to delete:

- memories;
- tasks;
- digests;
- local drafts;
- local recordings;
- local task notifications; and
- related local application state.

Deleting local MindFox data does not:

- delete copies you previously exported;
- recall information already transmitted to Google or Apple;
- delete information retained independently by third-party processors; or
- cancel an Apple subscription.

---

### 25) Deleting the app

Deleting MindFox removes data stored in the app's local container from the device, subject to normal iOS device-backup and restore behavior.

Deleting the app does not automatically delete:

- files you exported elsewhere;
- information independently retained by Apple or Google; or
- an active App Store subscription.

---

## Third-party processing

### 26) Apple Speech Recognition

Apple provides speech-recognition services used to create voice transcripts.

When supported on-device recognition is used, speech processing can occur locally.

When server-based recognition is used, audio may be transmitted to Apple for processing.

Apple's independent handling and retention of this information is governed by Apple's applicable policies and settings.

---

### 27) Google Gemini through Firebase AI Logic

MindFox uses Google Gemini through Firebase AI Logic for optional AI functionality.

Firebase AI Logic provides the connection between MindFox and the configured Gemini provider.

Firebase states that Firebase AI Logic itself does not store the customer input and output sent to and received from the selected generative AI provider. The provider's own retention and data-use policies apply.

MindFox currently uses the Gemini Developer API backend.

Google's data-use and retention terms can vary based on the developer project's service tier and configuration.

Google currently states that:

- for **Paid Services**, prompts and responses are not used to improve Google's products;
- Paid Services may retain prompts and responses for a limited period for abuse monitoring;
- developer project logging for Generate Content requests is not enabled automatically merely to view logs;
- when Gemini project logging is enabled, Google currently documents a default maximum log-retention period of **55 days**, configurable to 7, 14, 28, or 55 days;
- saved datasets or other explicitly enabled storage features may have different retention; and
- under applicable **Unpaid Services** terms, submitted content and generated responses may be used by Google to provide, improve, and develop its products and machine-learning technologies.

MindFox does not itself use your transcript text to train its own AI model.

Google's independent processing, security, abuse-prevention, logging, retention, and model-improvement practices are governed by Google's applicable terms and project configuration.

---

### 28) Firebase App Check

MindFox uses Firebase App Check to help protect Firebase-connected AI requests from unauthorized clients.

Production builds use:

- Apple App Attest when supported; or
- Apple DeviceCheck as a fallback.

App Check may process technical information including:

- app attestation information;
- App Check tokens;
- device/app integrity signals; and
- information required to verify that a request originates from an authentic app or supported device.

This security information is not used by MindFox to build a profile of your thoughts.

Firebase's and Apple's independent handling of attestation information is governed by their applicable policies.

---

### 29) Apple StoreKit

MindFox offers optional MindFox Pro subscriptions through Apple StoreKit.

MindFox may request StoreKit information needed to:

- display available subscription plans and prices;
- determine introductory-offer eligibility;
- verify active entitlements;
- process a user-initiated purchase;
- restore purchases; and
- open Apple's subscription-management interface.

Apple processes payment and Apple Account information.

MindFox does not receive your full payment-card details.

Deleting MindFox does not cancel an Apple subscription. Subscription management and cancellation are handled through Apple.

---

### 30) iOS Share Sheet and Files

When you deliberately export, share, or save MindFox information, Apple's sharing or file-selection interfaces may be used.

The external destination you select controls any copy stored outside MindFox.

MindFox cannot automatically delete a file after you have saved or shared it to another service.

---

### 31) Support email

If you deliberately contact MindFox support, your email provider and the receiving email service process the information you choose to send.

MindFox does not automatically attach notes or recordings to a support email.

---

## Same or equal protection

Any third party that processes user data for MindFox **provides the same or equal protection of user data** as stated in this policy and as required by Apple's App Review Guidelines.

MindFox shares information with third parties only for the functionality described in this policy and subject to the choices and permissions described above.

---

## What MindFox does not do

MindFox does not:

- require a MindFox user account;
- sell your personal data;
- share your personal data with advertising networks;
- perform cross-app advertising tracking;
- send raw voice recordings to Gemini;
- automatically create reminders from AI suggestions;
- sync tasks to Apple Reminders;
- perform a web search for ordinary library search or Ask My Mind;
- automatically attach your memories or recordings to support messages; or
- require Google AI in order to type, save, read, search, manually organize, manually create tasks, export original text, or delete your locally stored data.

---

## Security

MindFox is designed around local storage and user-controlled processing.

The app uses Apple's application sandbox and iOS file-protection mechanisms for applicable local files.

MindFox uses Firebase App Check with Apple App Attest or DeviceCheck to help protect Firebase-connected AI requests.

Exported files and standard MindFox backup files are not password-protected by MindFox. Once you export or share information, protect the destination appropriately.

No method of storage or network transmission can be guaranteed to be completely secure.

---

## Your choices

You can:

- type instead of recording;
- deny or revoke microphone permission;
- deny or revoke Speech Recognition permission;
- enable **On-device speech only** where supported;
- choose whether completed audio is retained;
- keep Google AI disabled;
- turn automatic AI organization off at any time;
- choose whether to organize an older memory with AI;
- choose whether to ask a question or generate a review;
- manually add tasks without AI;
- choose whether to create a reminder;
- hide task text in notifications;
- delete individual memories, tasks, or digests;
- use **Delete all data on this device**;
- export a backup before deletion; and
- manage or cancel MindFox Pro through Apple.

Turning AI off affects future AI requests. It cannot recall information already transmitted to Google.

Revoking Apple Speech permission affects future speech-recognition requests. It does not recall information already processed by Apple.

---

## Children’s privacy

MindFox is not directed to children under 13, and we do not knowingly collect personal information from children under 13.

---

## Changes to this policy

We may update this Privacy Policy from time to time.

The **Last updated** date above reflects the latest version.

---

## Contact

For questions or privacy requests regarding MindFox, contact:

**Email:** Simon.Yam227@gmail.com
