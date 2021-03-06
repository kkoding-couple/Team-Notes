## 경영통계분석 2주차 요약 자료 - 20214025 오수열

> 본 요약 과제는 깃허브를 통해 정리하여 pdf 파일로 다운로드 하였습니다.<br>github 주소 : http://bit.ly/3v1QeB4

<br>

# Graphical Descriptive Techniques

> **그래프 기술통계**<br>
>
> : 자료를 기술하는 것을 기술통계라 한다. 이를 데이터 시각화를 통한 그래프로 표현하면 자료의 특성과 패턴을<br>직관적이고 쉽게 알아볼 수 있다. 
>
> * 데이터 시각화 과정을 거칠때 그래프나 도표는 명료하고 흥미로우며 설득력이 있어야 한다.
> * 데이터 시각화는 먼저 체계적이고 논리적인 방법을 통해 데이터 값을 시각적 속성으로 변환한 다음,<br>그 속성들로 최종 그래프를 만드는 과정으로 이루어진다.

<br>

## 다양한 시각화 방식

> 데이터의 형태 혹은 목적에 따라 사용할 수 있는 시각화 방식 정리해 본다.

<br>

### 수량의 시각화

> 데이터 시각화 작업에서는 수치 집합의 크기를 나타내야 할 때가 많다.<br>수량을 시각화 하는 가장 흔한 방법은 막대를 가로나 세로로 그리는 것이다.

<br>

* 수량의 시각화 예시

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/amounts-1.png" width="600" height="150"/>

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/amounts_multi-1.png" width="600" height="300"/>

<br>

> * **도수분포표(frequency distribution)** : 같은 항목, 같은 숫자 자료가 몇개 있는지를 정리 (범주형 자료/숫자형 자료)
> * **막대그래프(bar chart)** : 명목형 자료를 그래프로 표시
> * **묶은 막대그래프(grouped bar chart)** : 수량 값을 지닌 범주가 둘 이상일때 막대들을 그룹으로 묶어서 만든 그래프
> * **누적 막대그래프(stacked bar chart)** : 수량 값을 지닌 범주가 둘 이상일때 막대들을 그룹으로 쌓아서 만든 그래프

<br>

### 분포의 시각화

> 데이터셋 안에서 특정 변수가 어떻게 분포되어 있는지를 파악

<br>

* 분포의 시각화 예시

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/single-distributions-1.png" width="600" height="150"/>

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/multiple-distributions-1.png" width="600" height="300"/>

<br>

> * **히스토그램(histogram)** : 숫자형 자료(양적 자료)를 도수분포표를 이용해 그래프 형태로 표현
> * **줄기-잎 전시(stem-and-leaf display)** : 히스토그램을 옆으로 돌려 놓은 형태
> * **밀도 도표(density plot)** : 데이터의 분포를 비율로 나타내어 보여주는 그래프
> * **QQ 도표(qq plot)** : 관찰된 데이터 포인트가 주어진 분포를 따르는 범위와 따르지 않는 범위를 판단할때 유용한 그래프
> * **박스플롯, 상자그림(boxplot)** : 다섯숫자요약(최솟값/일사분위수/중앙값/삼사분위수/최댓값)을 이용하여 그래프로 표현
> * **바이올린 도표(violin plot)** : 분포 값의 전반적인 변화 추이를 중점적으로 보려고 할때 유용한 그래프<br>바이올린 도표의 경우 어떤 경우든 박스플롯을 대체할 수 있고, 데이터의 미묘한 차이를 훨씬 선명하게 보여준다.

<br>

### 비율의 시각화

> 데이터가 조각으로 나뉘었을때 전체에서 차지하는 비율을 표현한다.<br>한 집단에서의 성비, 정당의 득표율, 기업의 시장 점유율 등을 예로 들 수 있다.

<br>

* 비율의 시각화 예시

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/proportions-1.png" width="600" height="150"/>

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/proportions-multi-1.png" width="600" height="150"/>

<br>

> * **파이차트(pie chart)** : 한 항목이 차지하는 크기를 파이의 비율(=각도) 크기로 바꾸어 표현
> * **모자익그림(mosaic plot)** : 여러 그룹화 변수에 따라 비율 값이 정해지는 경우에 유용한 그래프
> * **트리맵(treemap)** : 모자익그림과 관련있지만 확실한 차이를 나타내는 방식
> * **평행좌표그림(parallel coorinates plot)** : 다변량 자료를 이차원 평면에 나타내고 해석

<br>

### x-y 관계로 나타내는 시각화

> 여러 정량 변수의 관계를 시각화 하는 방식

<br>

* x-y 관계 시각화 예시

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/basic-scatter-1.png" width="600" height="150"/>

<img src="https://clauswilke.com/dataviz/directory_of_visualizations_files/figure-html/xy-lines-1.png" width="600" height="150"/>

<br>

> * **산점도(scatter plot)** : 짝으로 되어 있는 두 개의 자료를 나타낼때 사용 (양/음의 선형 관계)
> * **버블차트(bubble chart)** : 산점도 그래프에 변수를 하나 더 추가하여 원의 사이즈로 표현
> * **시계열 그림(time series plot)** : x축이 나타내는 데이터가 시간 또는 증가하는 수치인 경우에 주로 사용하는 꺽은선 그래프

