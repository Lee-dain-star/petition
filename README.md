# K-평균 클러스터링을 이용한 국민청원 내용과 동의 수 분석
## Analysis of National petition contents and number of consent using K-Means Clustering
---
## 요약(abstract)
 본 논문에서는 K-평균 클러스터링을 활용하여 청원내용과 동의 수의 분포를 분석한다. 청원을 crawling 
한 후, 각 청원을 twitter 형태소 분석기 (okt)로 토큰화 (tokenize) 한다. 그리고 scikit-learn의 TF-IDF를 
활용하여 특성 단어의 빈도수에 따라 벡터화하고 문서에 대한 중요도를 수치화한다. 또한, 가중치에 따라 
정렬된 내용의 특징 벡터를 PCA, T-SNE 알고리즘을 이용해 차원 축소하여 시각화하고 K-평균 연산으로 
나눠진 cluster 별 데이터들의 키워드를 추출한다. 마지막으로 K-평균 클러스터링 그래프를 통해 cluster 
별 동의 수의 평균, 표준편차, 최댓값, 최솟값을 구했으며, 이를 통해 청원내용과 동의 수 분포를 시각적
으로 표현함으로써 국민청원의 실태를 살펴본다.

## 목차 (contents)
1. 서론
2. 관련 연구
3. 실험 방법
   1. 데이터 수집 및 전처리
   2. TF-IDF 벡터화
   3. K-means clustering algorithm
   4. 청원내용 특징분포, 시각화
4. 실험 결과
5. 결론 및 향후 연구계획
6. 참고문헌

## 실험 결과
그림1. PCA, T-SNE Cluster 시각화 결과
![image](https://user-images.githubusercontent.com/57992071/110309414-a89e2500-8044-11eb-805e-9add2466c2be.png)

그림2. 청원내용 (text)과 투표 수(vote)   
![image](https://user-images.githubusercontent.com/57992071/110309512-c7042080-8044-11eb-8384-17df04a9b7b7.png)

표1. 각 Cluster의 상위 키워드 추출
![image](https://user-images.githubusercontent.com/57992071/110309457-b5bb1400-8044-11eb-849d-38bac8261db2.png)
![image](https://user-images.githubusercontent.com/57992071/110309476-bce22200-8044-11eb-9c7d-797c7fa227ae.png)
