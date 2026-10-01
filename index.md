# MindFox Privacy Policy

**Last updated:** September 30, 2026

MindFox (“MindFox,” “we,” “us”) is a local-first thought-capture and organization app. It lets you record or type thoughts, save memories and tasks, optionally use AI to organize saved text, ask questions about your memories, generate reviews, create local reminders, and export or back up your information.

This Privacy Policy explains what information MindFox processes, how it is used, where it is stored, when information may be sent to third parties, and what controls are available to you.

---

## Summary

- Your saved MindFox library is stored locally on your device.
- You can use MindFox without enabling Google AI.
- Voice capture is optional.
- MindFox uses Apple's Speech framework for transcription.
- Apple Speech Recognition and Google Gemini are separate services.
- Raw voice recordings are not sent to Google Gemini.
- Before Google AI is enabled, MindFox presents a disclosure and asks for your permission.
- When AI is enabled, transcript text and relevant saved text may be sent to Google Gemini through Firebase AI Logic.
- Ordinary Memories search is performed locally.
- Sharing a saved range from Digest is prepared locally and does not create a new AI request.
- Mind Packs are prepared locally and are available as Text or Markdown.
- Task reminders are local iOS notifications.
- Standard backups contain saved text/data; audio files are separate.
- MindFox does not require a MindFox account.
- MindFox does not sell personal information.
- MindFox does not use personal information for advertising or cross-app advertising tracking.

---

# Information MindFox processes

## 1) Typed thoughts

You may type a thought directly into MindFox.

Typed content may be stored locally as:

- an unfinished draft;
- an original saved transcript;
- a saved memory;
- task source material;
- AI-generated organization associated with the memory; or
- content included in an export or backup that you deliberately create.

Typing and saving a thought does not require Google AI.

If Google AI is disabled, the thought is saved locally without being sent to Google Gemini.

---

## 2) Microphone and voice recordings

If you choose voice capture, MindFox requests microphone permission.

During voice capture, MindFox records audio and stores recording segments in the app's private local storage.

Recordings have a 20-minute safety limit.

MindFox does not use an always-listening wake word.

A voice capture may also be started or finished through supported Apple system features such as Siri, Shortcuts, or an Action Button shortcut. The same MindFox microphone, transcription, storage, and privacy rules apply.

### Audio retention

Audio retention depends on transcription status and your settings.

If transcription is complete and **Keep audio after transcription** is turned off, MindFox normally removes the completed local audio after the thought has been successfully saved.

If **Keep audio after transcription** is turned on, the recording may remain locally so you can replay or deliberately share it.

Incomplete or interrupted recordings may remain locally so MindFox can attempt transcription recovery.

When you delete an associated memory or use **Delete all data on this device**, MindFox attempts to remove the corresponding locally stored recording.

**Raw voice recordings are not sent to Google Gemini.**

---

## 3) Apple Speech Recognition

MindFox uses Apple's Speech framework to convert recorded speech into transcript text.

Microphone permission and Speech Recognition permission are requested separately.

MindFox provides an **On-device speech only** preference.

When supported by the selected language and device, speech recognition can be required to occur on-device.

If on-device-only recognition is selected and is not supported for that language or device, MindFox does not intentionally fall back to server-based recognition for that request.

If server-based Apple Speech Recognition is used, audio may be transmitted to Apple to perform speech recognition.

Apple's processing and retention of speech-recognition information are governed by Apple's applicable privacy policies and system settings.

Google Gemini is not used to transcribe the original audio.

Apple privacy information:

https://www.apple.com/legal/privacy/

---

## 4) Saved memories

A saved MindFox memory may contain information such as:

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
- people explicitly mentioned;
- topics;
- tags;
- content-tone or sentiment label;
- pinned or favorite status;
- AI-processing state;
- source quotations supporting generated information;
- transcript revision information; and
- recording references when locally retained audio is associated with the memory.

Saved memories are stored locally using Apple's SwiftData framework and related private application storage.

---

## 5) Tasks

