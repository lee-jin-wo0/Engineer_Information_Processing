# Section 01 소프트웨어 개발 환경 분석

## 01 현행 시스템 파악

### 01 현행 시스템 파악 개요

:one: 현행 시스템 파악 정의

:small_blue_diamond: 목표 시스템의 개발 범위 및 방향성을 정하기 위해 현재 운행되는 시스템의 구성을 파악하는 활동.

 :small_blue_diamond: 제공 기능과 주고 받는 정보뿐 아니라 소프트웨어, 하드웨어, 네트워크 구성 등도 파악.

<br />

:two: 현행 시스템 파악 절차

<img src="https://github.com/lee-jin-wo0/License-EngineerInformationProcessing-Study/blob/main/Part01/Chapter02/Section01/img/%EA%B7%B8%EB%A6%BC2.1.01.png" alt="그림2.1.01"  />

<br />

### 02 현행 시스템 구성 및 기능 파악

:one: 시스템 구성 현황 파악

:small_blue_diamond: 기간 업무 : 주요 업무.

:small_blue_diamond: 지원 업무 : 주요 업무를 지원하는 업무​.

:small_blue_diamond: 각 단위 업무 정보 시스템의 명칭과 주요 기능을 명시하여 조직 내 모든 정보 시스템의 현황을 파악.

<br />

:two: 시스템 기능 현황 파악

:small_blue_diamond: 단위 업무 시스템이 현재 제공하고 있는 기능을 파악하는 것.

:small_blue_diamond: ​ 단위 업무 시스템에서 제공하는 기능들을 주요 기능과 세부 기능으로 구분하여 계층형으로 표현.

<br />

:three: 시스템 인터페이스 파악

:small_blue_diamond: 단위 업무 시스템들이 서로 주고 받는 데이터의 종류나 형식, 프로토콜, 연계 유형, 주기 등을 파악.

:small_blue_diamond: 데이터 형식 : 고정 포맷, 가변 포맷, JSON, XML 등

:small_blue_diamond: 통신규약(프로토콜) : TCP/IP, X, 25 등

:small_blue_diamond: 연계 유형 : EAI, FEP 등

<br />

### 03 현행 시스템 아키텍처 및 소프트웨어 파악

:one: 시스템 아키텍처 구성도 파악

:small_blue_diamond: 기간 업무 수행을 위한 기술 요소들을 계층별로 구성한 도표

:small_blue_diamond: 업무 시스템별로 아키텍처가 다른 경우에는 가장 핵심이 되는 기간 업무 처리 시스템을 기준으로 함.

<br />

:two: 소프트웨어 구성도 파악

:small_blue_diamond: 단위 업무 시스템의 업무 처리를 위해 설치되어 있는 소프트웨어들의 사양과 라이선스 방식, 개수 등을 파악.

:small_blue_diamond: 시스템 구축 시 소프트웨어 비용이 적지 않기 때문에, 소프트웨어 라이선스 파악이 중요.

<br />

### 04 현행 시스템 하드웨어 및 네트워크 파악

:one: 하드웨어 구성도 파악

:small_blue_diamond: 단위 업무 시스템들의 물리적 위치와 주요 사양, 수량, 이중화 적용 여부 등을 파악.

:small_blue_diamond: 이중화는 서비스 기간, 장애 대응 정책에 따라 결정되며, 현행 시스템에 이중화가 적용된 경우에는 목표 시스템에도 대부분 구축이 필요.

:small_blue_diamond: 이중화를 적용할 경우 인프라 구축 기술 난이도 및 비용 증가의 가능성이 높음.

<br />

:two: 네트워크 구성도 파악

:small_blue_diamond: 단위 업무 시스템들의 네트워크 구성을 파악하여 그림으로 표현.

:small_blue_diamond: ​서버의 위치 및 네트워크 연결 방식 파악을 통해 조직 내 서버들의 물리적인 위치 관계를 파악할 수 있음.

:small_blue_diamond: 조직 내 보안 취약성 분석 및 대응, 네트워크 장애 발생 추적 및 대응을 하기 위한 근거로 활용 가능.

