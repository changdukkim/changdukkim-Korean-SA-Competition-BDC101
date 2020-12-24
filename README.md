## 고려대학교 컴퓨터정보통신대학원 빅데이터 자연어처리기술 기말고사 과제

### 0. 실행 환경
* Google `colab pro`환경에서 진행
* 런타임 유형: 하드웨어 가속기 (GPU), 런타임 구성 (고용량 RAM)
* `pytorch` 이용

### 1. NSMC 네이버 영화 리뷰 데이터 감정 분석
학습코드:`kor/기말고사_KOR_학습코드_model_kor_koelectra_v3_base.ipynb`  
검증코드:`kor/기말고사_KOR_검증코드_model_kor_koelectra_v3_base.ipynb`  
테스트를 용이하게 하기 위해 검증 코드와 학습 코드를 분리하였습니다. 검증코드는 미리 학습 하여 s3에 저장한 모델을 다운로드하여 테스트를 진행하게 됩니다. 



- 검증 코드 실행 방법
	1. kor 폴더로 이동
	2. `기말고사_KOR_검증코드_model_kor_koelectra_v3_base.ipynb` 파일 오픈  
	3. 모든 셀 실행을 통해 **1) test set 다운로드, 2) 모델 다운로드, 3) 검증, 4) csv 파일 변환 및 다운로드** 가능  

- 학습 코드 실행 방법
	1. kor 폴더로 이동
	2. `기말고사_KOR_학습코드_model_kor_koelectra_v3_base.ipynb `파일 오픈
	3. 모든 셀 실행을 통해 **1) 데이터 전처리, 2) 모델 구현 및 학습, 3) 모델 다운로드 가능**	
- 데이터 출처  
[https://github.com/e9t/nsmc.git](https://github.com/e9t/nsmc.git)

- 참고문헌 및 코드  
[http://kko.to/DhikTz8D0](http://kko.to/DhikTz8D0)

### 2. Friends 드라마 대본 데이터 감정 분석  
학습코드:`eng/기말고사_ENG_학습코드_model_bert_large.ipynb`  
검증코드:`eng/기말고사_ENG_검증코드_model_bert_large.ipynb`  
테스트를 용이하게 하기 위해 검증 코드와 학습 코드를 분리하였습니다. 검증코드는 미리 학습 하여 s3에 저장한 모델을 다운로드하여 테스트를 진행하게 됩니다. 



* 검증 코드 실행 방법
	1. eng 폴더로 이동
	2. `기말고사_ENG_검증코드_model_bert_large.ipynb` 파일 오픈  
	3. 모든 셀 실행을 통해 **1) test set 다운로드, 2) 모델 다운로드, 3) 검증, 4) csv 파일 변환 및 다운로드** 가능  

- 학습 코드 실행 방법
	1. eng 폴더로 이동
	2. `기말고사_ENG_학습코드_model_bert_large.ipynb `파일 오픈
	3. 모든 셀 실행을 통해 **1) 데이터 전처리, 2) 모델 구현 및 학습, 3) 모델 다운로드 가능**	
- 데이터 출처  
[http://doraemon.iis.sinica.edu.tw/emotionlines/index.html](http://doraemon.iis.sinica.edu.tw/emotionlines/index.html)

- 참고문헌 및 코드  
[https://github.com/jiwonny/nlp_emotion_classification/blob/master/friends_electra.ipynb](https://github.com/jiwonny/nlp_emotion_classification/blob/master/friends_electra.ipynb)

### 3. 다른 모델 및 학습방법
[trials readme](https://github.com/changdukkim/changdukkim-SA-Competition-BDC101/tree/main/trials)로 이동  
* 참고 문헌 및 코드:  
Electra Large, KoBERT 참고 코드:  [https://github.com/jiwonny/nlp_emotion_classification](https://github.com/jiwonny/nlp_emotion_classification)  
