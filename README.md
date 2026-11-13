# 🚗 카크크 (Car-KeuKeu)
> **"스마트폰 대신 서로의 목소리에 집중하는 시간, AI 레크리에이션 MC와 함께하는 패밀리 인카(In-Car) 소통 플랫폼"**
> 
> **현대자동차그룹 Pleos Connect 차량용 앱 개발 공모전 출품작**

[![Platform](https://img.shields.io/badge/Platform-Pleos%20Connect%20(AAOS)-002C5F?style=flat-square&logo=hyundai)](https://developer.hyundai.com/)
[![Language](https://img.shields.io/badge/Language-Kotlin-7F52FF?style=flat-square&logo=kotlin)](https://kotlinlang.org/)
[![AI](https://img.shields.io/badge/AI-Gemini%202.5%20Flash-4285F4?style=flat-square&logo=google)](https://deepmind.google/technologies/gemini/)
[![Release](https://img.shields.io/badge/APK-v1.0.0-success?style=flat-square&logo=android)]()

---

## 📌 1. 프로젝트 기획 의도 (Background & Purpose)

* **주목한 문제 (Pain Point):** 모처럼 떠나는 가족 나들이 길에서조차 뒷좌석 자녀들은 스마트폰 화면에만 빠져 있고, 앞좌석 부모는 운전 집중과 공감대 부족으로 인해 차 안에 어색한 침묵만 흐르는 **'단절된 이동 순간'**에 주목했습니다.
* **해결 솔루션 (Solution):** 바쁜 일상 속에서 온 가족이 한자리에 모이는 유일한 공간인 자동차를 **'달리는 패밀리 토크 스튜디오'**로 재정의합니다. **카크크(Car-KeuKeu)**는 내비게이션 도착 예정 시간(ETA)과 차량 주행 데이터를 연동하여, 운전자의 시선 분산(Zero-Glance) 없이 AI 음성 MC가 세대 공감 퀴즈와 토크를 진행하며 가족의 유쾌한 대화와 웃음을 이끌어냅니다.

---

## 🎥 2. 시연 영상 및 주요 화면 (Demo & Screenshots)

### ▶️ 시연 영상 보러가기
* **[🔗 카크크(Car-KeuKeu) 공식 시연 영상 (YouTube 링크 삽입)](https://youtu.be/여기에_영상_링크를_넣어주세요)**

### 🖼️ 주요 인포테인먼트 UI 화면
| ① 사전 온보딩 & 구호 등록 | ② 주행 중 AI MC 퀴즈 진행 | ③ 2시간 주행 휴게소 미션 | ④ 도착 후 가족 대화 리포트 |
| :---: | :---: | :---: | :---: |
| <img src="docs/images/screen1.png" width="220" alt="온보딩 화면"/> | <img src="docs/images/screen2.png" width="220" alt="주행 중 화면"/> | <img src="docs/images/screen3.png" width="220" alt="휴게소 미션 화면"/> | <img src="docs/images/screen4.png" width="220" alt="리포트 화면"/> |
| 가족별 나이·음성·구호 설정 | 다크 모드 & 음성 파형 UI | P단 전환 시 현장 미션 전송 | QR 연동 모바일 카드뉴스 공유 |

> *(※ 위 이미지 경로 `docs/images/...`에 실제 앱 캡처 화면이나 GIF를 업로드해 교체해 주세요.)*

---

## ✨ 3. 핵심 기능 및 차량 특화 요소 (Key Features)

### ① 내비게이션 ETA 연동 타임라인 자동 스케줄링
* **동적 코스 설계:** 실시간 도착 예정 시간(ETA)과 교통 체증 데이터를 분석해 `[전체 ETA - 5분(안전 버퍼)]`에 맞춘 최적의 레크리에이션 코스를 자동 구성합니다.
* **도착 5분 전 안전 종료:** 목적지 도착 5분 전에는 운전자가 초행길 진입 및 주차에 온전히 집중할 수 있도록 게임을 자동 마무리하고 잔잔한 배경음악으로 전환합니다.

### ② Voice-First AI MC & 0.1초 단위 '음성 구호 버저'
* **Zero-Glance 인터랙션:** 주행 중 화면 터치 없이 AI MC('크크봇')의 음성 진행과 좌석별(1열/2열) 음성 인식만으로 모든 게임에 참여합니다.
* **개인별 음성 구호 판독:** 출발 전 등록한 가족별 고유 구호(예: 아빠 *"왕년에!"*, 첫째 *"저요저요!"*, 둘째 *"크크!"*)를 외치면, 성문 인식 및 발화 타임스탬프를 0.1초(ms) 단위로 분석해 가장 먼저 외친 사람에게 정답 기회를 부여합니다.

### ③ 장거리(2시간+) 주행 감지 & 휴게소 현장 미션 (O2O 연계)
* **졸음운전 예방:** 2시간 이상 연속 주행이 감지되면 내비게이션 경로 상 전방 휴게소(POI)를 탐색해 휴식을 권유합니다.
* **휴게소 보너스 미션:** 휴게소 진입 후 기어를 주차(P단)로 전환하면 *"아빠가 제일 좋아하는 휴게소 간식 맞히고 사 오기"* 등 현장 미션을 스마트폰으로 전송해 환기와 휴식을 돕습니다.

### ④ 세대 공감 맞춤형 퀴즈 & 삼행시·노래 AI 실시간 심사
* **세대 교차 콘텐츠:** 부모 세대(1990s 삐삐 암호 등)와 자녀 세대(2020s 최신 유행어 등)의 나이 및 목적지 지역 정보를 반영한 실시간 퀴즈를 생성합니다.
* **AI 심사위원:** 목적지 이름으로 삼행시 짓기(운율·재치 분석), 애창곡 한 소절 부르기(음정·박자·성량 분석)를 실시간 채점하여 유머러스한 심사평과 순위를 제공합니다.

### ⑤ In-Car to Mobile '오늘의 가족 대화 리포트'
* 목적지 도착 후 **기어 P단 전환 시**, 오늘의 대화 MVP, 베스트 삼행시, 휴게소 미션 인증샷이 담긴 요약 화면을 표시하고 QR 코드 및 카카오톡 공유를 통해 가족 스마트폰으로 리포트 카드뉴스를 전송합니다.

---

## 🛠️ 4. 시스템 아키텍처 및 기술 스택 (Tech Stack & SDK)

| 개발 영역 | 적용 기술 / SDK / API | 핵심 구현 내용 |
| :--- | :--- | :--- |
| **차량·내비 연동**<br>*(Pleos Connect)* | • **Pleos Connect Navigation SDK**<br>• **Pleos Vehicle API** (`CarPropertyManager`) | • 목적지명, 실시간 ETA, 전방 휴게소(POI) 거리 데이터 실시간 구독<br>• 기어 상태(`GEAR_SELECTION`), 주행 속도(`PERF_VEHICLE_SPEED`) 감지 및 안전 제어 |
| **화자 구분 및**<br>**음성 구호 인식** | • **Pleos Multi-Zone Audio API**<br>• **Picovoice Eagle & Porcupine SDK**<br>• **ReturnZero VITO STT** (또는 Google STT) | • 차량 내 좌석별(1열·2열) 마이크 오디오 스트림 분리<br>• 온디바이스 성문 인식으로 가족 구분 및 `ms` 단위 구호 선착순 판정<br>• 한국어 특화 실시간 STT로 퀴즈 정답 및 삼행시 텍스트 변환 |
| **퀴즈 생성 및**<br>**AI MC·심사** | • **Google Gemini 2.5 Flash API**<br>• **ElevenLabs API / CLOVA Voice** | • 탑승자 연령대 + 목적지명 + 남은 시간 기반 JSON 스키마 프롬프팅으로 실시간 퀴즈 생성 및 삼행시 창의력 심사<br>• 라디오 DJ 톤의 고품질 감정 표현 TTS 발화 |
| **노래 심사**<br>*(오디오 DSP)* | • **TarsosDSP** / **Web Audio API** | • 마이크 입력 음성의 실시간 주파수(Pitch/Hz)와 데시벨(dB, 성량·호응도)을 분석하여 노래 부르기 정량 점수 산출 |
| **모바일 확장**<br>*(O2O 연동)* | • **Firebase Realtime Database**<br>• **KakaoTalk 공유 API** | • P단 전환 시 클라우드 DB 동기화 및 QR/카카오톡 기반 모바일 리포트 카드뉴스 즉시 공유 |

---

## 🚀 5. 빌드 및 실행 방법 (How to Build & Run)

### 방법 A. 제출된 APK 파일로 즉시 실행 (심사위원 권장)
별도의 API 키 설정 없이 모든 기능을 즉시 테스트하실 수 있도록 빌드된 **완성본 APK**를 함께 제출하였습니다.
1. 제출 파일 중 `CarKeuKeu-release.apk` (또는 GitHub [Releases] 탭의 APK)를 다운로드합니다.
2. Pleos Connect 에뮬레이터(AAOS) 또는 테스트 기기에 아래 명령어로 설치합니다.
   ```bash
   adb install CarKeuKeu-release.apk

<img width="1498" height="766" alt="image" src="https://github.com/user-attachments/assets/795827c3-d90c-406b-a898-c9470f855cdb" />
