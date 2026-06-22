# dart_iztro

[한국어](README.md) | [English](README.en.md) | [简体中文](README.zh_CN.md) | [繁體中文](README.zh_TW.md) | [日本語](README.ja.md) | [ภาษาไทย](README.th.md) | [Tiếng Việt](README.vi.md)

> 이 저장소는 molpass가 포크한 사본입니다. 기본 출력 언어를 한국어(ko_KR)로 설정했습니다.

자미두수(紫微斗數)와 팔자(八字) 계산을 위한 크로스플랫폼 Flutter 플러그인입니다. 자미두수 명반과 팔자 계산 기능을 제공하며, 음력·양력 변환을 지원하고, 운명 분석·점술·점성 응용에 사용할 수 있습니다.

> 면책: 이 프로젝트 코드는 [@SylarLong/iztro](https://github.com/SylarLong/iztro)에서 파생되었습니다. 원작자의 오픈소스 기여에 감사드립니다.
>
> 문서: 전체 문서는 [iztro.com](https://iztro.com)에서 확인할 수 있습니다(@SylarLong/iztro 기준).

## 주요 기능

- 양력에서 음력 날짜 계산
- 팔자(八字) 정보 계산
- 자미두수 명반 정보 계산
- 명반의 각 궁(宮)에 대한 상세 정보 제공
- 진태양시(眞太陽時) 정확 계산(천문 알고리즘 기반)
- 위도·경도 기반 지리 위치 조회
- 다중 플랫폼 지원: Android, iOS, macOS, Windows, Linux, Web
- 다국어 지원: 간체·번체 중국어, 영어, 일본어, 한국어, 태국어, 베트남어

## 설치

`pubspec.yaml`에 의존성을 추가합니다:

```yaml
dependencies:
  dart_iztro: ^latest
```

또는:

```bash
flutter pub add dart_iztro
```

## 언어 설정

이 포크는 기본 출력 언어가 한국어(ko_KR)입니다. 다른 언어로 바꾸려면:

```dart
import 'package:dart_iztro/dart_iztro.dart';

// 초기화 시 언어 지정 (미지정 시 기본값 ko_KR)
IztroTranslationService.init(initialLocale: 'ko_KR');

// 실행 중 언어 변경
IztroTranslationService.changeLocale('en_US');
```

## 자세한 사용법

자미두수 명반 생성, 팔자 계산, 궁·별 분석 등 전체 한국어 사용 가이드와 API 설명은 다음을 참고하세요.

- 사용 가이드: [iztro.com](https://iztro.com)
- 라이선스: [LICENSE](LICENSE) (MIT)
