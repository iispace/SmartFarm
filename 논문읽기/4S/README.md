# 제목
Continuous observation of vegetation canopy dynamics using an integrated low-cost, near-surface remote sening system

# 저자
Kim, J., Ryu, Y., Jiang, C., & Hwang, Y.

# 출처
Agricultural and forest meteorology, 264, 164-177. 2019

# 초록 내용
식생 지수(VIs), 광합성 유효 복사량(fPAR), 잎 면적 지수(LAI)를 위성 원격 탐사를 통해 지속적으로 모니터링함으로써 생물권과 대기 간 상호작용에 대한 이해가 향상되었지만, 이 세 가지 변수를 현장에서 동시에 관측하는 기술은 부족한 실정임.
이 논문에서는 이러한 문제를 해결하기 위해 기존의 저가 부품들로 스마트 지표면 센싱 시스템(Smart Surface Sensing System, 4S)를 개발하는 과정을 소개하고, 여러 종류의 위성 영상 데이터와 비교하여 4S 시스템의 정확성과 신뢰성을 검증하였음.
4S는 자동으로 VIs, fPAR, LAI 데이터를 수집하고 인터넷을 통해 서버로 전송하여 처리할 수 있는 시스템으로, 마이크로컴퓨터(Raspberry Pi), 컨트롤러(Arduino), 마이크로 카메라(Raspberry Pi Camera), LED 기반 다중 스펙트럼 분광기를 서로 연결하여 구현된 저가형 센서임. 본 센서는 온도나 습도의 변화에도 성능에 크게 영향을 받지 않음. 실험실과 현장(여름철 장마를 겪은 논)에서의 실험 결과, 벼의 생육 기간 동안 광범위한 온/습도 조건에서 R,G,B,NIR 스펙트럼 채널이 빛의 세기와 선형 관계를 보이는 것이 확인됨.  4S로 측정된 VIs와 fPAR의 값은 기준 분광기로 측정한 값과 선형 관계를 보였으며($R^2=0.98$; NDVI, $R^2$=0.96; EVI) 4S로 측정한 LAI도 기준 LAI 장비인 LAI-2200의 측정값과 선형 관계(($R^2$ = 0.76)가 관찰되었음. LED 센서로 측정한 틈 비율 기반 LAI와 마이크로 카메라로 얻은 녹색 지수(GI)를 결합함으로써, 녹색 LAI의 계절적 변화를 추적할 수 있었음.(<<=단순히 전체 잎 면적인 LAI를 보는 것이 아니라, 실제로 광합성에 기여하는 녹색 잎만을 추적함으로써 정확한 생육 상태를 파악할 수 있었다는 것).  4S 관측의 지속적이고 다양한 특성은 위성 원격 감지 제품을 평가하는 데 있어서 그 잠재력을 강조함. 4S 시스템은 다양한 공간적,시간적 규모에 걸친 생태 센서 네트워크의 확장에 유용할 것임.

# 용어 정리
|용어|설명|
|:-:|:-|
|VIs|Vegetation Indices, 식생지수|
|fPAR|Fraction of Absorbed Photosynthetically Active Radiation, 광합성 유효 복사량|
|LAI|Leaf Area Index, 엽면적지수|
|GI|Green Index, 마이크로 카메라로 촬영한 이미지에서 녹색 성분의 비율|
|Gap fraction-based LAI|LED 센서를 통해 측정한 광 투과율(틈 비율)을 기반으로 계산된 엽면적지수(LAI)|
|Green LAI|전체 LAI 중에서 광합성에 실제로 기여하는 녹색 잎의 면적만을 반영한 LAI|
|NDVI|Normalized Difference Vegetation Index|
|EVI|Enhanced Vegetation Index|
|MODIS|NASA가 육상 관측을 위해 1999년부터 운용 중인 Terra 위성과 해양 관측을 위해 2002년부터 운용중인 Aqua 위성에 탑재된 센서. 다양한 공간 해상도를 가진 총 36개의 밴드 제공.<br> 밴드 1 ~ 2(250m), 밴드 3 ~ 7(500m), 밴드 8~36(1000m)|
|LandSat 8|30m 공간 해상도의 영상을 제공하는 위성|
|Sentinel-2|10m 공간 해상도의 영상을 제공하는 위성|
|CubeSet|10x10x10(cm)크기의 초소형 위성|
|Constellations of CubeSet|CubeSat 위성 군집. 여러 개의 CubeSat을 동시에 궤도에 배치하여 서로 보완적으로 작동하게 하는 방식. 이를 통해 지구의 특정 지역을 더 자주, 더 정밀하게 관측할 수 있음.|
