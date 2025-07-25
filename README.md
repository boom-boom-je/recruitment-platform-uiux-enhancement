# 사용자 행동 패턴 분석을 통한 홈페이지 개선 제안

본 프로젝트는 채용 플랫폼의 사용자 로그 데이터를 분석하여, 유저 행동을 이해하고 지원 전환율을 높이기 위한 전략을 도출하는 것을 목표로 합니다.

## 📌 프로젝트 개요

**목표**

  - 채용 플랫폼의 로그 데이터를 활용하여 AARRR 프레임워크를 통해 고객 행동 정의 및 분석
  - 분석 내용을 바탕으로 서비스 개선을 위한 UI/UX 개선 방안 제시

**배경**

  - 실제 채용 플랫폼의 사용자 로그 데이터를 활용하여 데이터 기반 인사이트 도출 경험을 쌓기 위한 프로젝트

**데이터 출처**

  - 채용 플랫폼 제공

## ✨ 개선안
![개선안](https://github.com/user-attachments/assets/98a1a76a-0e02-4712-bad8-7b2869cac75a)

## 📝 분석 프로세스

**1. 데이터 구조 확인 및 로그 분석**

  - 테이블 명세서 확인 및 각 테이블 데이터의 구조 확인
  - 로그 데이터를 하나하나 확인하며, 경로별 의미와 행동이 어떻게 기록되는지 확인
  - 이를 통해 로그 데이터의 전체적인 구조와 흐름을 이해하고, 사용자 여정을 구성할 수 있는 기반 마련
    
**2. 데이터 전처리 및 EDA**

  - 각 테이블별 인사이트 도출하고, 테이블 간의 연계를 통해 더 복합적이고 입체적인 사용자 행동 분석을 수행
    
**3. 전환 행동 분석**

  - AARRR 프레임워크를 통해 사용자 행동을 정의하고 분석
  - 신규 회원가입부터 지원 완료, 지원 후 추가 지원 관련 활동을 정의하여 이탈률/전환률 확인
  - 합격자와 불합격자로 사용자를 구분하여 각 Segment별 Retention 및 상위 행동 패턴 분석

## 📊 주요 인사이트

**1. 합격자/불합격자간 주요 행동 패턴 차이**

  - 합격자
    - 회원가입 이후 지원 활동까지 매우 적극적으로 참여하며, 공고 탐색부터 지원 완료까지 비교적 선형적인 퍼널 흐름을 따름
    - 이력서 작성 및 지원 완료 관련 행동 빈도가 높아 실제 전환으로 이어지는 경우가 많음
  - 불합격자
    - 기업 정보 탐색이 주를 이루며, 실제 지원 단계로 이어지는 비율이 낮음
    - 회원가입 이후 지원활동 내에서 지원 완료 없이 이탈하는 경우가 많아 전환까지 도달하는데에 어려움을 보임
  
**2. 합격자/불합격자간 Retention 경향 차이**

  - 합격자

![합격자](https://github.com/user-attachments/assets/d646e365-ef7c-4012-85a9-f5d896146f9b)

  - 불합격자

![불합격자](https://github.com/user-attachments/assets/3ae8560f-3c4a-4907-8d08-4aa19fbaa012)

**3. 합격자/불합격자간 지원 단계별 체류시간 분포**

![1](https://github.com/user-attachments/assets/54387218-14bd-4021-987a-ff495c97edd2)

  - step1, step2에 비해 step3, step4에서 더 오래 체류하는 경향 확인
  - 그 중 step3에서 가장 오래 체류하고 이를 통해 step3에서 가장 중요한 내용을 입력하는 페이지로 추정

**4. 예상 지원 프로세스 설정**

  - 분석 내용을 바탕으로 가상의 채용 플랫폼을 생성하고 분석 내용을 근거로 기존 채용 플랫폼의 지원 프로세스를 구성

![2](https://github.com/user-attachments/assets/6054916c-7680-4ac7-88b2-801b992ee123)


## 💡 전략 제안

![3](https://github.com/user-attachments/assets/ec4874c6-2806-4052-a72d-1c709a18d0d1)

## 📚 프로젝트 구조

- 📁`AARRR` : 사용자 행동 분석 및 퍼널 분석
- 📁`EDA` : 데이터 테이블 탐색 및 전처리
- 📁`report`: 분석 내용 정리된 pdf파일 및 가상 플랫폼의 개선안 구성한 figma 링크
- 📁`로그 분석`: 로그 데이터 탐색 및 설계 구조 확인

## 🛠 사용 도구 및 라이브러리

- **언어:** ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

- **분석 도구:** ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-ffffff?style=for-the-badge&logo=matplotlib&logoColor=black) ![Seaborn](https://img.shields.io/badge/Seaborn-2D708EFF?style=for-the-badge&logo=seaborn&logoColor=white)

- **환경:** ![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white) ![VSCode](https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