MindFox supports manually created tasks and tasks proposed by AI.

Task information may include:

- task text;
- source memory identifier;
- supporting source quotation;
- status such as Open, Later, or Completed;
- priority;
- creation date;
- completion date;
- due date;
- optional time;
- optional reminder time;
- time zone;
- AI-suggested timing words; and
- information indicating whether the task was manually edited.

Creating a task manually does not require Google AI.

AI-generated task proposals are created only when AI processing is enabled.

An AI date suggestion is not automatically scheduled as a reminder.

---

## 6) Digests and AI reviews

MindFox can generate source-grounded reviews from saved memories that you select or from memories within a selected time range.

When you tap **Generate review**, Google AI must be enabled.

For an AI review, MindFox may send relevant information to Google Gemini through Firebase AI Logic, including:

- transcript text or excerpts;
- memory identifiers;
- memory titles;
- capture dates;
- current task text;
- task status;
- due dates;
- completion dates; and
- instructions needed to produce the requested review.

The app may limit the number of memories or excerpt long memories to stay within processing limits.

A generated review may contain:

- themes;
- progress;
- decisions;
- open items;
- possible next steps;
- supporting source references; and
- coverage information.

Generated Digests are stored locally on your device.

---

## 7) Local Digest sharing

Digest also provides a separate **Share** action.

This is different from **Generate review**.

When you use the Digest Share action, MindFox prepares the selected saved thoughts and their current task information locally on your device.

The share can respect:

- the selected Digest time range; and
- specific memories that you deliberately select.

Preparing and opening this local share action does **not** enable Google AI and does **not** create a new Gemini request.

The resulting text is passed to Apple's iOS share sheet only when you choose to share it.

---

## 8) Ask My Mind

Ask My Mind lets you ask questions about saved MindFox memories.

MindFox first ranks candidate memories locally.

When Google AI is enabled and you submit a question, MindFox may send Google Gemini:

- your question;
- relevant transcript text or excerpts;
- memory identifiers;
- memory titles;
- capture dates;
- relevant current task text;
- task status;
- due dates;
- completion dates;
- current date/time; and
- time-zone information.

The AI is instructed to answer from the MindFox source material supplied with the request.

Ask My Mind does not perform a general web search.

---

## 9) Local search and related memories

Ordinary search in Memories is performed locally on your device.

Local search may inspect saved information such as:

- transcript text;
- memory titles;
- current task text;
- tags;
- people;
- topics; and
- saved organized information.

Related-memory suggestions are also determined locally using shared saved people, topics, or tags.

These local operations do not create a Gemini request.

---

# Google AI

## 10) Explicit AI permission

Google AI is optional.

Before automatic AI organization is enabled, MindFox presents an AI and privacy disclosure.

The disclosure explains that:

- transcript text is sent to Google Gemini through Firebase for AI processing;
- the original audio recording is not sent to Gemini;
- Ask My Mind and AI-generated Digests may send relevant saved text and current task information; and
- turning AI off stops future Google AI requests but cannot recall information that was already transmitted.

Opening the disclosure does not by itself enable AI or send a saved thought.

AI is enabled only after you choose **Enable Automatic Organization**.

If you choose **Not Now**, MindFox continues to save and use your thoughts locally without enabling Google AI.

You can change this choice later in **More → AI & privacy**.

---

## 11) Automatic organization

When Google AI is enabled, a newly saved thought may be sent to Google Gemini through Firebase AI Logic for organization.

Information included in an organization request may include:

- original transcript text;
- capture date/time;
- time zone; and
- instructions describing how MindFox should organize the thought.

Gemini may return structured information such as:

- title;
- summary;
- takeaways;
- decisions;
- ideas;
- questions;
- commitments;
- proposed tasks;
- people;
- topics;
- tags; and
- a content-tone label.

MindFox checks AI-provided supporting quotations against the saved transcript before using them as supporting evidence.

AI output may be incorrect.

MindFox preserves your original saved words so you can compare generated information against the source.

---

