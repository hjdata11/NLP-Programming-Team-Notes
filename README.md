## 자연어 처리를 위한 깃허브 공간

* 임베딩 : 사람이 쓰는 자연어를 기계가 이해할 수 있는 숫자의 나열인 벡터(vector)로 바꾼 결과 혹은 그 일련의 과정 전체를 의미

* 임베딩의 역할
  * 단어/문장 간 관련도 계산
    * 코사인 유사도 : 각 쿼리 단어별로 벡터 간 유사도 측정 기법
    * t-SNE : 차원 축소(dimension reduction) 기법으로 100차원의 단어 벡터들을 2차원으로 줄여 시각화에 사용
  * 의미적/문법적 정보 함축
    * 단어 유추 평가(word analogy test) : 단어 벡터 간 덧셈/뺄셈을 통해 단어들 사이의 의미적, 문법적 관계를 도출
  * 전이 학습
    * 전이 학습(transfer learning) : 임베딩을 다른 딥러닝 모델의 입력값으로 쓰는 기법
   
   
* 임베딩 기법의 역사와 종류
  * 통계 기반
    *잠재 의미 분석(Latent Semantic Analysis): 단어 사용 빈도 등 말뭉치의 통계량 정보가 들어 있는 커다란 행렬에 특이값 분해(Singular Value Decomposition)등 수학적 기법을 적용해, 행렬에 속한 벡터들의 차원을 축소하는 방법  \\(단어-문서 행렬(Word-Document Matrix), TF-IDF(Term Frequency-Inverse Document Frequency), 단어-문맥 행렬(Word-Context Matrix), 점별 상호 정보량 행렬(PointWise Mutual Information Matrix)
   
  * 뉴럴 네트워크 기반
    * 이전 단어들이 주어졌을 때 다음 단어가 뭐가 될지 예측
    * 문장 내 일부분에 구멍을 뚫고 해당 단어가 무엇일지 예측
  
  * 단어 수준 : NPLM, Word2Vec, GloVe, FastText, Swivel ...
  * 문장 수준 : ELMo, BERT, GPT ...
 

