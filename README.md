<img width="700" alt="스크린샷 2022-09-14 오후 3 09 49" src="https://user-images.githubusercontent.com/97447841/190073314-b827ea68-d503-4b9c-b803-97aa514f3723.png">

Date : 2022.3.17~2022.3.22

Tags : `sklearn` `Regression` 

Link : [https://github.com/heezzing/Project2.git](https://github.com/heezzing/Project2.git) 

발표영상 : [https://youtu.be/zvVHcPlQEOk](https://youtu.be/zvVHcPlQEOk)

## 개요

- 주제 : 국방비 예측 데이터 (나라별 군사비 규모를 예측하기 위해 선정)
- 베이스라인 : 단순선형회귀
    - 국방비 규모라 분류보단 회귀가 맞다고 생각하여 회귀를 선택함
- 평가지표 : • 회귀 평가지표(evaluation metrics): MAE,MSE,RMSE,R^2
- 데이터 출처  :  Kaggle
    
    [Military expenditure by country from 1970-2020](https://www.kaggle.com/datasets/prasertk/military-expenditure-by-country-from-19702020)
    
- 기여 내용 : 주제도출, 스토리텔링, 데이터 분석, 발표자료
- 종속변수 : M_USD
- 독립변수 : **M_of_gov,M_of_GDP**

## 프로젝트 내용

<img width="700" alt="스크린샷 2022-09-14 오후 3 10 32" src="https://user-images.githubusercontent.com/97447841/190073426-c7936889-4d25-484c-a3b9-e1a9070bad9b.png">

- 주제는 국방비 예측 데이터입니다.
- 주제를 선택한 이유 :
    - 우크라이나와 러시아의 전쟁을 보며 내가 누리고 있는 안전이 언제든이 없어질 수 있다고 느끼게 되었고 국가와 국민을 지키기 위해 각 나라별 국방비에 어느정도 투자하는지 궁금하여 선정하게 되었습니다.
- 가설은 GDP대비 국방비 비율과 국가지출 대비  국방비 비율이 국방비에 큰 영향을 미친다 입니다.

<img width="700" alt="스크린샷 2022-09-14 오후 3 11 02" src="https://user-images.githubusercontent.com/97447841/190073503-5d090f7d-3d25-4252-8912-cd48de11daa6.png">
<img width="700" alt="스크린샷 2022-09-14 오후 3 11 17" src="https://user-images.githubusercontent.com/97447841/190073547-e5393153-12da-4ab3-8e14-72234a9dcdd5.png">

- 데이터 수집은 kaggle에서 ****military expenditure.csv****를 다운받았습니다.
- pandas를 이용하여 데이터 전처리를 해주었습니다.
    - 결츨값 처리,불필요한 컬럼 처리


<img width="766" alt="스크린샷 2022-09-14 오후 3 13 50" src="https://user-images.githubusercontent.com/97447841/190074002-d8eca87a-2b7b-415e-ba26-01961c4f4743.png">

- 베이스라인을 회귀로 잡고 선형회귀를 이용하였고 평가지표는 mse,rmse,mae,R^2를 이용하였습니다.
- 왼쪽은 GDP 대비 국방비 비율(M_of_GDP)과 국방비규모(USD)의 선형회귀선입니다.
- 오른쪽은 정부지출 대비 비율(M_of_gov)과 국방비규모(USD)의 선형회귀선입니다.
- 왼쪽의 그래프 기울기와 R^2값이 더 크므로 GDP대비 국방비 비율이 정부지출 대비 국방비 비율보다 국방비에 더 영향을 미치는걸 알 수 있습니다.

