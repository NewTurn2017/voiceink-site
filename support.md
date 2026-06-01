---
layout: default
title: VoiceInk Support
permalink: /support/
---

# VoiceInk Support

Need help with VoiceInk? You're in the right place. / VoiceInk 사용에 도움이 필요하신가요?

## Contact / 문의

For any questions, bug reports, or feature requests, email us:

**📧 hyuni2020@gmail.com**

We aim to reply within 2 business days. / 영업일 기준 2일 이내 답변을 드리도록 노력하고 있습니다.

## Frequently asked questions / 자주 묻는 질문

### Where do I get a Google Gemini API key? / Gemini API 키는 어디서 받나요?

Visit [Google AI Studio](https://aistudio.google.com/), sign in with your Google account, and create a free API key. Paste it into VoiceInk's settings screen — it is stored securely in your device's Keychain.

[Google AI Studio](https://aistudio.google.com/)에서 Google 계정으로 로그인한 뒤 무료 API 키를 만들 수 있습니다. 발급받은 키를 VoiceInk 설정 화면에 붙여넣으면 기기의 Keychain에 안전하게 저장됩니다.

### How do I enable the VoiceInk keyboard? / 키보드는 어떻게 활성화하나요?

1. Open iOS **Settings → General → Keyboard → Keyboards → Add New Keyboard** and select **VoiceInk**.
2. Tap **VoiceInk** again and turn on **Allow Full Access** (this lets the keyboard open the VoiceInk app, where recording happens).
3. In any app, hold the globe key and switch to VoiceInk.

iOS **설정 → 일반 → 키보드 → 키보드 → 새로운 키보드 추가**에서 **VoiceInk**를 선택한 뒤, 다시 **VoiceInk**를 눌러 **전체 접근 허용**을 켜주세요. (키보드가 녹음을 위해 VoiceInk 앱을 열 수 있게 해줍니다.)

### Why does recording open the VoiceInk app? / 왜 녹음할 때 앱이 열리나요?

iOS does not allow keyboard extensions to access the microphone. When you tap the mic, the keyboard opens the VoiceInk app, which records in the foreground. After you stop, the cleaned-up text is inserted back at your cursor.

iOS는 키보드 확장이 마이크에 접근하는 것을 허용하지 않습니다. 마이크를 누르면 키보드가 VoiceInk 앱을 열고, 앱이 포그라운드에서 녹음합니다. 정지 후 키보드로 돌아오면 정리된 텍스트가 커서 위치에 입력됩니다.

### Does VoiceInk store my recordings or transcripts? / 녹음이나 전사 내용을 저장하나요?

No. VoiceInk has no servers. Audio and text are sent only to Google's Gemini API using your own key, and the app does not retain recordings or transcripts. See our [Privacy Policy](../privacy/) for details.

아니요. VoiceInk는 서버가 없습니다. 음성과 텍스트는 사용자 본인의 키로 Google Gemini API에만 전송되며, 앱은 녹음과 전사 결과를 저장하지 않습니다. 자세한 내용은 [개인정보 처리방침](../privacy/)을 참고하세요.

### Transcription isn't working. What should I check? / 전사가 안 될 때 확인할 것들

1. **API key** — make sure a valid Gemini API key is entered in VoiceInk settings. / 유효한 Gemini API 키가 설정에 입력되어 있는지 확인하세요.
2. **Internet connection** — transcription requires a network connection. / 전사에는 인터넷 연결이 필요합니다.
3. **Microphone permission** — check iOS Settings → VoiceInk → Microphone. / iOS 설정 → VoiceInk → 마이크 권한을 확인하세요.
4. **Quota** — free Gemini API keys have daily limits; check [Google AI Studio](https://aistudio.google.com/). / 무료 키는 일일 사용량 제한이 있습니다.

---

[Home](../) · [Privacy Policy](../privacy/)

© 2026 VoiceInk