<img src="https://github.com/lee-jin-wo0/License-EngineerInformationProcessing-Study/blob/main/Part01/Chapter02/Section01/img/%EA%B7%B8%EB%A6%BC2.1.02.png" alt="그림2.1.02"  />

<br />

<br />

## 02 개발 기술 환경 식별

### 운영체제

:one: 운영체제 정의

:small_blue_diamond: 사용자가 손쉽고 효율적으로 컴퓨터 시스템을 사용하도록 돕는 소프트웨어.

:small_blue_diamond: 하드웨어와 소프트웨어 리소스를 관리하고 컴퓨터 프로그램을 위한 공통 서비스를 제공.

<br />

:two: 운영체제 종류 및 특징

:small_blue_diamond: Microsoft Windows : 다양한 라이선스 정책, 중소 규모 서버, 개인용 PC

:small_blue_diamond: UNIX : 다양한 라이선스 정책, 대용량 처리, 안정성이 요구되는 서버

:small_blue_diamond: Linux : 무료, 확장성, 다양한 버전 제공, 중대 규모 서버

:small_blue_diamond: iOS : 유료, 하드웨어에 포함, 스마트폰, 태블릿PC

:small_blue_diamond: Android : 무료, 리눅스 기반, 스마트폰, 태블릿PC

<br />

:three: 운영체제 식별 시 고려 사항

:small_blue_diamond: 신​뢰도 : 메모리 누수, 보안 취약점, 버그 등으로 인한 성능 저하 및 장애 발생 가능성.

:small_blue_diamond: 성능 : 대규모 작업 처리, 동시 사용자 요청 처리, 지원 가능 메모리 크기.

:small_blue_diamond: 기술 지원 : 공급 업체의 안정적인 기술 지원, 사용자 커뮤니티, 오픈 소스 여부.

:small_blue_diamond: 주변 기기 : 설치 가능 하드웨어, 주변 기기 지원 여부.

:small_blue_diamond: 구축 비용 : 하드웨어, 라이선스, 유지 관리 비용.

<br />

### 02 DBMS(DataBase Management System)

:one: DBMS 정의

:small_blue_diamond: 사용자, 애플리케이션, 데이터베이스와 상호 작용하여 데이터를 저장, 관리, 상호작용하는 시스템.

<br />

:two: DBMS 종류 및 특징

:small_blue_diamond: Oracle : 유료, 대규모, 대량 데이터의 안정적인 처리.

:small_blue_diamond: MS-SQL : 유료, 중소 규모 데이터의 안정적인 처리.

:small_blue_diamond: MY-SQL : 무료, 오픈 소스 관계형 DBMS.

:small_blue_diamond: MongoDB : 무료, 오픈 소스 NoSQL DBMS.

<br />

:three: DBMS 식별 시 고려사항

:small_blue_diamond: 가용성 : 백업 및 복구의 편의성, 이중화 및 복제 지원.

:small_blue_diamond: 성능 : 대용량 데이터 처리 능력, 질의 최적화.

:small_blue_diamond: 상호 호환성 : 설치 및 운용 가능한 운영체제가 다양함.

<br />

### 03 미들웨어(Middleware)

:one: 미들웨어 정의

:small_blue_diamond: 운영체제와 소프트웨어 애플리케이션 사이에 위치하여 운영체제가 제공하는 서비스를 확장하여 제공하는 소프트웨어.

:small_blue_diamond: 데이터 교환의 일관성 유지를 위해 표준화된 인터페이스를 제공.

<br />

:two: 미들웨어 식별 시 고려사항

:small_blue_diamond: 가용성, 성능, 기술 지원, 구축 비용 등을 고려해야 함.

<br />

#### 04 오픈 소스(Open Source) 소프트웨어

:one: 오픈 소스 정의

:small_blue_diamond: 소스 코드를 무료로 공개하여 제한 없이 누구나 사용 및 개작이 가능한 소프트웨어.

<br />

:two: 오픈 소스 식별 시 고려사항

:small_blue_diamond: 무료로 공개하는 범위에 따라 다양한 라이선스가 존재.

:small_blue_diamond: 사용 가능한 라이선스의 개수와 기술의 지속 가능성을 파악해야함.