## 12) Re-running AI after an edit

You may edit a saved transcript.

When the transcript changes, MindFox does not present an older AI interpretation as though it necessarily describes the edited text.

If you later choose **Organize with AI** or **Re-run AI**, the updated transcript may be sent to Gemini in a new request.

---

## 13) Turning AI off

You can turn **Automatic AI organization** off.

Turning AI off:

- stops future MindFox Gemini requests;
- cancels or prevents pending MindFox AI work where possible;
- keeps your saved local memories available; and
- does not recall information already transmitted to Google.

Turning Google AI off does not automatically turn off Apple's Speech Recognition permission.

---

## 14) Information not sent to Gemini

MindFox does not send raw voice recording files to Gemini.

MindFox does not need to send an entire Mind Pack or local Digest Share export to Gemini merely because you export or share it.

Local search does not send a Gemini request.

Manually creating or editing a task does not send a Gemini request.

Preparing a backup does not send a Gemini request.

---

# Local storage

## 15) SwiftData library

MindFox stores memories, tasks, and saved Digests locally using Apple's SwiftData framework.

This may include:

- original transcripts;
- generated organization;
- tasks;
- task states;
- source references;
- saved Digests; and
- related local metadata.

MindFox does not require a separate developer-hosted MindFox user account to access this library.

---

## 16) Local drafts

MindFox keeps unfinished drafts locally so ordinary navigation, keyboard dismissal, or an interruption does not immediately destroy unfinished work.

Local drafts may include:

- an unfinished typed thought;
- unsaved transcript edits; and
- an unfinished manually created task.

These drafts remain in MindFox's private local application storage until saved, cleared, replaced, or deleted.

---

## 17) Local audio storage

Voice recordings are stored separately from the SwiftData text library.

MindFox applies iOS file-protection options to recording files and recording metadata.

Depending on transcription status and your **Keep audio after transcription** preference, audio may be deleted after a successful save or retained for replay, recovery, or deliberate sharing.

---

# Reminders and notifications

## 18) Local task reminders

MindFox can schedule optional task reminders through Apple's local notification system.

Notification permission is requested when you choose to save a reminder and permission has not already been decided.

A local MindFox notification may contain:

- the MindFox app title;
- an internal task identifier used to reopen the applicable task; and
- either generic reminder text or the actual task text.

MindFox provides a **Hide task text in notifications** preference.

When this preference is enabled, MindFox uses generic notification text instead of displaying the task content in the notification body.

MindFox reminders are local notifications.

MindFox does not sync tasks to Apple Reminders.

Nothing is automatically scheduled merely because AI suggested a possible date.

You select and save a reminder yourself.

---

# Exports, backups, and sharing

## 19) Mind Packs

MindFox can create Mind Packs from saved content.

The current app supports:

- **Markdown**; and
- **plain text**.

MindFox does not create PDF Mind Packs in the current version.

Mind Pack ranges include:

- the last 7 days;
- the last 30 days; and
- all time.

A Mind Pack may contain:

- saved summaries;
- decisions;
- ideas;
- questions;
- current task states;
- original transcripts; and
- source information.

Mind Packs are assembled locally on your device from already saved content.

Creating or sharing a Mind Pack does **not** make a new AI request.

Audio files are not included in Mind Packs.

When MindFox creates a temporary local file for the iOS sharing workflow, it attempts to remove that temporary share file after the sharing workflow ends or is cancelled.

---

## 20) Individual sharing, copying, and exporting

You may deliberately:

- share saved text;
- copy saved or generated text to the clipboard;
- export plain text;
- export Markdown; or
- share a locally retained recording.

These operations occur only when you choose them.

Once information is passed to another app, file location, or service that you select, that destination controls its copy according to its own privacy practices.

---

## 21) Full library backup

MindFox can create a restorable JSON backup containing saved library text and data.

A backup may contain:

- memories;
- original transcripts;
- generated organization;
- tasks; and
- saved Digests.

Audio recording files are separate and are not included in the standard text/data backup.

