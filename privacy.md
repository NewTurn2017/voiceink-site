---
layout: default
title: WithVoice Privacy Policy
permalink: /privacy/
---

# WithVoice Privacy Policy

_Last updated: 2026-10-15_

WithVoice ("the app", "we", "us"; internal code name and bundle ID: VoiceInk / `com.voiceink.ios`) is an AI voice-dictation keyboard for iPhone. You speak, your speech is transcribed and cleaned up into text, and the text is inserted at your cursor. This policy explains exactly what data the app handles, where it goes, and what is kept on your device.

**Short version:** WithVoice has no servers and no accounts. Your audio and the resulting text are sent only to Google's Gemini API to perform transcription. During the built-in free trial (the first 10 dictations), that request uses the developer's Gemini API key on Google's free tier; after the trial, it uses an API key that you supply. Under Google's free-tier terms, Google may use the content to improve its products (see "How Google handles your data" below). We do not upload or store your recordings or transcripts on any server of ours, and we do not use any analytics or tracking.

> 한국어 요약은 [이 페이지 하단](#한국어-요약)에 있습니다.

## Who is the data controller

WithVoice is the app developer. For the transcription step, your audio and text are sent to Google LLC ("Google") through its Gemini API and are handled under Google's terms for the API key used for the request: the developer's key during the free trial, or your own key after you add one.

Contact: hyuni2020@gmail.com

## What data the app handles

1. **Recorded audio.** When you start dictation, the WithVoice app records audio from your device's microphone for the duration of your dictation. Recording runs in the app, in the foreground (the keyboard opens the app to start it); the app does not record in the background.
2. **Transcribed text.** The text produced by transcription and cleanup, which is then inserted at your cursor in whatever app you are using.
3. **Your Google Gemini API key** (optional during the free trial). A credential you provide so the app can call Google's Gemini API on your behalf.
4. **App settings and usage counters.** Your selected model, dictation mode, keyboard input language and keyboard haptic setting; the number of free-trial dictations used; and, for dictations made with your own key, token counts and an estimated API cost shown in Settings.

The app does **not** collect your name, email, contacts, location, advertising identifiers, or any device-tracking identifiers.

## How the data is used and where it goes

- **Audio → Google Gemini API.** Your recorded audio is sent over an encrypted connection (HTTPS) to Google's Gemini API for transcription and clean-up (removing filler words, adding punctuation). This is the core function of the app and cannot be performed without sending the audio to Google.
- **Which API key is used.** If you have not added your own key and free-trial dictations remain, the request is authenticated with the developer's Gemini API key, which belongs to a Google Cloud project with billing disabled (Google's free tier). Once you add your own key, every request uses your key. If a trial request fails with an error (for example, the trial key is unavailable), the app returns a clearly labeled placeholder text ("[데모]" / "[Demo]") instead of a transcription; that placeholder is fixed text built into the app.
- **Resulting text → your cursor.** The transcribed text is returned to the app, handed to the WithVoice keyboard on your device, and inserted into the active text field. It is not sent anywhere else by the app.
- **No WithVoice server.** WithVoice does not operate any backend server. Your audio and text never pass through, and are never stored on, any infrastructure controlled by us. The only network destination of your audio and text is Google's Gemini API.

## How Google handles your data

Google's handling of the data sent to the Gemini API depends on whether the API key belongs to a free-tier or a paid-tier Google project. Google's official Gemini API pricing page (ai.google.dev/gemini-api/docs/pricing, checked 2026-10-15) lists, for each model, whether data is "Used to improve our products": **Yes** on the free tier and **No** on the paid tier. This means:

- **Free trial:** the trial uses a free-tier key, so the audio and text of trial dictations may be used by Google to improve its products.
- **Your own key on the free tier:** the same applies if your key belongs to a project without billing enabled.
- **Your own key on the paid tier:** according to the pricing page, the data is not used to improve Google's products.

