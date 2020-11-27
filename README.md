# AI악성코드탐지 프로젝트
- 국민대학교 소프트웨어학부 2020-2학기 
- 정보보호와시스템보안 **윤명근 교수님**

## 프로젝트 과제
파일들의 정보에서 추출한 특징들을 이용하여 정상과 악성파일을 높은 정확도로 가려내는 AI머신러닝 프로그램을 완성한다.

## 프로젝트 멤버
- 20163148 이헌재
- 20163090 김동욱
- 20171696 장한영

## 프로젝트 목표
- 파일들의 정보를 분석하고 이 정보들 중에 다양한 특징을 사용한다.
- 주어진 데이터를 분류하여 필요한 데이터로 구성한다.
- AI를 통하여 데이터를 학습 하고 검증한다.
- 여러 알고리즘을 사용하여 결과를 앙상블한다.
- 정확도를 높이는 특징을 추출한다.

## 입력 데이터
- PEMINER
  - 학습데이터, 검증데이터, 테스트데이터.json
- EMBER
  - 학습데이터, 검증데이터, 테스트데이터.json
- PESTUDIO
  - 학습데이터, 검증데이터, 테스트데이터.json
- 학습데이터 정답.csv
- 검증데이터 정답.csv

## 솔루션
- **PEMINER**
 +기존 전체 188개의 피처중 학습을 방해하는 특징 벡터를 제거한다.
 +for문을 통해 피처를 한개씩 제거하여 정확도가 오르는 특징 벡터들을 확인
- **EMBER**
 + 기존에 있던 특징들을 수정한다.
 + 새로운 특징을 찾아 vector에 하나씩 추가하여 정확도가 증가하면 추가, 감소하면 제거한다.
- **PESTUDIO**
 + 데이터들을 완전히 확인하여 특징을 추출한다.
 + 새로운 특징을 찾아 vector에 하나씩 추가하여 정확도가 증가하면 추가, 감소하면 제거한다.
 
## 검증데이터 최종 정확도
- 0.9607