Restorable JSON backups are limited by MindFox to **30 MB**.

MindFox backup and text export files are not password-protected by MindFox.

Store exported files only in locations you trust.

---

## 22) Original-transcript export

MindFox can create a plain-text export containing saved original transcripts.

This export is prepared locally and does not require a Gemini request.

---

## 23) Importing a backup

You may deliberately choose a MindFox JSON backup for import.

MindFox validates the backup before import.

Import is designed to:

- add new memories;
- avoid replacing existing memory IDs;
- reject malformed or conflicting records;
- avoid restoring local recording-file references;
- avoid restoring delayed AI work; and
- avoid automatically scheduling reminders contained in the imported file.

Importing a backup does not create device synchronization.

---

# Retention and deletion

## 24) Local retention

Saved memories, tasks, Digests, drafts, and any retained recordings remain in MindFox's local storage until they are removed according to the app's controls, operating-system behavior, or your settings.

Completed audio may be removed automatically when **Keep audio after transcription** is off.

Exported copies are controlled by the location or service to which you exported them.

---

## 25) Deleting an individual memory

You can delete individual memories.

Deleting a memory is designed to remove:

- that locally stored memory;
- its associated local tasks;
- its associated local reminders;
- associated local recording files; and
- saved Digests that reference the deleted memory.

Previously exported copies are not automatically deleted.

A saved legacy Digest that does not reference the deleted memory may remain.

---

## 26) Deleting tasks and Digests

You can delete tasks and Digests separately.

Deleting a task cancels its associated local MindFox reminder.

Deleting a Digest does not delete its original source memories.

---

## 27) Delete all data on this device

MindFox provides **Delete all data on this device**.

This operation is designed to delete:

- saved memories;
- tasks;
- Digests;
- local drafts;
- local recordings;
- pending and delivered MindFox task notifications; and
- related local MindFox application state.

Deleting local MindFox data does not:

- delete copies you previously exported;
- recall information already transmitted to Google or Apple; or
- delete information retained independently by another service.

---

## 28) Deleting MindFox

Deleting the app removes information stored in MindFox's app container from the device, subject to normal iOS backup, restore, and operating-system behavior.

Deleting MindFox does not automatically delete:

- files you previously exported elsewhere; or
- information independently processed or retained by Apple, Google, or another service.

---

# Third-party processing

## 29) Apple Speech Recognition

Apple provides speech-recognition technology used by MindFox.

When supported on-device recognition is required, speech processing can occur locally.

If Apple server-based recognition is used, audio may be transmitted to Apple for speech recognition.

Apple's independent handling, protection, and retention of that information are governed by Apple's policies.

Apple privacy information:

https://www.apple.com/legal/privacy/

---

## 30) Google Gemini through Firebase AI Logic

MindFox uses Google Gemini through Firebase AI Logic for optional AI functionality.

The current MindFox code uses the Gemini Developer API provider through Firebase AI Logic.

Firebase states that Firebase AI Logic itself does not store customer input and output data sent to and received from the selected generative-AI model provider.

The selected Gemini provider's retention and data-use rules still apply.

Google's data-use and retention practices can depend on the developer project's service tier and configuration.

Google currently documents that:

- Paid Services do not use prompts and responses to improve Google's products;
- prompts and responses may still be retained for limited periods for abuse monitoring;
- Generate Content project logging is separate from abuse-monitoring retention;
- project logging, when enabled for supported requests, has configurable retention; and
- information deliberately placed into saved datasets or other explicitly enabled storage features may follow different retention rules.

MindFox does not control Google's independent retention after information has been transmitted.

MindFox does not itself use your transcript text to train a separate MindFox AI model.

Google information:

https://ai.google.dev/gemini-api/docs/zdr

https://ai.google.dev/gemini-api/docs/logs-policy

https://policies.google.com/privacy

Firebase privacy information:

https://firebase.google.com/support/privacy/

---

## 31) Firebase App Check

MindFox uses Firebase App Check to help protect Firebase-connected AI requests against unauthorized clients.

