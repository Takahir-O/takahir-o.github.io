---
layout: ../../layouts/BaseLayout.astro
title: KoeKey - Privacy Policy
description: KoeKey Privacy Policy
---

# KoeKey Privacy Policy

Last updated: 2026-03-29

> [日本語版はこちら](/koekey/privacy-policy-ja)

## Overview

KoeKey is a voice dictation application that converts speech to text. This policy explains what personal information KoeKey accesses, collects, or transmits, how it is used, stored, and secured, and what controls you have over your data.

## How KoeKey Processes Your Voice

### Local Processing (Whisper / sherpa-onnx)

When you use a local speech recognition model (Whisper or sherpa-onnx), **all audio processing happens entirely on your device**. No audio data leaves your device. KoeKey does not collect, transmit, or have access to your voice data in this mode.

### Cloud Processing (Soniox, Deepgram)

When you choose to use a cloud speech-to-text provider, your audio is streamed to the selected provider over a TLS encrypted connection. Audio is sent only while you are actively dictating.

- **No audio is sent to any cloud provider until you provide and configure an API key.** The app cannot transmit audio without a valid key.
- KoeKey does not store or retain your audio recordings. Audio is held in memory only during the active dictation session and is discarded afterward.
- Your audio data is **not used for AI training** by KoeKey.

## What Data We Store

### API Keys

If you use cloud providers, you provide your own API keys. These are stored using your operating system's native secure credential store (Windows Credential Manager on Windows, Keychain on macOS). KoeKey never transmits your API keys to any server other than the speech-to-text provider you selected.

### Transcription History

Your transcription history is encrypted with AES-256-GCM and stored locally on your device. The encryption key is kept in your operating system's secure credential store. History data is never sent to any external server.

### File Output

When you use features that save transcription results to files (such as voice memos or listening output), these files are stored in plaintext at locations you choose on your device. These files are not encrypted and are not automatically deleted.

### Screenshots

If you enable the optional screenshot feature, KoeKey captures an image of the active window during dictation and saves it to a directory you specify. Screenshots are stored locally and are not transmitted to any server. This feature is disabled by default.

### Clipboard

KoeKey uses the system clipboard to insert transcription results into the active application via paste (Ctrl+V / Cmd+V). By default, the original clipboard contents are restored after insertion. You can change this behavior in settings to keep the transcription text in the clipboard instead.

### In-App Purchases

KoeKey uses the platform's native store (Microsoft Store on Windows, App Store on macOS) for in-app purchases. Purchase transactions are handled entirely by the platform. KoeKey does not collect or process any payment information.

### Telemetry and Analytics

KoeKey does **not** collect any telemetry, analytics, crash reports, or usage data. No information about how you use the app is sent to the developer or any third party.

## How We Protect Your Data

- Audio transmission to cloud providers uses TLS encryption.
- API keys are stored in OS-level secure credential stores with automatic cache expiration.
- Transcription history is encrypted with AES-256-GCM.
- No data is stored on external servers controlled by KoeKey.
- KoeKey employs the above measures, in line with current security standards, to protect your data. Please note that no software can guarantee absolute security.

## Third-Party Services

KoeKey connects to the following third-party services depending on your usage:

### Cloud Speech-to-Text (user-initiated)

When you configure and use a cloud provider, your audio data is transmitted to the provider you select:

- **Deepgram**: [Privacy Policy](https://deepgram.com/privacy)
- **Soniox**: [Privacy Policy](https://soniox.com/policies/privacy-policy)

These providers process your data under their own privacy policies. KoeKey sends audio data and your API key; no other personal information is transmitted.

### Model Downloads (user-initiated)

When you choose to use local processing and download a model, KoeKey downloads model files from **Hugging Face** (`huggingface.co`) or **GitHub** (`github.com`). No personal data is sent, but your IP address is visible to the hosting service during the download.

- **Hugging Face**: [Privacy Policy](https://huggingface.co/privacy)
- **GitHub**: [Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)

### Platform Stores

In-app purchase verification is handled by the platform's native store (Microsoft Store or App Store). KoeKey does not process payment data directly.

## Your Controls

You have full control over your data:

- **Choose local processing**: Use the local Whisper model to keep all audio data on your device.
- **Choose your cloud provider**: You decide which provider to use and provide your own API key.
- **Delete transcription history**: You can clear your history at any time within the app.
- **Remove API keys**: You can delete stored API keys through the app settings.
- **Manage output files**: Files you save to disk can be deleted through your file manager.

## Data Removal

- **Transcription history and settings**: Stored in your local app data directory. You can delete history within the app, or remove the directory manually.
- **API keys and encryption keys**: Stored in your OS credential store. You can remove them through the app settings. Note that uninstalling the app may not automatically remove credential store entries; you can clear them manually via Windows Credential Manager or macOS Keychain Access.
- **Output files**: Saved in locations you chose and must be deleted manually.

## Applicable Laws

KoeKey is designed to comply with applicable privacy laws. Under GDPR, CCPA, and similar regulations, you have rights to access, correct, and delete your personal data. Since all data is stored locally on your device, you can exercise these rights directly without contacting us.

## Children's Privacy

KoeKey is not directed at children under 13. We do not knowingly collect personal information from children.

## Changes to This Policy

We may update this policy when new features are added. Changes will be posted on this page with an updated date.

## Contact

If you have questions about this product, please contact us via our [inquiry form](https://forms.gle/oPqLindmrnVmocRt5).
