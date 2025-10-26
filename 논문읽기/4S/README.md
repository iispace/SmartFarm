# 제목
<b>Continuous observation of vegetation canopy dynamics using an integrated low-cost, near-surface remote sensing system</b>
<br>
[Github](https://github.com/Kinznice/Smart-Surface-Sensing-System/tree/master)

# 저자
Jongmin Kim, Youngryel Ryu, Chongya Jiang, Yorum Hwang

# 출처
Agricultural and forest meteorology, 264, 164-177. 2019

# 초록 내용
식생 지수(VIs), 광합성 유효 복사량(fPAR), 잎 면적 지수(LAI)를 위성 원격 탐사를 통해 지속적으로 모니터링함으로써 생물권과 대기 간 상호작용에 대한 이해가 향상되었지만, 이 세 가지 변수를 현장에서 동시에 관측하는 기술은 부족한 실정임.
이 논문에서는 이러한 문제를 해결하기 위해 기존의 저가 부품들로 스마트 지표면 센싱 시스템(Smart Surface Sensing System, 4S)을 개발하는 과정을 소개하고, 여러 종류의 위성 영상 데이터와 비교하여 4S 시스템의 정확성과 신뢰성을 검증하였음.
4S는 자동으로 VIs, fPAR, LAI 계산을 위한 데이터를 수집하고 인터넷을 통해 서버로 전송하여 처리할 수 있는 시스템으로, 마이크로컴퓨터(Raspberry Pi), 컨트롤러(Arduino), 마이크로 카메라(Raspberry Pi Camera), LED 기반 다중 스펙트럼 분광기를 서로 연결하여 구현한 저가형 센서임. 본 센서는 온도나 습도의 변화에도 성능에 크게 영향을 받지 않음. 실험실과 현장(여름철 장마를 겪은 논)에서의 실험 결과, 벼의 생육 기간 동안 광범위한 온/습도 조건에서 R,G,B,NIR 스펙트럼 채널이 빛의 세기와 선형 관계를 보이는 것이 확인됨.  4S를 이용하여 산출된 VIs와 fPAR의 값은 기준 분광기로 측정한 값과 선형 관계를 보였으며($R^2=0.98$; NDVI, $R^2$=0.96; EVI) 4S를 이용한 LAI도 기준 LAI 장비인 LAI-2200의 측정값과 선형 관계(($R^2$ = 0.76)가 관찰되었음. LED 센서로 측정한 틈 비율 기반 LAI와 마이크로 카메라로 얻은 녹색 지수(GI)를 결합함으로써, 녹색 LAI의 계절적 변화를 추적할 수 있었음.(<<=단순히 전체 잎 면적인 LAI를 보는 것이 아니라, 실제로 광합성에 기여하는 녹색 잎만을 추적함으로써 정확한 생육 상태를 파악할 수 있었다는 것).  다양한 데이터를 지속적으로 측정할 수 있는 특성을 가진 4S는 위성 원격 감지 제품을 평가하는 데 잠재력이 있음. 4S 시스템은 다양한 공간적,시간적 규모에 걸친 생태 센서 네트워크의 확장에 유용할 것임.
<br>

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
|MODIS|NASA가 육상 관측을 위해 1999년부터 운용 중인 Terra 위성과 해양 관측을 위해 2002년부터 운용중인 Aqua 위성에 탑재된 센서. 다양한 공간 해상도를 가진 총 36개의 밴드 제공.<br> 밴드 1 ~ 2(250m), 밴드 3 ~ 7(500m), 밴드 8~36(1000m). 동일 지역 재방문 주기는 하루 또는 이틀로 짧은데다가 Terra와 Aqua의 촬영 시간이 달라(예: 오전, 오후) 적절히 사용하면 동일 지역을 짧은 간격으로 모니터링 가능|
|LandSat 8| 미국 지질조사국(USGS)이 NASA와 공동 운영하는 지구 관측 위성. Landsat 프로그램의 8번째 위성. 30m 공간 해상도의 영상을 제공하는 위성, 총 11개의 촬영 밴드(가시광선, 근적외선, 단파장 적외선, 열적외선 등), 동일 지역을 최소 16일마다 촬영|
|Sentinel-2| 유럽우주국(ESA)이 운영하는 지구 관측 위성 시리즈로 Copernicus 프로그램의 핵심 구성 요소 중 하나. 10m, 20m, 60m 공간 해상도(밴드별로 다름), 총 13개 밴드, 동일 지역을 최소 5일마다 촬영|
|CubeSet|10x10x10(cm)크기의 초소형 위성|
|Constellations of CubeSet|CubeSat 위성 군집. 여러 개의 CubeSat을 동시에 궤도에 배치하여 서로 보완적으로 작동하게 하는 방식. 이를 통해 지구의 특정 지역을 더 자주, 더 정밀하게 관측할 수 있음.|
|K3100 Solar Cell chamber| K3100이라는 모델의 IPCE(Incident Photon-to-Current Efficiency) 측정 시스템. 특정 파장의 빛을 선택적으로 방출하고, 그 빛에 대한 태양전지 또는 광센서의 반응을 측정함.|
|solar irradiance|태양 복사량|
|spectral reflectance|스펙트럼 반사율|

<br><hr>

# Materials and methods

- <b>Calibration and evaluating the LED:</b> 적색, 녹색, 청색 및 근적외선(NIR) 영역의 스펙트럼 파장 대역이 MODIS 스펙트럼 대역[(UserGuide 참고)](#userguide_modis)과 일치하는 LED를 선택하기 위해서, 스펙트럼 선택적 광을 방출하는 태양전지 챔버(K3100 태양전지 IPCE 측정 시스템, Mc Science, 수원, 대한민국)를 사용하여 다양한 종류의 LED를 테스트하였으며, 그 결과로 다음과 같은 파장을 가진 R,G,B,NIR LED를 선택하고 각 LED의 FWHM 값을 확인함(FWHM 값을 알면 파장의 범위도 알 수 있음).
  
<div align="center">
<img width="521" height="192" alt="image" src="https://github.com/user-attachments/assets/b0ee8e90-3fc2-401c-b645-d0d688b0f0dd"/>
</div>

- <b>Cover the LED sensors with Teflon diffuser:</b> 유입되는 빛이 LED 헤드 인클로저 내부로 완전히 확산되도록 하기 위해 LED 센서를 테플론으로 덮어 분광 조도 측정
  
- <b>LED sensor calbiration:</b> LED 센서 보정을 위해, 다양한 복사 강도(광량의 정도: 60 ~ 1000W/m<sup>2</sup>) 조건에서 LED(LED 센서)에서 출력된 전압값(DN, Digital Number)을 코사인 보정기가 설치된 FieldSpec 4 Wide-Res Field Spectroradiometer라는 고정밀 야외용 분광복사계로 측정한 spectral irradiance( 스펙트럼별 조도, 복사량, 복사 조도값)와 비교. 즉, FieldSpec 4로 350 ~ 2500nm 범위의 스펙트럼 복사조로를 1nm 간격으로 수집한 후, 수집된 데이터에서 각 LED의 FWHM과 파장 범위에 해당하는 범위의 복사조도값 추출 후 평균하여 LED 센서의 기준값으로 사용

- <b>fPAR 모니터링:</b> R,G,B LED를 조합하여(PAR =  &alpha; × red + &beta; x green + &gamma; x blue) PAR 값을 결정함. 이 때 사용된 회귀 계수 &alpha;, &beta;, &gamma;는 linear regression model을 적용하여 구함. 이렇게 구한 PAR 값은 비교 기준이 되는 값("PQS 1 PAR quantum sensor"이라는 광량 측정 센서로 측정한 PAR 값)을 이용하여 보정하는 작업을 거쳐 최종적으로  &alpha;, &beta;, &gamma; 값 설정.

<br>

# 4S 센서 설치 장소, 설치 방법, 데이터 수집 및 처리

- 설치 장소: (벼)논
- 설치 방법:
<div align="center">
  <img width="529" height="744" alt="image" src="https://github.com/user-attachments/assets/5bda8786-5ecf-4a93-a14a-aaee1c02a999" />
</div>

- 데이터 수집 및 처리:

    - 위쪽과 아랫쪽에 설치한 센서의 값을 비교하여 반사율 계산(Spectral Reflectance)
        - 위쪽 센서: 하늘에서 들어오는 빛(입사광) 측정
        - 아랫쪽 센서: 식생에서 반사된 빛 측정
        - Spectral Reflectance = 반사된 빛 / 입사된 빛
  

# 추가 내용

1. <a id="userguide_modis"></a>[MOD09_UserGuide](https://modis-land.gsfc.nasa.gov/pdf/MOD09_UserGuide_v1.4.pdf)
2. <a id="info01"></a>[MODIS 위성 영상의 활용 방법 소개](https://scienceon.kisti.re.kr/commons/util/originalView.do?cn=JAKO202030161655677&oCn=JAKO202030161655677&dbt=JAKO&journal=NJOU00291580)
3. <a id="info02"></a>MODIS 위성 영상 획득 사이트<br>
    - [AppEEARS](https://lpdaacsvc.cr.usgs.gov/appeears)
    - [Earth Data Search](https://www.earthdata.nasa.gov/)
    - [EarthExplorer](https://earthexplorer.usgs.gov/)
   
   
