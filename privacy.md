---
layout: default
title: VoiceInk Privacy Policy
permalink: /privacy/
---

# VoiceInk Privacy Policy

_Last updated: 2026-06-01_

VoiceInk ("the app", "we", "us") is an AI voice-dictation keyboard for iPhone. You speak, your speech is transcribed and cleaned up into text, and the text is inserted at your cursor. This policy explains exactly what data the app handles, where it goes, and what we do and do not keep.

**Short version:** VoiceInk has no servers and no accounts. Your audio and the resulting text are sent only to Google's Gemini API, using an API key that you supply, to perform transcription. We do not retain your recordings or transcripts, and we do not use any analytics or tracking.

> 한국어 요약은 [이 페이지 하단](#한국어-요약)에 있습니다.

## Who is the data controller

VoiceInk is the app developer. For the transcription step, Google LLC ("Google") acts as the processor of the audio and text you send to its Gemini API, under your own Google API key and under Google's terms.

Contact: **hyuni2020@gmail.com**

## What data the app handles

1. **Recorded audio.** When you start dictation, the VoiceInk app records audio from your device's microphone for the duration of your dictation. Recording runs in the app, in the foreground (the keyboard opens the app to start it); the app does not record in the background.
2. **Transcribed text.** The text produced by transcription and cleanup, which is then inserted at your cursor in whatever app you are using.
3. **Your Google Gemini API key.** A credential you provide so the app can call Google's Gemini API on your behalf.

The app does **not** collect your name, email, contacts, location, advertising identifiers, or any device-tracking identifiers.

## How the data is used and where it goes

- **Audio → Google Gemini API.** Your recorded audio is sent over an encrypted connection (HTTPS) to Google's Gemini API for transcription and clean-up (removing filler words, adding punctuation). This is the core function of the app and cannot be performed without sending the audio to Google.
- **Resulting text → your cursor.** The transcribed text is returned to the app and inserted into the active text field on your device. It is shown to you and placed where you are typing; it is not sent anywhere else by the app.
- **No VoiceInk server.** VoiceInk does not operate any backend server. Your audio and text never pass through, and are never stored on, any infrastructure controlled by VoiceInk. The only network destination is Google's Gemini API.

Google's handling of the data you send to the Gemini API is governed by Google's own terms and privacy policy for that service. Please review Google's terms for the Gemini API / Google AI Studio to understand how Google processes API requests made with your key. We encourage you to use an API key whose project settings reflect your desired data-handling preferences.

## Your Google Gemini API key

- You obtain your own API key from Google (for example, via Google AI Studio) and enter it in the app's settings.
- The key is stored locally on your device in the **iOS Keychain**, in a shared Keychain access group so that both the VoiceInk app and its keyboard extension can use it. It is not transmitted to VoiceInk and is sent only to Google as part of authenticating your own API requests.
- You can remove the key at any time from the app's settings. Removing the key disables transcription.

## Data retention

- **The app does not retain your audio.** Recordings are held only in memory/temporarily on-device for the moment needed to send them for transcription, and are not saved by the app afterward.
- **The app does not retain your transcripts.** The resulting text is inserted at your cursor and not stored by the app.
- **No history or logs of your dictations** are kept by VoiceInk.
- Your API key persists on-device in the Keychain until you remove it or uninstall the app.

## Permissions

- **Microphone.** Required to record your speech when you tap the mic. Audio is captured only while you are actively dictating.
- **Keyboard "Full Access".** iOS requires "Allow Full Access" for the VoiceInk keyboard to open the VoiceInk app, where recording and transcription happen. The keyboard itself does not send your data anywhere; the app performs the Google Gemini API request. VoiceInk uses Full Access only to open the app and to share your selected settings between the app and keyboard.

## Analytics and tracking

VoiceInk contains **no third-party analytics, no advertising SDKs, and no tracking** of any kind. We do not build user profiles and we do not track you across apps or websites.

## Children

VoiceInk is not directed at children and does not knowingly collect data from children. The app is rated 4+ but requires a Google API key and is intended for general audiences.

## Data sharing and sale

We do not sell, rent, or share your personal data with third parties. The only transfer of your data is the technical request you initiate to Google's Gemini API to perform transcription, using your own key.

## Security

Audio and text are transmitted to Google over encrypted HTTPS connections. Your API key is stored in the iOS Keychain, which is protected by the operating system. Because there is no VoiceInk server, there is no central store of your data to breach.

## International users

When you use the app, your audio and text are sent to Google's Gemini API, which may process data on infrastructure located outside your country. This transfer is initiated by you, with your key, to provide the transcription service.

## Changes to this policy

We may update this policy as the app evolves. Material changes will be reflected by updating the "Last updated" date above and, where appropriate, in the app or its App Store listing.

## Contact

Questions about privacy? Contact: **hyuni2020@gmail.com**

---

## 한국어 요약

**VoiceInk는 서버와 계정이 없는 앱입니다.** 사용자의 음성과 전사된 텍스트는 사용자 본인이 제공한 API 키를 통해 오직 Google Gemini API로만 전송되며, VoiceInk는 녹음·전사 기록을 저장하지 않고 어떠한 분석 도구나 추적도 사용하지 않습니다.

- **수집하는 데이터**: 받아쓰기 중 녹음된 음성(포그라운드에서만), 전사된 텍스트, 사용자가 입력한 Gemini API 키(기기 Keychain에만 저장). 이름·이메일·연락처·위치·광고 식별자는 수집하지 않습니다.
- **데이터가 가는 곳**: 음성과 텍스트는 HTTPS 암호화 연결로 Google Gemini API에만 전송됩니다. VoiceInk 서버는 존재하지 않습니다.
- **보관**: 앱은 음성, 전사 결과, 받아쓰기 기록을 보관하지 않습니다. API 키는 삭제하거나 앱을 제거할 때까지 기기에만 저장됩니다.
- **권한**: 마이크(받아쓰기 중에만 사용), 키보드 전체 접근(키보드가 앱을 열고 설정을 공유하기 위해서만 사용).
- **추적 없음**: 제3자 분석, 광고 SDK, 사용자 추적이 전혀 없습니다.
- **문의**: hyuni2020@gmail.com

---

[Home](../) · [Support](../support/)

© 2026 VoiceInk