Production builds use:

- Apple App Attest when supported; or
- Apple DeviceCheck as a fallback.

These services may process technical app/device attestation information and tokens needed to verify that a request originates from an authentic app or supported device.

MindFox does not use these security signals to build a profile of the content of your thoughts.

Firebase's and Apple's independent handling of security and attestation information is governed by their applicable policies.

---

## 32) Apple's iOS sharing and file interfaces

When you deliberately share, export, save, or import information, MindFox may use Apple system interfaces such as:

- the iOS share sheet;
- the Files exporter; or
- the Files importer.

The destination or source you select may be managed by Apple or another third-party service.

MindFox does not control copies of information after you deliberately export or share them outside the app.

---

## 33) Siri and Shortcuts

On supported versions of iOS, MindFox exposes App Intents that can be used through Apple system features such as Siri and Shortcuts to start or finish a recording.

Apple controls the Siri and Shortcuts system environment and may process interaction information under Apple's own privacy practices.

Using these entry points does not change MindFox's treatment of the resulting recording, transcript, or saved memory.

---

## 34) Support email

If you deliberately contact MindFox support, the information you choose to include in your message is processed by the email services involved.

MindFox does not automatically attach your notes or recordings to a support email.

---

# Same or equal protection

Any third party that processes user data for MindFox **provides the same or equal protection of user data** as stated in this policy and as required by Apple's App Review Guidelines.

MindFox shares information with third parties only for the functions described in this policy and subject to the choices and permissions described above.

---

# What MindFox does not do

MindFox does not:

- require a MindFox user account;
- sell your personal information;
- share your information with advertising networks for targeted advertising;
- perform cross-app advertising tracking;
- send raw voice recording files to Google Gemini;
- automatically schedule reminders from an AI suggestion;
- sync tasks with Apple Reminders;
- perform a general web search for ordinary Memories search;
- perform a general web search for Ask My Mind;
- make a new Gemini request merely because you share a Digest range;
- make a new Gemini request merely because you create a Mind Pack;
- require Google AI to type and save a thought;
- require Google AI to read or locally search your memories;
- require Google AI to manually create or edit tasks;
- require Google AI to create a local export or backup; or
- automatically attach your memories or recordings to support messages.

---

# Security

MindFox is designed around local storage and user-controlled processing.

MindFox uses Apple's application sandbox and iOS file-protection mechanisms for applicable local files.

MindFox uses Firebase App Check with Apple App Attest or DeviceCheck to help protect Firebase-connected AI requests.

Exported files and standard MindFox backups are not password-protected by MindFox.

Once you export or share information, protect the destination appropriately.

No storage or transmission method can be guaranteed to be completely secure.

---

# Your choices

You can:

- type instead of recording;
- deny or revoke microphone permission;
- deny or revoke Speech Recognition permission;
- select **On-device speech only** where supported;
- choose whether completed recordings are retained;
- keep Google AI disabled;
- turn automatic AI organization off;
- choose whether to organize an older or edited memory with AI;
- choose whether to use Ask My Mind;
- choose whether to generate an AI Digest review;
- share a saved Digest range locally without generating an AI review;
- manually add or edit tasks without AI;
- choose whether to create a reminder;
- hide task text in notifications;
- delete individual memories;
- delete tasks;
- delete Digests;
- export your saved information;
- create a backup;
- use **Delete all data on this device**; and
- control relevant permissions through iOS Settings.

Turning AI off stops future MindFox Gemini requests but cannot recall information already transmitted to Google.

Revoking Speech Recognition permission affects future speech-recognition requests but does not recall information already processed by Apple.

---

# Children’s privacy

MindFox is not directed to children under 13.

We do not knowingly collect personal information from children under 13.

---

# Changes to this policy

We may update this Privacy Policy from time to time.

The **Last updated** date above reflects the latest version.

---

# Contact

For questions or privacy requests regarding MindFox, contact:

**Simon Yam**

**Email:** Simon.Yam227@gmail.com
