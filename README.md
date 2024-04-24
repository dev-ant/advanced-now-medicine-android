# 🚀 복약 관리 도우미 “지금이약” Advanced 프로젝트 🚀 
[![Android CI](https://github.com/dev-ant/advanced-now-medicine-android/actions/workflows/android-build.yml/badge.svg)](https://github.com/dev-ant/advanced-now-medicine-android/actions)
[![ktlint](https://img.shields.io/badge/code%20style-%E2%9D%A4-FF4081.svg)](https://ktlint.github.io/)

<!-- ![그림1](https://github.com/dev-ant/advanced-now-medicine-android/assets/59863112/b8cb2572-5523-4b2a-8cb0-b7d057e032f0) -->

이 프로젝트는 2023년 캡스톤 디자인 프로젝트였던 "지금이약"의 안드로이드 어플리케이션 업그레이드를 목표로 합니다. *전체 구조의 재구축, 약간의 기능 변화, 더 나은 성능, 가독성 및 유지 보수성을 위해 최근 안드로이드 개발 트랜드와 라이브러리를 도입하여 지난 1년간의 발전을 확인합니다.* `MVVM-Pattern`과 `Git-Flow`를 사용하고 있습니다. 원본 프로젝트와 개발 과정이 궁금하다면 아래의 링크를 확인해주세요.

> Now Medicine `Android`  <a href="https://github.com/Nter-developer/bravo-health-park-android" target="_blank">Origin Repository</a> `Tech Blog` <a href="https://velog.io/@nter-developer/series/NowMedicine" target="_blank">시리즈 | NowMedicine</a>

</br>

## 목차

1. [개선 사항](#-개선-사항)
2. [추가 사항](#-추가-사항)
3. [기능 변화](#%EF%B8%8F-기능-변화)

</br>

## 🌱 개선 사항
* 언어: Java에서 안드로이드 공식 언어인 Kotlin으로 전환하여 생산성과 가독성을 향상시킵니다.
* 아키텍처: MVP(Model-View-Presenter)에서 MVVM(Model-View-ViewModel)으로 전환하여 관심사 분리를 개선하고 테스트를 용이하게 합니다.
* 데이터 저장: SharedPreferences을 대신하는 데이터 저장소 솔루션인 DataStore을 사용합니다. 로컬 데이터베이스 관리를 위해 Room을 사용합니다.
* UI: XML 기반 레이아웃에서 더 선언적이고 유연한 UI 개발 경험을 위해 Jetpack Compose로 전환합니다.

</br>

## ✨ 추가 사항
* 동시성: 비동기 및 논블로킹 프로그래밍을 위해 코루틴을 도입합니다.
* 의존성 주입: 종속성 주입을 간소화하기 위해 Hilt를 활용합니다.
* ViewModel: 라이프사이클을 고려한 UI 관련 데이터 관리를 위해 ViewModel을 사용합니다.
* Ktlint: 코드 가독성의 확보와 코드 스타일 엄수의 자동화를 위해서 Ktlint를 도입합니다.
* GitHub Actions: 지속적인 테스트의 자동화를 위해서 간단한 CI 파이프라인을 구축합니다.
* 테스트: 코드의 품질과 안정성을 위해 JUnit을 도입하여 테스트를 수행합니다.

</br>

## 🕹️ 기능 변화
* 오프라인: 서버와 통신 없이 모든 기능을 오프라인으로 사용 가능하게 변경합니다.
  * 제외 대상: 자동 로그인 및 회원가입, OCR(광학 문자 인식 설명)을 이용한 알림 생성
  * 변경 대상: 수동 알림 생성, 식사 시간대 설정, 사용자 설정

</br>
