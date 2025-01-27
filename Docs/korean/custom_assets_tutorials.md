# 커스텀 에셋

CARLA는 도로망, 건물, 인프라를 갖춘 완전한 마을과 도시, 시뮬레이션을 채울 차량과 보행자 등 기본적으로 사용할 수 있는 풍부한 에셋을 제공합니다. 하지만 많은 응용 프로그램에서 자신만의 에셋을 추가하고 싶을 수 있으며, CARLA는 최대한의 확장성을 위해 사용자가 완전히 새로 만든 에셋을 로드할 수 있습니다.

다음 문서에서는 자신만의 에셋을 만들어 CARLA에 추가하는 다양한 기술을 자세히 설명합니다.

- [__소품 추가하기__](tuto_A_add_props.md)
- [__차량 추가하기__](tuto_A_add_vehicle.md)
- [__에셋 패키징__](tuto_A_create_standalone.md)
- [__재질 커스터마이제이션__](tuto_A_material_customization.md)

## [소품 추가하기](tuto_A_add_props.md)

소품은 도로와 차량을 제외한, 장면을 채우는 에셋입니다. 여기에는 가로등, 건물, 나무 등이 포함됩니다. 시뮬레이터는 간단한 과정을 통해 언제든지 새로운 소품을 추가할 수 있습니다. 이는 맵에서 커스터마이즈된 환경을 만드는 데 매우 유용합니다. [__이 문서__](tuto_A_add_props.md)에서는 커스텀 소품을 만들고 포함하는 방법을 보여줍니다.

## 차량 추가하기

차량은 CARLA의 핵심입니다. 차량은 다른 도로 사용자를 시뮬레이션하고 자율 에이전트가 제어하도록 설계된 차량의 가상 에뮬레이션 역할을 합니다. CARLA는 기본적으로 크고 계속 성장하는 차량 라이브러리를 보유하고 있지만, 특수한 응용을 위해 맞춤 설계된 차량을 로드할 수 있습니다. [__이 문서__](tuto_A_add_vehicle.md)에서는 커스텀 차량을 만들고 가져오는 방법을 자세히 설명합니다.

## 에셋 패키징

CARLA에서는 독립 패키지로 에셋을 관리하는 것이 일반적인 관행입니다. 에셋을 따로 보관하면 빌드 크기를 줄일 수 있습니다. 이러한 에셋 패키지는 언제든지 CARLA 패키지로 쉽게 가져올 수 있습니다. 또한 에셋을 체계적으로 쉽게 배포하는 데 매우 유용합니다. [__이 문서__](tuto_A_create_standalone.md)에서는 CARLA에서 사용할 에셋을 패키징하는 방법을 보여줍니다.

## 커스텀 재질

CARLA 팀은 모든 에셋이 특정 기본 설정에서 실행되도록 준비합니다. 하지만 소스에서 빌드하는 사용자는 자신의 필요에 가장 잘 맞도록 이를 수정할 수 있습니다. [__이 문서__](tuto_A_material_customization.md)에서는 이를 달성하는 방법을 보여줍니다.