If you do not want your dictations to be used to improve Google's products, add a key from a paid-tier (billing-enabled) Google project before you dictate, instead of using the free trial. The governing terms are Google's, not ours; please review the Gemini API Additional Terms of Service (https://ai.google.dev/gemini-api/terms) and Google's privacy policy.

## Your Google Gemini API key

- You obtain your own API key from Google (for example, via Google AI Studio) and enter it in the app's settings.
- The key is stored locally on your device in the **iOS Keychain**, in a Keychain access group shared by the WithVoice app and its keyboard extension. Only the app uses the key, to authenticate your own requests to Google. It is not transmitted to us.
- To stop using your key, clear the "Gemini API Key" field in the app's settings and tap "저장" (Save). This replaces the stored key with an empty value, and dictation no longer uses it. The app does not have a separate delete button.
- iOS may keep Keychain items even after an app is deleted, so clear the key in the app first if you want it removed from your device.

## Data retention

- **Audio is not retained.** Recordings are held only in memory for the moment needed to send them for transcription. The app does not save them to storage.
- **The most recent transcript is kept on your device for the handoff.** To hand the result from the app to the keyboard, the app writes the latest transcript to storage shared by the app and its keyboard on your device (an App Group). How long it stays there depends on the app version: in versions before 1.2.0, it stays there until the next dictation overwrites it; from version 1.2.0, it is deleted when the keyboard inserts it or when you tap "처음으로" (Start over) on the completion screen. From 5 minutes after the dictation, it can no longer be inserted, and it is deleted the next time the app or the keyboard checks for it. While the app stays open, it also keeps the latest transcript in memory to show it on the completion screen; if you tap "복사" (Copy) there, the text is placed on the iOS clipboard, which iOS manages. The transcript is never uploaded to us.
- **No dictation history.** The app does not keep a list or log of your past dictations.
- **Settings and counters** (see "What data the app handles") stay on your device until you change or reset them. The trial-use counter is kept in the iOS Keychain. You can reset the token and cost counters in Settings.
- Your API key stays on your device in the Keychain until you clear it as described above (see "Your Google Gemini API key").
- Data that reaches Google is retained and used under Google's terms (see "How Google handles your data").

## Permissions

- **Microphone.** Required to record your speech when you tap the mic. Audio is captured only while you are actively dictating.
- **Keyboard "Full Access".** Typing works without Full Access. The mic key needs "Allow Full Access" so the keyboard can open the WithVoice app, where recording and transcription happen, and so the app and keyboard can share your settings and the transcription result on your device. Key-press haptic feedback (a light vibration) also works only with Full Access, and you can turn it off in the app's settings. The keyboard itself makes no network requests; only the app sends the Google Gemini API request.

## Analytics and tracking

WithVoice contains **no third-party analytics, no advertising SDKs, and no tracking** of any kind. We do not build user profiles and we do not track you across apps or websites.

## Children

WithVoice is not directed at children and does not knowingly collect data from children. The app is rated 4+. After the free trial it requires a Google API key, and it is intended for general audiences.

## Data sharing and sale

We do not sell or rent your personal data, and we do not share it with third parties. The only transfer of your data is the transcription request you start, which goes to Google's Gemini API (with the developer's free-tier key during the trial, or with your own key afterwards). Google handles that data under its own terms.

## Security

Audio and text are transmitted to Google over encrypted HTTPS connections. Your API key is stored in the iOS Keychain, which is protected by the operating system. Because there is no WithVoice server, there is no central store of your data to breach.

## International users

When you use the app, your audio and text are sent to Google's Gemini API, which may process data on infrastructure located outside your country. This transfer happens when you start a dictation, to provide the transcription service.

## Changes to this policy

We may update this policy as the app evolves. Material changes will be reflected by updating the "Last updated" date above and, where appropriate, in the app or its App Store listing.

## Contact

Questions about privacy? Contact: hyuni2020@gmail.com

---

