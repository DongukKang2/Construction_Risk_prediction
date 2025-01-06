# Construction_Risk_prediction

### Published paper
**Title**: "Development of Document Classification Model for Deriving The Construction Risk Based on Machine Learning Using Construction Project Documents"

**Author**: Dong-Uk Kang, Min Geon Cho, Gi-Chun Cha, Seung Hee Park

**Journal**: KOREAN SOCIETY OF CIVIL ENGINEERS

**DOI**: [https://doi.org/10.12652/Ksce.2023.43.6.0841]
### Abstract
건설프로젝트는 공기 지연, 건설 재해 등 다양한 원인으로 인한 리스크가 존재한다. 이러한 건설 리스크를 기반으로 건설프로젝트의 공사 기간의 산정 방법은 주로 감독자 경험에 의존한 주관적 판단으로 이루어지고 있다. 또한, 공기 지연과 건설 재해로 지연된 건설프로젝트 일정을 맞추기 위한 무리한 단축 시공은 부실시공 등의 부정적인 결과를 초래하며, 지연된 일정으로 인한 사회 기반 시설물 부재로 경제적 손실이 발생한다. 이러한 건설프로젝트의 리스크 해결을 위한 데이터 기반의 과학적 접근과 통계적 분석이 필요한 실정이다. 실제 건설프로젝트에서 수집되는 데이터는 비정형 텍스트 형태로 저장되어 있어 데이터를 기반으로 한 리스크를 적용하기 위해서는 데이터 전처리에 많은 인력과 비용을 수반하기 때문에 텍스트 마이닝을 활용한 데이터 분류 모델을 통한 기초자료를 요구한다. 따라서, 본 연구에서는 건설프로젝트 문서를 수집하여 텍스트 마이닝을 활용하여 SVM(Support Vector Machine) 기반의 데이터 분류 모델을 통해 리스크 관리를 위한 문서 기초자료 생성 분류 모델을 개발하였다. 향후 연구 결과를 통해 정량적인 분석을 통해서 건설프로젝트 공정관리 등에 있어 효율적이고 객관적인 기초자료로 활용되어 리스크 관리가 가능해질 것으로 기대된다.
### Figures
<p align="center">
<img src="Average Performance.png" width="1000px"/>
</p>

<p align="center">
<img src="Construction Work Breakdown Structure(WBS) Classification Criteria.png" width="500px"/>
</p>

<p align="center">
<img src="Predictive Performance of Machine Learning Algorithms Using Data normalization.png" width="500px"/>
</p>

This repository contains the code(not providing dataset) for the following paper.

## ⚠️ 보안 안내
- 본 폴더에는 민감한 리스크 분석 데이터가 포함되어 있어 GitHub에 원본 데이터는 제외되었습니다
- 실제 데이터는 내부 시스템에서 별도 관리됩니다

## 📋 데이터 설명
각 폴더는 다음과 같은 데이터를 포함합니다:

- l0.수발신공문: 리스크 관련 공문 자료
- l1.리스크 구간분류: 리스크 평가 구간 분류 데이터
- l2.리스크 wbs분류: 작업 분류 체계별 리스크 데이터
- l3.리스크 그룹화: 리스크 그룹 분류 데이터
- l4.리스크 기초자료: 기초 분석용 리스크 데이터
- l5.리스크 확률분포: 리스크 확률 분석 데이터

## 🔒 데이터 접근
- 데이터 접근이 필요한 경우 프로젝트 관리자에게 문의부탁드립니다.
- email : kkdu7964@gmail.com
