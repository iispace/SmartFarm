# 제목
<b>Development of a filter-based near-surface remote sensing system to retrieve far-red sun-induced chlorophyll fluorescence</b>

[Github](https://github.com/Kinznice/4S-SIF)


# 저자
Jongmin Kim, Youngryel Ryu, Benjamin Dechant

# 출처
Remote Sensing of Environment, 283, 113311. 2022  

# 초록 내용
태양 유도 엽록소 형광(SIF)의 원격 탐사를 통한 관측은 식생의 구조적 및 생리적 역학에 대한 우리의 이해를 향상시켰다. 태양 유도 엽록소 형광을 측정하기 위해 지상 센서 시스템을 활용한 연구가 활발히 진행되어 왔지만, 다양한 식물 기능형(plant functional types)에 대한 현장 관측 데이터는 여전히 부족한 실정이다. 이는 상용업 SIF 측정 시스템의 제한된 보급, 고가의 초분광 분광복사계, 그리고 현장에서의 센서 보정 및 유지 관리의 어려움 때문이기도 하다. 본 연구에서는 센서 비용을 낮추고 보다 광범위한 공간 샘플링이 가능하도록 필터 기반의 4S-SIF 시스템을 개발하였다. SIF를 추출하기 위해, 본 연구에서는 초협대역 필터(full width half maximum < 1.3nm)와 포토다이오드 검출기를 결합하여 특정 파장(757nm, 761nm, 770nm)에서의 전자기 복사를 관측하고 기준 장비로 사용된 고분광 분광복사계와 비교함으로써, 대역통과 필터의 분광 및 방사 성능이 SIF를 추출하는 데 충분히 만족스러움을 확인하였다. 특히, 4S-SIF에서 얻은 DN 값은 각 파장대에서 기준 분광복사계의 DN 값과 강한 선형 관계(R<sup>2</sup> > 0.99)를 보였다. 또한, 온도 변화로 인한 필터 투과율의 변화를 보정하기 위한 보정식을 개발하여, 야외 환경에서도 온도를 적극적으로 안정화하지 않고도 SIF를 안정적으로 추출할 수 있도록 하였다. 또한, 4S-SIF에서 측정한 SIF 신호가 기준 분광복사계 기반의 SIF 신호와 강한 선형 관계가 있다는 것도 확인하였다. 이 관계는 제초제 처리로 인해 식물의 생리적 메커니즘이 변화하고 SIF 신호에 큰 변화가 발생했을 때에도 유지되었는데((R<sup>2</sup>=0.85, relative RMSE = 0.22), 이는 4S-SIF가 SIF를 안정적으로 추출할 수 있는 시스템임을 나타낸 것이다. 4S-SIF는 다양한 공간적.시간적 규모에서 현장 기반 SIF 데이터를 수집하는 데 유용한 도구가 될 것이라고 믿는다.

# keywords
Sun-induced chlorophyll fluorescence, Photodiode, Bandpass filters, Spectroradiometer 
<br>

# 용어 정리
|용어|설명|
|:-|:-|
|SIF|태양광 유도 엽록소 형광, 식물에서 방출되는 형광 신호|
|Plant functional types(식물 기능형)|식물 종(species)이 아니라, 기능적 특성(functional traits)에 따라 식물을 분류하는 방식 <br> - C3 작물: 쌀, 밀 등 일반적인 광합성 경로 사용 작물 <br> - C4 작물: 옥수수, 사탕수수 등 고온.강광 환경에 적응한 작물 <br> - CAM: 선인장, 다육식물 등 밤에 CO<sub>2</sub>를 흡수하는 식물|
|gross primary production (GPP)|식물이나 조류 같은 광합성 생물들이 태양 에너지를 이용해 CO<sub>2</sub>를 유기물로 전환하는 총량. 즉, 광합성을 통해 생성된 총 에너지 또는 탄소량<br>GPP는 대기 중 CO<sub>2</sub> 흡수량을 나타내므로 탄소 순환을 이해하는 데 핵심 지표임<br>GPP가 높다는 것은 식생이 활발히 성장하고 있다는 의미 |
|Vegetation phenology|식생의 생물계절학. 식물의 생장과 계절적 변화 과정을 연구하는 분야<br> - 발아(Germination)<br> - 잎 발달(Leaf-out)<br> - 개화(Flowering)<br> - 결실(Fruiting)<br> - 낙엽(Leaf senescence) 등의 항목 관찰|
|cropland|경작지|
|O₂A 밴드<br>(Oxigen A-band)|산소 분자가 태양광을 흡수하는 특정 파장대로, 대략 760.7nm 근처의 근적외선 영역에 위치<br> - 이 영역은 대기 중 산소(O₂)가 태양광을 강하게 흡수하는 지점이기 때문에 식물에서 방출되는 형광(SIF) 신호가 상대적으로 두드러지게 나타나는 구간임.|
|FLD method|Fraunhofer Line Depth 기법. <br> - O₂A 밴드의 안쪽과 바깥쪽 파장대(예: 757nm, 760.7nm, 770nm)를 비교하여 SIF 추출<br> - 이 때 O₂A 밴드 중심(760.7nm)은 형광이 포함된 파장대, 바깥쪽은 형광이 없는 기준 파장대로 사용됨|
|Kautsky effect| 식물이 어둠에 적응한 상태에서 갑자기 빛을 받으면 형광이 급격히 증가했다가 감소하는 현상<br> 이 효과는 광합성 초기 반응과 엽록소 형광의 관계를 분석하는 데 유용|

## 왜 지상 기반 (near-surface) SIF 연구가 필요한가?

- 위성에서 관측한 SIF가 실제 식물의 광합성과 얼마나 잘 맞는지 확인하려면 지상에서 직접 측정한 값이 필요함.
- 위성 SIF는 대기, 구름, 센서 특성 등 다양한 변수에 영향을 받기 때문에, 지상 데이터로 보정해야 더 정확한 GPP 추정 가능
- 식물 종류, 생육 단계, 스트레스 상태 등은 위성만으로는 구분하기 어려워, 현장 데이터가 필수적임
- SIF-GPP 관계를 설명하는 생태 모델을 개선하려면 실제 지상에서 관측한 값이 필요함.
- 즉, 위성으로 식물의 생산성을 넓게 관측할 수는 있으나, 그 정확성과 의미를 제대로 이해하려면 지상에서 직접 측정한 SIF 데이터가 더 많이 필요함.

## 기존 지상 기반 SIF 시스템의 한계

- 높은 가격 => 낮은 가격의 장비 개발 필요
- 초분광 분광복사계(Spectroradiometer)를 기반으로 한 시스템은 고품질 SIF를 정확하게 추출하기 위해 요구되는 엄격한 조건들을 만족시키는 것이 실제 현장에서는 매우 어려움. => 환경 조건에 민감하지 않아 보정이 필요 없는 장비 개발 필요
- 어려운 사용 방법 : 생태학, 식물생리학, 지리학에 대한 지식이 있더라도 광학 장비나 스펙트럼 분석에 익숙하지 않은 경우 장비를 제대로 활용하기 어려움.  => 쉽게 사용할 수 있는 장비 개발 필요
- 전체 스펙트럼을 측정할 필요 없이 몇 개의 핵심 파장대만 관측하면 되는 식생 모니터링의 경우, 값비싸고 복잡한 초분광 분광복사계(spectroradiometer) 대신, 포토다이오드와 광학 필터를 결합한 다중 스펙트럼 센서 시스템을 사용하는 것도 가능(Garrity et al., 2010; Pontailler et al., 2003; Pontailler and Genty, 1996)하지만, __잎 단위(leaf scale)에서 SIF를 추출하는 연구만 있었을 뿐, 야외에서 캐노피(식물 군락) 수준의 SIF를 지속적으로 모니터링할 수 있는 시스템은 아직 개발되지 않았음__
  - Fraunhofer line depth(FLD) 기법이 O₂A 밴드의 안쪽과 바깥쪽 두세 개의 파장대만으로도 SIF를 추출할 수 있기 때문에, 포터다이오드와 필터의 조합은 SIF를 보다 간편하게 추출할 수 있는 잠재력을 가지고 있음( (Meroni et al., 2009; Plascyk, 1975).
  - SIF는 757nm 및 760.7nm와 같은 몇 개의 매우 좁은 파장대만 관측함으로써 추출할 수 있음.
  - SIF는 식물이 광합성 중 방출하는 미세한 빛인데, 이 빛은 태양광에 섞여 있기 때문에 직접적으로 측정하기 어렵다. 하지만, O₂A 밴드에서는 태양광이 산소에 의해 흡수되어 줄어들기 때문에, 그 틈을 통해 식물에서 방출되는 형광 신호(SIF)를 상대적으로 더 쉽게 감지할 수 있는 것.

## 제안 (가설)

- 현장(field)에서 SIF를 모니터링할 때 발생하는 기술적 어려움을 극복하고, 센서 비용을 낮춰 보다 넓은 공간에서 효율적으로데이터를 수집할 수 있도록 설계된 필터 기반의 스마트 근접 원격탐사 시스템(4S-SIF)를 제안함.
- SIF 관측을 위해 초협대역(ultra-narrow) 밴드패스 필터와 포토다이오드 검출기를 결합하여 특정 파장에서의 전자기 복사 에너지(빛)를 감지하는 방식으로 시스템을 구성함.
- 본 논문의 제2장인 "Materials and methods"에서는 다음의 세 가지 내용을 다룸.
  - 4S-SIF 개발 방법 설명
  - 기준 장비인 상업용 초분광 분광복사계(hyperspectral spectroradiometer)를 이용하여 4S-SIF 성능 평가
  - 제초제 처리로 인해 SIF 수준이 빠르게 변화하는 실제 야외 환경에서, 4S-SIF 시스템이 SIF를 얼마나 정확하게 추출하는지를 기준 장비와 비교하여 평가
<br>

#  Materials and methods

## 장치 디자인 및 기술 명세

- 4S-SIF의 기본 구조는 기존 연구에서 개발한 4S(Kim et al., 2019)를 기반으로 함
- Raspberry Pi b3 module, customized 3d printed structure, phosensor amplifier(C9329), internet router, silicon photodiode(S2386-18 K), and three ultra-narrow bandpass filters
  
  <img width="828" height="400" alt="image" src="https://github.com/user-attachments/assets/09d3cc2e-0c5d-4cfd-8191-0b71b1315d55" />

  <img width="876" height="600" alt="image" src="https://github.com/user-attachments/assets/67cee480-1906-4c64-9c93-3ec3f88e76a1" />

- 

