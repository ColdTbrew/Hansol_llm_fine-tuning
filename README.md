# Hansol_llm_fine-tuning
도배 하자 질의 응답 처리 : 한솔데코 시즌2 AI 경진대회
[![대회정보](./pngs/dacon.png)](https://dacon.io/competitions/official/236216/overview/description)  
- 대회 바로가기 이미지 클릭
- 이번 시즌 2에서는 한 걸음 더 나아가, NLP(자연어 처리) 기반의 QA (질문-응답) 시스템을 통해 도배하자와 관련된 깊이 있는 질의응답 처리 능력을 갖춘 AI 모델 개발에 도전합니다.

## Member   
### 
  **최승혁**  
  [Dacon](https://dacon.io/myprofile/472402/home)
  [Github](https://github.com/ColdTbrew)

----------------------------------------------------------
## 데이터  
![데이터 프리뷰](./pngs/data_preview.png)  
### train.csv
    id : 질문 - 답변 (QA) 샘플 고유 번호  
    질문_1, 질문_2 : 샘플 별 동일한 내용으로 구성된 질문 2개  
    category : 질문 - 답변 (QA) 샘플의 도메인 세부 분야  
    답변_1, 답변_2, 답변_3, 답변_4, 답변_5 : 샘플 별 질문에 대한 동일한 답변 Reference 5개  

### test.csv
    id : 평가 질문 샘플 고유 번호
    질문 : 평가 샘플의 질의 내용

### sample_submission.csv 
    id : 평가 질문 샘플 고유 번호  
    vec_0, vec_1 ... vec_511 : 생성된 답변을 512 차원의 Embedding Vector로 표현된 결과  

## 평가 산식
    평가 산식 : Cosine Similarity (코사인 유사도)
    Public score : 전체 테스트 데이터 중 사전 샘플링된 40%
    Private score : 전체 테스트 데이터 100%

    
----------------------------------------------------------
# ViT-Adapter  


