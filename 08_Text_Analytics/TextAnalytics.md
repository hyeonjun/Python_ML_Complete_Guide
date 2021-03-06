### NLP? 텍스트 분석?
* NLP는 머신이 인간의 언어를 이해하고 해석하는 데 더 중점을 두고 기술 발전.
    * 언어를 해석하기 위한 기계 번역, 질의응답 시스템 등
    * 텍스트 분석을 향상하게 하는 기반 기술
* 텍스트 분석(=텍스트 마이닝)은 비정형 텍스트에서 의미 있는 정보를 추출하는 것에 좀 더 중점을 두고 기술 발전.
    * 머신러닝, 언어 이해, 통계 등을 활용해 모델을 수립하고 정보를 추출해 비즈니스 인텔리전스(Business Intelligence)나 예측 분석 등의 분석 작업을 주로 한다.

### 텍스트 분석의 기술 영역
* 텍스트 분류(Text Classification) : Text Categorization. 문서가 특정 분류 또는 카테고리에 속하는 것을 예측하는 기법. 지도학습
* 감성 분석(Sentiment Analysis) : 텍스트에서 나타나는 감정/판단/믿음/의견/기분 등의 주관적인 요소를 분석하는 기법. 지도학습 + 비지도학습
* 텍스트 요약(Summarization) : 텍스트 내에서 중요한 주제나 중심 사상을 추출하는 기법. ex) 토픽 모델링(Topic Modeling)
* 텍스트 군집화(Clustering)와 유사도 측정 : 비슷한 유형의 문서에 대해 군집화 수행하는 기법. 문서들 간의 유사도를 측정해 비슷한 문서끼리 모을 수 있는 방법.

# 텍스트 분석
* 비정형 데이터인 텍스트를 분석.
* 피처 벡터화(Feature Vectorization, 피처 추출) : 텍스트를 단어 기반의 다수 피처로 추출하고 이 피처에 단어 빈도수와 같은 숫자 값을 부여하여 텍스트를 단어의 조합인 벡터값으로 변환하는 것
* 변환 방법 : BOW(Bag of Words), Word2Vec

### 텍스트 분석 수행 프로세스
1. 텍스트 전처리 : 클렌징, 대소문자 변경, 특수문자 삭제 등, 단어 등의 토큰화 작업, 의미 없는 단어 제거, 어근 추출(Stemming/Lemmatization) 등의 텍스트 정규화 작업
2. 피처 벡터화/추출 : 전처리 된 텍스트에서 피처를 추출하고 벡터값 할당. ex) BOW - Count 기반, TF-IDF 기반, Word2Vec
3. ML 모델 수립 및 학습/예측/평가 : 피처 벡터화된 데이터 세트에 ML 모델 적용하여 학습/예측 및 평가 수행

### 파이썬 기반 NLP, 텍스트 분석 패키지
* NLTL(Natural Language Toolkit for Python) : 파이썬의 대표적인 NLP. 수행 속도 측면에서 아쉬운 부분이 있어 실제 대량의 데이터 기반에서는 제대로 활용되지 못함
* Gensim : 토픽 모델링 분야에서의 대표적인 패키지. SpaCy와 함께 가장 많이 사용됨
* SpaCy : 뛰어난 수행 성능으로 최근 가장 주목받는 NLP 패키지.
