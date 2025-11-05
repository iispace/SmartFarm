# BOX 1 Definitions of leaf angles

- 여기서는 잎 각도와 관련된 여러 정의들을 요약하여 제공함. 이어서 캐노피 전체에 대해 잎 각도의 통계적 분포만을 사용하는 접근을 넘어서야 한다는 주장을 제시하며, 특히 캐노피 내에서의 공간적 분포, 그 중에서도 수직적 잎 각도 분포의 중요성을 강조하고자 함.

- 또한 식물에게 중요한 다른 각도들도 존재한다는 점을 주목할 필요가 있음. 예를 들어, 잎자루를 중심으로 잎몸이 회전하는 회전 각도(Farque et al., 2001), 잎자루 자체의 각도, 그리고 침엽수의 경우 가지 각도 등이 이에 해당함.

<img width="1299" height="757" alt="image" src="https://github.com/user-attachments/assets/ce19c134-dbf0-44ad-bdab-115c8627acd0" />


|용어|설명|
|:-|:-|
|Leaf angles|본 논문에서는 Leaf angle(LA)을  &theta;<sub>L</sub>로 표기함|
|Leaf inclination angles|잎 평면과 수평면 사이의 각도<br>- 즉, 잎이 지면에 대해 얼마나 기울어져 있는지를 나타내는 각도|
|Leaf zenith angle |잎의 법선(잎 표면에 수직인 방향)과 천정 방향(수직 방향) 사이의 각도<br>- 수학적으로는 잎 경사각(leaf inclination angle)과 동일<br>- 즉, 잎이 수직 방향에서 알마나 기울어져 있는지를 나타내는 각도|
|Leaf azimuth angle (&alpha;<sub>L</sub>)|잎의 법선(잎 표면에 수직인 방향)이 북쪽 기준으로 얼마나 회전되어 있는지를 나타내는 방위각<br>- 즉, 잎이 어느 방향을 향하고 있는지를 나타내며, 북쪽을 기준으로 측정한 수평 회전 각도라고 할 수 있음.|
|Mean laef angle(MLA)|식물 전체 캐노피의 평균 잎 각도. <br> <img width="138" height="58" alt="image" src="https://github.com/user-attachments/assets/021b34a6-be40-454a-8571-b7427ed8f0a9" /><br>- f(&theta;<sub>L</sub>): 잎 각도의 확률 밀도 함수<br>- 이 식은 0도에서 90도까지의 각도 범위에서 잎 각도와 그 확률 밀도를 곱한 값을 적문하여 평균을 구하는 방식<br>- 잎들이 수평에서 수직까지 어떤 각도로 분포되어 있는지를 통계적으로 반영함|
|The angle of incidence|잎 표면에 도달하는 직접 태양광의 입사각으로, 복사 에너지의 양에 영향을 미치는 각도<br> - 태양광이 잎에 얼마나 비스듬히 또는 직각으로 들어오는지를 나타내며, 이 각도가 작을수록 잎이 더 많은 빛을 직접적으로 흡수할 수 있음.|
|Leaf angle distribution (LAD)|특정 잎 각도에서의 잎 면적 비율의 통계적 분포<br> -  잎 각도의 확률 밀도 함수 f(&theta;<sub>L</sub>)는 일반적으로 두 개의 매개변수를 가진 베타 분포로 적합되며(de Vit, 1965), 이와 유사한 변형(Campbell, 1990) 또는 삼각함수 기반의 함수(Verhoef, 1984)로도 표현됨.<br><br> - 모델링에서 널리 사용되는 6가지 LAD 유형<br> <img width="701" height="332" alt="image" src="https://github.com/user-attachments/assets/909a462a-6ff0-4583-b7bc-9379bdeb3968" /><br> - 모델에서는 LAD를 종종 구형(spherical)으로 가정하지만(Baldocchi et al., 2002), 실제로 LAD는 종에 따라 매우 다양하며, 많은 일반적인 식물 종들은 비구형 LAD를 가지고 있음(Pisek et al.,2013; Ross, 1980).|
|G-function|복사 전달(radiative transfer) 모델링에서 널리 사용되는 개념으로, 태양광이 들어오는 방향에 수직한 평만에 투영된 잎 면적과 실제 잎 면적의 비율을 의미함(Ross, 190). <br> - G-함수는 중요한 캐노피 구조 매개변수로, 태양 천정각과 잎 각도 분포(LAD)에 따라 달라짐.<br> - 즉, 태양이 하늘에서 위치하는 각도와 잎들이 어떻게 배열되어 있는지에 따라 G-함수 값이 변하며, 이는 빛의 투과와 흡수, 에너지 흐름을 모델링하는 데 핵심 역할을 함.<br> - 더욱이 잎의 군집(clumping) 현상은 잎 각도와도 관련이 있으며, 수직 방향으로 변화한다는 것이 연구를 통해 밝혀졌음(Béland & Baldocchi, 2021; Pearcy et al., 2005)<br> - 식물 전체 캐노피에 대해 빛 투과 확률, 즉 갭 분율(P<sub>gap</sub>)은 다음과 같은 방식으로 추정됨.<br> <img width="282" height="64" alt="image" src="https://github.com/user-attachments/assets/bbfefc6e-3c61-42eb-a3c8-29e5854a96ae" /><br> - &Omega; : 잎 군집 계수<br> - cos&theta;<sub>v</sub> : 관측 천정각의 코사인 값|


- LAD(잎 각도 분포)는 복사 전달 모델과 지표면 모델에서 효율적으로 사용되어 왔으며, 일반적으로 하나 또는 두 개의 매개변수만으로 표현할 수 있음.
- 그러나, LAD는 빛과 온도의 캐노피 피로파일을 모델링하는 데 매우 중요한 캐노피 내 잎 각도의 수직적 변화에 대한 정보를 제공하지 않음.
- 예를 들어, 구형 캐노피에서 수직 잎이 소평 입포다 많은 극단적인 경우를 생각해보면,
  - 대부분의 수직 잎이 캐노피 상부에 위치한 경우와
  - 대부분의 수평 잎이 캐노피 상부에 위치한 경우를 비교할 때,
    - 전자의 경우 상부 캐노피 온도는 더 낮고, 하부는 정오 무렵 더 따뜻해질 가능성이 높다.
- 다양한 잎 각도 분포와 수직 프로파일의 4가지 예시
  - Cecropia schreberiana: 신열대림(neotropical forest)의 초기 천이종(early successional species)으로, 플라노필(planophile) LAD를 가진 대표적 사례. 캐노피 수목에서느 드물과 관찰되는 유형(Figure 3a)
  - Quercus alba(흰참나무): 온대 지역의 대표적 수목종. 상부 캐노피에서 잎 각도가 크고, 하부로 갈수록 잎 각도가 작아지는 수직 분포. 그러나 공존하는 종에 대한 수직 프로필에서 상당한 변화가 관찰되기도 함.
  - Juglans nigra(흑호두나무): 수직 프로파일에서 잎 각도의 변화가 거의 없음
  - Fagus grandifolia(아메리카 너도밤나무): 상부 캐노피에서 평균 잎 각도(MLA)가 약 20도 감소하는 뚜렷한 수직 변화(Figure 3).
 
    <img width="1015" height="752" alt="image" src="https://github.com/user-attachments/assets/27a4a689-fedd-4946-afa8-4974222c1167" />