<br>

### 기타 표 or 그래프

> * **분할표** : 둘 이상의 변수들에 대한 이차원 또는 다차원 형태의 도수분포표
> * **종횡비** : 그래프를 그릴 때 시각적인 느낌에 영향을 주는 경향성 (우상향/우하향)
> * **특잇값** : 자료를 기입하거나 정리할 때 특이하게 아주 크거나 작은 값

<br>

## R 시각화 도구 (ggplot2)

> ggplot2 패키지
>
> * 통계 프로그래밍 언어 R에 대한 데이터 시각화 패키지

<br>

* 패키지 설치 및 준비

```R
# ggplot2 패키지 설치
install.packages("ggplot2")

# ggplot2 패키지 불러오기
library(ggplot2)
```

<br>

* 그래프 그리기

```R
# 기본 형식 :　데이터(축)　+　그래프 종류　+　세부 설정

# 데이터(축)
# ggplot(데이터 세트, aes(데이터 속성))
ggplot(mpg, aes(manufacturer))

# 데이터(축) + 그래프 종류
ggplot(mpg, aes(manufacturer)) + geom_bar()

# 데이터(축) + 그래프 종류 + 세부 설정
ggplot(mpg, aes(manufacturer)) + geom_bar() + coord_flip(clip = "off")
```

```r
# 데이터(축) + 그래프 종류 + 세부 설정1 + 세부 설정2
ggplot(mpg, aes(manufacturer)) + 
    geom_bar() + 
    coord_flip(clip = "off") + 
    theme(axis.text.y=element_text(size=17))
```

<br>

* 그래프 종류 예시

```r
geom_bar()  # 막대그래프
geom_bar(aes(fill=factor(변수)))  # 누적 막대그래프
geom_bar(aes(fill=factor(변수))) + coord_polar('y')  # 파이차트
geom_histogram(binwidth=1)  # 히스토그램
geom_density()  # 밀도 그래프
geom_boxplot()  # 그림 상자, 박스플롯
geom_violin()  # 바이올린 도표
mosaicplot()  # 모자익그림
geom_point()  # 산점도
geom_point(aes(size=변수))  # 버블차트
geom_line()  # 선그래프, 시계열그래프
geom_abline()  # 직선 추가
```

<br><br>

# Numerical Descriptive Techniques

> **수치 기술통계**<br>
>
> : 그래프를 이용하는 것과 달리 숫자를 이용하여 자료의 정보를 요약 기술하는 것을 의미한다.

<br>

### 중심위치와 척도

> 평균, 중앙값 등 표본 데이터의 중심적인 경향성을 정확하게 설명할 수 있는 기술통계
>
> * **평균(mean)** : 모든 자료의 값을 다 더한 후 전체 개수로 나눔, 산술평균(mathmetical average)라고도 함
> * **중앙값(median)** : 자료를 크시순으로 늘어 놓았을 때 가운데에 해당하는 값
> * **최빈값(mode)** : 자료 중에서 그 빈도수가 최대인 값
> * **사분위수(quartile)** : 자료를 크기 순으로 늘어놓고 똑같은 크기의 네 덩어리로 만들 때 그 경계에 해당하는 값

<br>

### 변동성 척도

> 표본의 속성을 나타내는 데이터가 얼마나 변하는지, 퍼져 있는 정도를 설명하는 기술통계
>
> * **범위(range)** : 제일 작은 값(최솟값)과 제일 큰 값(최댓값)의 거리
> * **사분위간 범위(Interquartile range, IQR)** : 범위에 의한 변동성 척도가 특잇값에 의하여 왜곡되는 경우 변동성의 척도로 사용
> * **분산(variance)** : 모든 자료가 그 평균으로부터 떨어져 있는 거리를 제곱한 것이 평균값의 분산
> * **표준편차(standard deviation)** : 분산값에 제곱근을 취한 값, 평균적으로 어느 정도가 편차가 있는지를 파악
> * **변동계수(coeffieicient of variation)** : 변동성을 평균에 대한 상대적인 값으로 표시, (표준편차/평균x100)%

<br>

### 특잇값의 발견

> 수집된 데이터에서 주목할 만큼 차이가 있는 일부 데이터
>
> * **Z-Score** : 자료에서 평균을 빼고 표준편차로 나눈 값<br>평균 = 0, 표준편차 = 1 인 표준화된 자료가 된다.

<br>

### 연관성 척도

> 둘 이상의 항목에 대한 숫자형 자료를 분석할 때 자료의 상호 연관성 측정
>
> * **공분산(covariance)** : 2개의 확률변수의 선형 관계를 나타내는 값
> * **상관계수(coefficient)** : 피어슨상관계수/곱적률상관계수<br>공분산/각 변수의 표준편차<br>상관계수를 구할 때는 산점도를 항상 그려보아야 함

<br>

### 그룹자료의 평균과 분산

> 자료의 도수분포표의 형태가 같은 그룹으로 모아져 있는 경우에는 개개의 원자료가 없으므로<br>계급의 중앙값을 그 계급이 속한 자료들의 대표값으로 사용