## 한국어 요약

**WithVoice는 서버와 계정이 없는 앱입니다.** 음성과 전사된 텍스트는 받아쓰기를 위해 Google Gemini API로만 전송됩니다. 무료 체험(처음 10회) 동안은 개발자의 Gemini API 키(Google 무료 등급)를, 그 뒤에는 사용자가 넣은 API 키를 씁니다. WithVoice는 녹음이나 전사 결과를 자체 서버에 올리거나 저장하지 않으며, 분석 도구나 추적을 쓰지 않습니다.

- **처리하는 데이터**: 받아쓰기 중 녹음된 음성(앱이 포그라운드일 때만), 전사된 텍스트, 사용자가 넣은 Gemini API 키(체험 중에는 선택, 기기 Keychain에만 저장), 앱 설정과 사용량 카운터(모델·받아쓰기 모드·키보드 입력 언어·키보드 햅틱 설정, 체험 사용 횟수, 본인 키로 받아쓴 경우의 토큰 수와 예상 비용). 이름·이메일·연락처·위치·광고 식별자는 수집하지 않습니다.
- **데이터가 가는 곳**: 음성과 텍스트는 HTTPS 암호화 연결로 Google Gemini API에만 전송됩니다. WithVoice 서버는 없습니다. 체험 요청이 오류로 실패하면 앱에 내장된 "[데모]" 표시 고정 문구를 대신 돌려줍니다.
- **Google의 처리**: Google의 Gemini API 가격표(2026-10-15 확인)에 따르면 무료 등급에서는 데이터가 Google 제품 개선에 쓰일 수 있고, 유료 등급에서는 쓰이지 않습니다. 무료 체험과 결제가 꺼진 프로젝트의 본인 키는 무료 등급입니다. 원하지 않으면 받아쓰기 전에 결제가 켜진 Google 프로젝트의 키를 넣으세요.
- **보관**: 음성은 저장하지 않습니다. 최근 전사문은 키보드로 넘기기 위해 기기 안 공유 저장소(App Group)에 둡니다. 1.2.0 이전 버전에서는 다음 받아쓰기가 덮어쓸 때까지 남고, 1.2.0부터는 키보드가 삽입하거나 완료 화면에서 '처음으로'를 누르면 지워집니다. 받아쓰기 5분 뒤부터는 더 이상 삽입되지 않고, 앱이나 키보드가 다음에 확인할 때 지워집니다. 앱이 열려 있는 동안에는 완료 화면에 보여 주려고 최근 전사문을 메모리에 들고 있으며, 거기서 '복사'를 누르면 iOS가 관리하는 클립보드에 들어갑니다. 받아쓰기 기록은 남기지 않으며, 전사문을 저희에게 올리지 않습니다. 설정과 카운터는 바꾸거나 초기화할 때까지 기기에 남고, 체험 사용 횟수는 Keychain에 보관됩니다.
- **API 키**: 기기 Keychain에 저장되며 앱이 Google 요청을 인증할 때만 씁니다. 그만 쓰려면 앱 설정의 "Gemini API Key" 칸을 비우고 "저장"을 누르세요(별도 삭제 버튼은 없습니다). 앱을 지워도 Keychain 항목이 남을 수 있으니 먼저 앱에서 비우세요.
- **권한**: 마이크(받아쓰기 중에만 사용). 키보드 '전체 접근 허용'은 타이핑에는 필요 없고, 마이크 키로 앱을 열 때, 앱과 키보드가 설정과 전사 결과를 기기 안에서 나눌 때, 키 햅틱에 필요합니다(햅틱은 앱 설정에서 끌 수 있습니다). 키보드 자체는 네트워크 요청을 하지 않습니다.
- **추적 없음**: 제3자 분석, 광고 SDK, 사용자 추적이 없습니다.
- **문의**: hyuni2020@gmail.com

---

[Home](../) · [Support](../support/)

© 2026 WithVoice
