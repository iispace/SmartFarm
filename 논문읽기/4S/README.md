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
이 논문에서는 이러한 문제를 해결하기 위해 기존의 저가 부품들로 스마트 지표면 센싱 시스템(Smart Surface Sensing System, 4S)을 개발하는 과정을 소개하고, 기준 장비로 측정한 데이터 및 여러 종류의 위성 영상 데이터와 비교하여 4S 시스템의 정확성과 신뢰성을 검증하였음.
4S는 자동으로 VIs, fPAR, LAI 계산을 위한 데이터를 수집하고 인터넷을 통해 서버로 전송하여 처리할 수 있는 시스템으로, 마이크로컴퓨터(Raspberry Pi), 컨트롤러(Arduino), 마이크로 카메라(Raspberry Pi Camera), LED 기반 다중 스펙트럼 분광기를 서로 연결하여 구현한 저가형 센서임. 본 센서는 온도나 습도의 변화에도 성능에 크게 영향을 받지 않음. 실험실과 현장(여름철 장마를 겪은 논)에서의 실험 결과, 벼의 생육 기간 동안 광범위한 온/습도 조건에서 R,G,B,NIR 스펙트럼 채널이 빛의 세기와 선형 관계를 보이는 것이 확인됨.  4S를 이용하여 산출된 VIs와 fPAR의 값은 기준 분광기(Jaz spectrometer)로 측정한 값과 선형 관계를 보였으며($R^2=0.98$; NDVI, $R^2$=0.96; EVI), LAI도 기준 LAI 장비인 LAI-2200의 측정값과 선형 관계(($R^2$ = 0.76)가 관찰되었음. LED 센서로 측정한 틈 비율 기반 LAI와 마이크로 카메라로 얻은 녹색 지수(GI)를 결합함으로써, 녹색 LAI의 계절적 변화를 추적할 수 있었음.(<<=단순히 전체 잎 면적인 LAI를 보는 것이 아니라, 실제로 광합성에 기여하는 녹색 잎만을 추적함으로써 정확한 생육 상태를 파악할 수 있었다는 것).  다양한 데이터를 지속적으로 측정할 수 있는 특성을 가진 4S는 위성 원격 감지 제품을 평가하는 데 잠재력이 있음. 4S 시스템은 다양한 공간적,시간적 규모에 걸친 생태 센서 네트워크의 확장에 유용할 것임.
<br>

# 용어 정리
|용어|설명|
|:-:|:-|
|VIs|Vegetation Indices, 식생지수|
|fPAR|Fraction of Absorbed Photosynthetically Active Radiation, 광합성 유효 복사량. 식물이 흡수한 PAR(약 400 ~ 700nm) 범위의 빛의 비율로 식물의 광합성 능력과 생장 상태를 평가하는 지표|
|LAI|Leaf Area Index, 엽면적지수|
|GI|Green Index, 마이크로 카메라로 촬영한 이미지에서 녹색 성분의 비율|
|GF|Gap Fraction, 식물 캐노피에서 빛이 통과할 수 있는 빈 공간의 비율. 즉, 잎 사이의 틈을 통해 빛이 얼마나 들어오는 지를 측정하는 값|
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

# 4S
<img width="484" height="354" alt="image" src="https://github.com/user-attachments/assets/3a736160-8913-40fd-a5ec-233de3937b2f" />
<br>
<img width="500" height="355" alt="image" src="https://github.com/user-attachments/assets/04a3fa6c-fe18-482d-828d-77e1aa252678" />

<br>


# 4S 센서 설치 장소, 설치 방법, 데이터 수집 및 처리

- 설치 장소: (벼)논
- 설치 방법:
<div align="center">
  <img width="529" height="744" alt="image" src="https://github.com/user-attachments/assets/5bda8786-5ecf-4a93-a14a-aaee1c02a999" />
</div>

- 실험 데이터 수집 및 처리:

    - 위쪽과 아랫쪽에 설치한 센서의 값을 비교하여 반사율(&rho;) 계산(Spectral Reflectance)
        - 위쪽 센서: 하늘에서 들어오는 빛(입사광) 측정
        - 아랫쪽 센서: 식생에서 반사된 빛 측정
        - Spectral Reflectance (&rho;) = 반사된 빛 / 입사된 빛
    
    - <img width="367" height="112" alt="image" src="https://github.com/user-attachments/assets/53428a0e-7bfd-45c9-944d-a29de1cab879" />
    
      - &rho; : Spectral Reflectance
      - G : a gain factor (2.5)
      - C<sub>1</sub> : 6  (one coefficient of the aerosol resistance term)
      - C<sub>2</sub> : 7.5 (the other coefficient of the aerosol resistance term)
      - L : 1 (soil adjustment factor)
      - 위에 나열한 값들(&rho;, G, C<sub>1</sub>, C<sub>2</sub>, L)은 선행 연구를 참조한 값인 듯.(Huete et al., 2002, Jiang et al., 2008))
 
    - 9600 bps로 수집된 LED 데이터를 분당 평균 데이터로 저장.
    - NDVI와 EVI는 분당 평균 데이터를 이용하여 매분 계산하여 30분 간격으로 평균 계산
    - 넓은 면적(180°)을 가진 Jaz 분광기(코사인 보정기를 부착한 고정밀 분광복사계)와 4S를 비교하기 위해 4쌍의 LED(센서)에서 얻은 데이터를 평균화하여 비교함. (예: Green LED 4개의 값을 평균값 1개로 처리)
    
    - fPAR 계산: 철제 데크 위에 설치된 세 개의 LED 센서 세트를 사용하여 입사광(PAR incoming), 반사광(PAR reflected), 투과광(PAR transmitted)를 측정함. 각 세트는 위쪽(zenith)과 아랫쪽(nadir) 방향으로 장착된 LED센서를 말함.
        - 입사광과 반사광은 NDVI 및 EVI를 측정하던 동일한 3개의 붐(지지대)에서 모니터링되었고, 간헐적으로 관개되는 논에서 투과광을 측정하기 위해서는 LED 센서를 각 4S 시스템과 함께 스티로폼 부표에 고정하여, 수위에 따라 수직으로 움직이는 정사각형 철제 프레임 안에 설치
        - <img width="306" height="56" alt="image" src="https://github.com/user-attachments/assets/fbb5ab40-da68-483a-aae4-2b86b9afe3ef" />
        
    - LAI 계산: 캐노피 위와 아래에 설치된 LED 센서의 블루 밴드를 통해 입사 스펙트럼 복사조도 값(spectral irradiance)을 측정하여 Gap Fraction(GF) 계산 (캐노피의 산란 효과를 최소화하기 위해 블루 밴드 사용. 파란색 빛은 식물 캐노피에서 산란이 가장 적은 파장대임. 적색이나 근적외선 등 다른 파장대는 잎에 의해 산란되거나 흡수되기가 더 쉬워서 정확한 광 투과량 측정이 어려움)
    - <img width="325" height="65" alt="image" src="https://github.com/user-attachments/assets/0918942f-32f8-4c72-9a9c-b61c117fa189" /> (GF는 쉽게 말해서 식물 잎 사이로 하늘이 보이는 비율)

    - &Omega;<sub>e</sub> = 평균 ln(GF(&theta;)) / 실제 ln(GF(&theta;))  (식물의 잎이 균일하게 퍼져 있지 않으면, 측정 위치에 따라 광 투과량이 달라지고 LAI 계산이 부정확해질 수 있으므로, &Omega;<sub>e</sub>를 통해 잎의 뭉침 정도를 보정해 주는 것이 필요)
      
    - <img width="147" height="60" alt="image" src="https://github.com/user-attachments/assets/87772b39-f3c7-4c0a-9967-321d3e7fad85" />
    
        - k: the extinction coefficient under diffuse sky conditions (소광계수)
        - &Omega;<sub>e</sub> : element clumping index  (식물 캐노피-덮개구조-의 잎이 얼마나 뭉쳐 있는지(군집화 정도)를 나타내는 지표

    - LED 센서로 얻은 전체 LAI를 녹색 LAI(LAI<sub>g</sub>)로 변환하기 위해 GI 계산
      
      - GI(Greenness Index): 디지털 이미지에서 녹색 성분의 상대적인 비율을 나타내는 지표. 식물의 생육 상태나 잎의 녹색 정도를 파악하는 데 사용되며, 특히 녹색 잎 면적(Green LAI)를 추정할 때 유용한 값. 
        
        <img width="195" height="52" alt="image" src="https://github.com/user-attachments/assets/b4bb4dfc-09ff-4d96-90eb-dc98c0350d97" />

          - DN<sub>r</sub>, DN<sub>g</sub>, DN<sub>b</sub>: 각각 이미지의 빨강(R), 초록(G), 파랑(B) 채널의 디지털 숫자(Digital Number)
       
      - <img width="208" height="32" alt="image" src="https://github.com/user-attachments/assets/74717399-f091-40f7-8bb0-c56ff1cfd9a5" />

 <br>
 <br>

- 참조(기준) 데이터 수집 및 처리:

  - LAI, green LAI 데이터:

    - 샘플링된 6개의 rice hills 중에서 3개의 rice hills에서 잎을 스캔(화이트보드에 붙이고 스캐너로 스캔, 300 dpi in JPEG)

      - 녹색 잎과 노란 잎은 파란색 반사율이 다르므로, 스캔 이미지로부터 파랑 채널(Blue channel)을 추출해 녹색 잎과 노란 잎을 구분.

      - 스캔 이미지에서 파랑 채널을 시각화하고, 임계값(threshold)를 적절히 설정하여 잎의 색상을 녹색과 노란색으로 구분한 후, 녹색 잎의 비율을 구함.

      - 나머지 3개의 rice hills는 80°C에서 48시간 동안 건조한 후, 잎 무게를 측정해 단위 면적당 잎 질량으로 LAI 계산 (LAI<sub>t</sub>)

      - 앞서, 스캔 이미지 분석으로 얻은 녹색 잎의 비율을 건조 샘플에 적용해 녹색 LAI(LAI<sub>g</sub>) 추정

      - 전체 잎에서 이삭이 차지하는 면적도 고려하기 위해 이삭 무게(graint weight)와 이삭의 반쪽 표면적(hemi-surface grain area)도 보조 지표로 측정

  - VIs 데이터

    - Jaz 분광기로 측정한 스펙트럼 반사율 데이터 활용해 NDVI와 EVI 계산
   
      - Jaz 분광기(Spectrometer): 고해상도 분광기, 1nm 간격으로 350 ~ 1033nm 범위의 빛 반사율을 측정할 수 있는 장비
      - Jaz 분광기로 측정한 스펙트럼 반사율 데이터를 1분 간격으로 저장.
      - 태양 고도가 높고 그림자 영향이 가장 적은 정오에 측정된 Jaz 데이터만 사용해 NDVI와 EVI 계산
     
        <img width="342" height="300" alt="image" src="https://github.com/user-attachments/assets/beb5f2d0-0559-456a-89ca-9c04c2802273" />
        
        [그림 출처](https://www.mdpi.com/2311-7524/10/8/828)


  - LAI와 fPAR 데이터
 
    - LAI-2200 Plant Canopy Analyzer 장비 사용: 2주 간격으로 정오(noontime)에 25개 이상의 임의 포인트(논의 특정 지점)에서 데이터 수집
    - 캐노피 위에서 입사광과 반사광, 캐노피 아래에서 투과광을 각각 측정
    - LAI-2200은 서로 다른 시야각(7°, 23°, 38°, 53°, 68°)을 가진 5개의 링(ring)으로 구성. 각 링은 특정 각도에서 들어오는 빛을 감지하며, 넓은 각도일수록 더 많은 하늘을 볼 수 있음.
   
    - <img width="275" height="51" alt="image" src="https://github.com/user-attachments/assets/2a0627c7-0341-4c4a-abf3-ceadbf46d022" />
 
    - LAI with scattering correction: LAI-2200 장비로 수집한 데이터를 기반으로 FV2200 software를 사용하여 계산함.
   
    <img width="231" height="293" alt="image" src="https://github.com/user-attachments/assets/3456078f-7815-4d6e-9236-33cc26326bed" />


- 위성 원격 센싱 데이터:

  - 필드 관측 결과를 MODIS Terra, MODIS Aqua, Landsat 8, SEntinel-2 Level 2A 위성 데이터와 비교함.
  - 이 위성 데이터들은 서로 다른 공간 해상도를 가지고 있음.
    
    |위성 데이터|공간 해상도| 촬영 주기|기타|
    | :-: | :-: | :-: | :-: |
    |MOD09GQ(MODIS Terra Surface Relection), MYD09GQ(MODIS Aqua Surface Relection products)|250m|매일|ideal quality, cloud free 등 특정 상태를 만족하는 이미지만 사용|
    |Landsat 8 reflectance products|30m|16일|구름으로 덮인 이미지는 제거|
    |Sentinel-2 Level 2A|10m|10일 (Level 2A: 대기 보정된 이미지)|구름으로 덮인 이미지는 제거|

    <br>
    
# Results and discussion

- 종합 성능
  
  - 4S 시스템은 장마철을 포함하여 작물의 생장 기간(growing season) 내내 데이터를 안정적으로 수집할 수 있었음.(LED senser data 수집율: 76%, camera data 수집율: 80%, 번개나 침수, SD card 오동작 등이 데이터 수집의 방해 요인이었음)
  - LED 센서: 온도 10 – 35°C , 습도 20 ~ 100% 사이에서 잘 동작함.
  - Jaz spectrometer와 4S 시스템의 LED 센서 중 NIR 밴드의 값이 R<sup>2</sup> = 0.98 로 높은 선형 관계를 보였음.
  
    <img width="542" height="200" alt="image" src="https://github.com/user-attachments/assets/e34e0cd4-0114-45a4-9cd3-794abb0f7331" />

- VI, fPAR 및 LAI의 계절적 변화

  - VIs(NDVI, EVI), fPAR, LAI는 계절에 따라 뚜렷한 변화를 보이며, 식물의 생육 단계와 밀접한 관련이 있음. 즉, 이 지표들은 생장기(vegetation or growth stage), 생식기(reproductive stage), 등숙기(ripening or maturation stage) 등 작물의 생리적 변화를 반영함.

  - VIs(NDVI, EVI): 4S LED sensors와 Jaz spectrometer는 재배 기간 동안 서로 잘 일치하는 VI 값을 생성했음 (R<sup>2</sup> = 0.96).

    - 모종 시점(transplating date) 근처: 4S 시스템과 Jaz 분광기로 측정한 VIs 값들이 약간 차이가 발생함 -> 이는 공간적으로 이질적인 물의 탁도(논 물의 탁도가 위치마다 다름)에 기인한 것으로 가정함(assumed).
    - 초기 생장기(after DOY 140): NDVI와 EVI가 급격히 증가하는 구간. 이는 잎이 빠르게 자라면서 녹색 면적이 늘어나기 때문.
    - 생식기 ~ 등숙기(DOY 160 ~ 209): NDVI는 포화 상태에 도달해 거의 일정하게 유지되고, EVI는 NDVI보다 민감하게 계속 증가함.
    - 등숙기 이후(DOY 209 and onward): 잎이 노랗게 변하고 이삭이 형성되면서 NDVI와 EVI가 모두 감소함. 이는 녹색 잎의 면적이 줄어들기 때문
    - 수확 이후 (after DOY 248): NDVI와 EVI 모두 급격히 감소(sudden drop)
      
    <img width="520" height="400" alt="image" src="https://github.com/user-attachments/assets/d89953b3-df33-4b89-8b6a-78f66cd7bbc5" />

  - 4S 시스템으로 측정한 fPAR 값과 LAI-2200장비로 측정한 fPAR 값과 크기(magnitude)와 계절적 변환(seasonal pattern)가 일치함.

    - DOY 167 이전에는 벼의 키가 센서의 높이보다 낮았기 때문에 관측할 수 없었음.
    - DOY 167에 센서 설치 직후에는 4S 시스템과 LAI-2200 장비로 측정한 fPAR 값이 서로 일치하지 않았는데, 이는 두 장비의 방법론적 차이에 기인한 것으로 풀이됨. (LAI-2200은 25개 이상의 무작의 지점에서 측정한 반면, 4S 시스템은 3개 지점에 고정 설치되었기 때문)
    - 그러나, DOY 180 이후에는 두 장비의 fPAR 값이 서로 일치하였음.
    
    <img width="1065" height="420" alt="image" src="https://github.com/user-attachments/assets/71b78fc7-9826-405e-9c18-473282721e27" />


  - 4S LAI, LAI<sub>g</sub>도 크기(magnitude)와 계절적 변화(seasonal pattern) 관점에서 LAI 기준 값과 유사함을 보였음.
 
    - 4S 시스템으로 측정한 LAI는 LAI-2200 장비로 측정한 LAI와 가장 높은 상관관계(R² = 0.71)를 보임.
      <br>
      <br>
      - 소광계수(k)와 클럼핑 지수(&Omega;<sub>e</sub>)를 생장기 내내 일정하다고 가정하였으나, 이 가정이 4S 시스템으로 계산한 LAI 값에 편향(bias)을 초래할 수도 있었을 것으로 추정됨.(이전 연구에 따르면 벼의 생육 단계에 따라 잎의 각도 분포가 달라지면서, 소광계수(k)도 변화한다고 보고되었고, 클럼핑 지수도 이식 시점부터 생장기 절정까지는 점차 감소하고, 수확 직전에는 다시 증가하는 경향을 보인다고 하였음)
      - 실제로 DOY 200(연중 200일 째, 대략 7월 중순)까지는 4S LAI 값이 다른 기준(reference) LAI 값보다 낮게 나오는 경향이 있었음.
      - <b>계절적으로 변하는 소광계수(k)와 클럼핑 지수(&Omega;<sub>e</sub>)는 4S 시스템으로 계산한 LAI 값에 상당한 영향을 줄 수 있지만, 현재의 4S 시스템으로는 그 변화를 감지하거나 반영할 수 없었다고 함.</b>
 
      
    <img width="864" height="350" alt="image" src="https://github.com/user-attachments/assets/7eb7d42f-fd29-4d4a-8fef-beb978a5d007" />

<br>
<br>

- 위성 원격 감지 데이터 평가에 대한 의미:

  - 4S 시스템으로 측정한 NDVI 데이터가 위성 기반 NDVI보다 더 유용하고 안정적이었음. 특히 기상 조건(구름 등)에 덜 영향을 받았고, 데이터 누락이 더 적었다는 점은 4S의 강점임.
  - 구름이 없는 맑은 날씨라고 가정하더라도 1day, 10days, 16days 간격으로만 촬영하는 위성 데이터와 달리 4S 시스템은 연속적으로 데이터 획득이 가능함.
  - 4S는 지상에 설치된 센서이므로, 구름, 대기 오염, 기상 변화와 같은 조건에 용향을 거의 받지 않지만, 위성은 구름이 많거나 대기 상태가 나쁘면 관측이 불가함.
  - 결과적으로 4S는 데이터 누락이 적고 연속성이 높음.
  - 벼의 생장 기간인 125일 중에, 4S는 28일만 데이터 수집에 실패하여 전체의 약 78% 이상을 안정적으로 수집하였으나, Sentinel-2는 좋은 품질의 이미지가 단 6장, Landsat 8은 단 2장 뿐이었음. MODIS는 매일 촬영은 가능하지만 80% 이상은 구름 때문에 품질이 낮거나 사용이 불가능함.
  - 구름에 의한 위성 데이터 오염 문제를 해결하기 위해 MODIS, Landsat, Sentinel-2 등 다양한 위성의 데이터를 조합하면 구름 없는 시기의 데이터를 더 많이 확보할 가능성은 있음.
  - 최근에는 소형 위성(CubeSat)의 군집(Constellation)을 활용해 매일 지표면 변화를 3m ~ 5m의 고해상도로 관측하는 것이 가능해짐.
  - 그러나, CubeSat은 센서 품질이 낮거나 센서 간 일관성이 부족할 수 있으므로, CubeSat의 표면 반사율(Surface reflection) 데이터의 정확도 검증과 보정이 필요함.
  - 4S 시스템은 현장에서 실제 반사율 데이터를 제공할 수 있으므로, CubeSat의 정확도 검증과 보정에 중요한 역할을 할 수 있음.
 
  - 지상에서 4S 시스템이 연속적으로 측정한 NDVI를 통해, 고해상도 위성이 저해상도 위성보다 더 정확한 관측 결과를 제공한다는 점을 입증함.
  - 4S 시스템은 공간적, 시간적으로 고해상도의 기준 센서의 역할을 할 수 있음. (작은 구역에서 세밀하고 연속적인 데이터를 제공할 수 있으므로)

- Opportunities:
  
  - 기존에는 경험적 추정 방식에 의하여 fPAR, VIs, LAI 와 같은 지표를 산출할 때, 어느 하나의 지표를 이용하여 또 다른 지표를 추정하는 방식(예: NDVI로 PAR 추정 등)이 일반적이었으나, 4S 시스템은 모든 지표를 직접 측정할 수 있음.
  - 4S 시스템을 이용하여 실제 측정한 결과, NDVI는 거의 일정하게(약 0.8) 유지되었지만 fPAR와 LAI는 하늘 조건에 따라 크게 달라짐을 확인함. 따라서, fPAR과 NDVI 사이의 선형 관계에 기반한 기존 경험적 모델은 신뢰성이 낮을 수 있으며, 직접 관측이 더 정확함을 보임.)

 <img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/e353b690-4af1-4275-a893-49527ab3945b" />

  - 4S 시스템의 카메라는 RAW 형식으로 이미지를 저장할 수 있는데, RAW 형식의 이미지는 압축되지 않은 원본 이미지로써, 픽셀당 빛의 강도 정보를 그대로 보존하므로 이를 통해 식물 캐노피의 구조(잎의 밀도, 색상, 틈새 등)를 더 정밀하게 분석할 수 있음.
  - JPEG은 감마 보정(gamma correction)을 적용하여 raw 이미지를 압축하므로, 빛의 강도와 픽셀 값 사이의 관계가 비선형적임. 이는 실제 빛의 양을 정량적으로 분석하기 어렵게 만듦.
  - 반면, raw 형식의 이미지는 빛 강도에 대한 선형 반응을 보이므로, 빛의 양을 직접 수치화(quantify)할 수 있고, 광 투과율, 그림자, 색상 변화 등 정밀 분석이 가능함.
  - 또한, raw 형식의 이미지는 더 많은 비트 깊이(예: 12 ~ 14 bit)로 저장되므로, 더 넓은 밝기 범위에 색상 정보를 담을 수 있음. JPEG은 8 bit로 저장되며, 압축 과정에서 세부 정보가 손실됨.
  - 실제 실험을 통해 4S 카메라의 디지털 숫자(DN) 값이 빛 강도에 선형적으로 반응함을 확인함. => 이는 정량적 광 분석에 적합한 센서임을 입증하는 것.
  - 이번 연구에서는 벼의 잎 면적 지수(LAI)가 높고, 카메라가 비스듬한 각도(57°)로 설치되어 이미지에서 식물과 토양을 명확히 구분하기 어려웠음.
  - 하지만, 하늘을 배경으로 촬영하면, 식물 사이의 틈(gap fraction, GF)을 분석할 수 있는 가능성이 있음. 이러한 가능성은 선행 연구를 통해 이미 다양한 캐노피 구조와 하늘 조건에서 테스트된 바 있음.
    
<br>

# Conclusion

- LED sensors, micro-camera, microcontroller, internet module을 하나로 통합하여 식물의 캐노피 구조를 모니터링하고, 여러 지표를 동시에 정확하게 측정할 수 있는, 저비용 원격 지표 센싱 시스템을 구현함.
- 4S 시스템에 사용된 다채널 LED 센서는 빛 강도에 대한 선형 반응을 보이며, 현장 환경(온도, 습도)에 대해 안정적임.
- 4S 시스템을 벼의 전체 생육 기간동안 논에 설치하여 테스트한 결과, 4S 시스템의 성능은 Jaz 분광기(VIs), LAI-2200(fPAR, LAI), 실험실에서 파괴적인 방법으로 측정한 LAI(전체 LAI, 녹색 LAI)와 동일한 수준임을 확인함.
- 4S 시스템에서 LED 센서와 디지털 커메라를 결합해 녹색 LAI(green LAI)의 계절 변화를 추적할 수 있었음. 이 녹색 LAI는 작물 생육 모니터링에 필수적인 지표임.
- 또한, 4S는 위성 원격 감지 제품 평가에 유용할 수 있다는 것도 발견함.
- 4S가 다양한 규모로 생태 감지 네트워크 연구를 발전시킬 것으로 기대함.
- 4S의 모든 소스코드와 하드웨어 정보는 [깃허브](https://github.com/Kinznice/Smart-Surface-Sensing-System)에 공개하였음.


<hr>

# 추가 내용

1. <a id="userguide_modis"></a>[MOD09_UserGuide](https://modis-land.gsfc.nasa.gov/pdf/MOD09_UserGuide_v1.4.pdf)
2. <a id="info01"></a>[MODIS 위성 영상의 활용 방법 소개](https://scienceon.kisti.re.kr/commons/util/originalView.do?cn=JAKO202030161655677&oCn=JAKO202030161655677&dbt=JAKO&journal=NJOU00291580)
3. <a id="info02"></a>MODIS 위성 영상 획득 사이트<br>
    - [AppEEARS](https://lpdaacsvc.cr.usgs.gov/appeears)
    - [Earth Data Search](https://www.earthdata.nasa.gov/)
    - [EarthExplorer](https://earthexplorer.usgs.gov/)
   
   
