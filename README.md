# SVM
SVM은 대표적인 군집화 분류기법
SVM에서 가장 중요한 인자는 커널 

군집과 분류의 차이를 알아야 함
군집 : 무리를 모으는 분석 , 학생들의 특성을 파악해서 유사한 속성끼리 모아 반을 확정 , 데이터를 보고 유사한 성질과 특성 또는 규칙에 따라 데이터를 묶는 작업 , 최종 개수는 사전에 알수 없음 , 기준을 탐사하고 나누는 것
분류: 무리를 나누는 분석 - 처음부터 나눌 대상이 있음 , 이미 설정된 체계와 규칙 또는 조건에 따라 데이터를 분리, 이미 개수가 정해져 있음 , 정해진 기준을 대상에 적용

#대상 집단을 구분 짓는 기준선을 결정하는 모델이 SVM
새로운 데이터가 입력되면 해당 데이터가 속한 범주를 찾기 위해 대상이 된 집단의 범주를 설정하기 위한 작업을 수행
SVM은 구분 마진을 가장 큰 쪽으로 결정하는 것 : 마진을 최대화 하는것

#import sklearn.svm as skv
#SVM_Model=skv.SVC(kernel='linear',C=1)
#C는 모델 구현시 발생되는 오류를 얼마나 수용할 것인지 결정하는 인지
#모델을 구현하고 정확도를 확인하며 C 값을 조절하고 정확도를 높혀주는 것
#기본이 1
#kernel 은 분류모델을 결정하는 인자 linear : 선형 모델
#다항식(polynomial커널: 2차원에서 3차원으로 표현)
#RBF(기본값): 가우시안 커널 : 2차원의 점을 무한한 차원의 점으로 변환 
