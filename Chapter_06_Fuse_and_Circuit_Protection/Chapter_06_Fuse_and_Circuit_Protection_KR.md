**Volume 02. Wire Harness Engineering**

# Chapter 06. Fuse and Circuit Protection

## 06.01. Wire Protection Philosophy

![](images/image1.png){width="7.268055555555556in" height="7.268055555555556in"}

보호 장치 설계(Wire Protection)는 단순한 공학적 원칙에서 시작한다. 보호 장치(Protective Device)는 단순히 전기 부하(Electrical Load)를 보호하기 위한 것이 아니라, 기본적으로 도체(Conductor)와 그 주변 시스템을 보호하기 위해 설치된다. 퓨즈(Fuse) 또는 회로 차단기(Circuit Breaker)는 도체 온도가 절연체(Insulation), 커넥터(Connector), 단자(Terminal), 주변 부품 또는 구조 재료를 손상시킬 수 있는 수준에 도달하기 전에 비정상 전류(Abnormal Current)를 차단해야 한다. 이러한 철학은 보호 설계를 와이어 크기 선정(Wire Sizing) 이후에 추가되는 부가 기능이 아니라 와이어 하니스 설계(Wire Harness Design)의 필수 요소로 정의한다.

정상 작동(Normal Operation) 상태에서 와이어는 부하 전류(Load Current)를 전달하며, 전기 저항(Electrical Resistance)에 의해 전달되는 전력의 일부가 지속적으로 열로 변환된다. 하니스(Harness)는 이 열을 방출하여 도체 또는 절연체의 허용 온도(Allowable Temperature)를 초과하지 않도록 설계된다. 그러나 과부하(Overload) 또는 단락(Short Circuit)이 발생하면 전류가 연속 운전 설계값(Continuous Design Value)을 크게 초과할 수 있다. 저항 발열(Resistive Heating)은 대략 전류의 제곱에 비례하여 증가하기 때문에 비교적 짧은 비정상 상황에서도 심각한 열적 스트레스(Thermal Stress)가 발생할 수 있다.

따라서 보호 전략(Protection Strategy)은 예상 부하 전류(Expected Load Current), 와이어 허용전류(Wire Ampacity), 환경 디레이팅(Environmental Derating), 보호 장치 특성(Protective-Device Characteristics)을 상호 조정해야 한다. 정상 운전 전류(Normal Operating Current)는 모든 관련 디레이팅 계수(Derating Factor)를 적용한 후의 도체 허용전류보다 낮아야 하며, 퓨즈 정격(Fuse Rating)은 기동 전류(Startup Current), 모터 가속(Motor Acceleration), 커패시터 충전(Capacitor Charging), 일시적인 액추에이터 피크 전류(Actuator Peak Current)와 같은 정상적인 과도 상태를 허용해야 한다. 로봇 전기 시스템(Robotic Electrical System)에서는 과도 응답(Transient Behavior)이 본질적인 특성이므로 명목 전류(Nominal Current)만으로 보호 장치를 선정해서는 안 된다.

유용한 보호 계층(Protection Hierarchy)은 개념적으로 정상 부하 전류가 보호 장치 정격보다 낮고, 보호 장치는 와이어가 열적 손상 한계(Thermal Damage Limit)에 도달하기 전에 동작하는 관계로 표현할 수 있다. 실제 관계는 하나의 전류값이 아니라 시간 의존적(Time-Dependent)이다. 와이어와 퓨즈 모두 열관성(Thermal Inertia)을 가지므로 보호 협조(Protection Coordination)는 전류-시간 거동(Current-versus-Time Behavior)을 비교해야 한다. 높은 전류가 수 밀리초 동안에는 허용될 수 있지만, 이보다 낮은 과전류라도 수십 초 동안 지속되면 동일한 도체가 손상될 수 있다.

이러한 시간-전류 관점(Time-Current Perspective)은 단순히 명목 부하 전류보다 약간 높은 퓨즈를 선정하는 방식이 충분하지 않은 이유를 설명한다. 모터(Motor), 펌프(Pump), 솔레노이드(Solenoid), DC-DC 컨버터(DC-DC Converter), 컴퓨터(Computer), 용량성 전자 부하(Capacitive Electronic Load)는 정상 상태에서도 큰 과도 전류를 발생시킬 수 있다. 퓨즈가 지나치게 빠르게 반응하면 정상 운전 중 불필요한 차단(Nuisance Opening)이 발생한다. 반대로 반응이 지나치게 느리거나 정격이 너무 높으면 하니스 자체가 사실상 퓨즈처럼 작용하여 전기적 차단이 이루어지기 전에 절연체 용융(Insulation Melting), 도체 손상(Conductor Damage), 발화(Ignition)가 발생할 수 있다.

보호 설계는 에너지원(Energy Source)에 대한 보호 장치의 위치도 고려해야 한다. 배터리(Battery) 또는 전력 분배 버스(Power Distribution Bus)에 직접 연결된 도체는 전원 단자에서 최초 보호 장치까지 전기적으로 보호되지 않은 상태로 남는다. 이 비보호 구간(Unprotected Section)에서 단락이 발생하면 하류 퓨즈(Downstream Fuse)에 의해 차단되지 않은 상태에서 고장 전류(Fault Current)가 흐를 수 있다. 따라서 보호 장치는 일반적으로 가능한 한 전원에 가깝게 배치해야 하며, 불가피한 비보호 도체 길이(Unprotected Conductor Length)는 배선 경로(Routing), 기계적 보호(Mechanical Protection), 패키징 설계(Packaging Design)를 통해 최소화해야 한다.

분기 회로(Branch Circuit)에서는 또 다른 중요한 원칙이 적용된다. 보호 장치는 상류 에너지원(Upstream Energy Source)이 과부하시킬 수 있는 가장 작은 도체(Smallest Conductor)를 기준으로 보호할 수 있어야 한다. 대형 피더(Feeder)가 여러 개의 작은 와이어로 분기되어 각각 다른 부하를 공급하는 경우, 피더에 적합한 보호 장치는 작은 분기 와이어를 보호하기에는 정격이 지나치게 높을 수 있다. 따라서 도체 허용 용량(Conductor Capacity)이 감소하는 모든 지점에서 보호 협조를 재검토하여 하류 와이어가 상류 보호 장치의 동작 임계값(Trip Threshold) 이하에서 손상되는 상황이 발생하지 않도록 해야 한다.

고장 보호(Fault Protection)는 과부하와 저임피던스 단락(Low-Impedance Short Circuit)을 모두 고려해야 한다. 과부하는 비교적 중간 수준의 초과 전류가 장시간 지속되는 형태로 나타날 수 있는 반면, 전원과 리턴 경로(Return Path) 사이의 직접 단락(Direct Short)은 주로 배터리 임피던스(Battery Impedance), 케이블 저항(Cable Resistance), 커넥터 저항(Connector Resistance), 전력 분배 부품(Distribution Component)에 의해 제한되는 매우 높은 전류를 발생시킬 수 있다. 두 종류의 고장은 서로 다른 열적 스트레스를 발생시키므로 보호 장치에 표시된 단순 전류 정격보다 전체 시간-전류 특성(Time-Current Characteristic)을 검토하는 것이 중요하다.

도체의 열적 성능(Thermal Capability)은 설치 조건(Installation Condition)의 영향을 크게 받는다. 자유 공기(Free Air) 상태에서 충분히 보호되는 와이어라도 밀집된 번들(Bundle), 전선관(Conduit), 슬리브(Sleeve), 밀폐형 인클로저(Sealed Enclosure), 고온 로봇 구획(High-Temperature Robot Compartment) 내부에서는 다르게 동작할 수 있다. 번들 디레이팅(Bundle Derating), 주변 온도(Ambient Temperature), 절연 재료(Insulation Material), 도체 단면적(Conductor Cross-Section), 배선 경로, 인접 열원(Neighboring Heat Source)은 모두 허용전류에 영향을 미친다. 따라서 보호 설계는 이상적인 카탈로그 허용전류(Catalog Ampacity)가 아니라 와이어 크기 선정 분석(Wire-Sizing Analysis) 과정에서 결정된 디레이팅 적용 하니스 용량(Derated Harness Capability)을 기준으로 해야 한다.

기계적 설계(Mechanical Design)와 전기적 보호(Electrical Protection)는 함께 작동해야 한다. 마모(Abrasion), 압착(Crushing), 반복 굽힘(Repeated Flexing), 커넥터 손상(Connector Damage), 수분 침투(Water Ingress), 오염(Contamination), 절연체 절단(Insulation Cut) 등은 기존 과전류 보호 장치가 반응하기 전에 국부적인 고장(Localized Fault)을 발생시킬 수 있으므로 퓨즈만으로 모든 하니스 고장을 방지할 수 없다. 슬리브, 전선관, 그로밋(Grommet), 클램프(Clamp), 스트레인 릴리프(Strain Relief), 이격 거리(Separation Distance), 굽힘 반경 제어(Bend-Radius Control), 보호 배선 경로(Protected Routing)는 이러한 고장의 발생 가능성을 감소시킨다. 전기적 차단은 고장의 결과를 제한하고, 기계적 보호는 고장 자체의 발생 가능성을 줄인다.

자율이동로봇(AMR, Autonomous Mobile Robot)과 모바일 로봇(Mobile Robot)에서는 전기 시스템이 고전류 구동 회로(High-Current Traction Circuit)와 컴퓨터, 센서(Sensor), 통신 장치(Communication Device), 안전 제어기(Safety Controller), 보조 부하(Auxiliary Load)를 함께 포함하므로 보호 철학이 특히 중요하다. 구동 모터(Drive Motor)는 가속 과정에서 큰 피크 전류를 요구할 수 있지만, 인지 및 컴퓨팅 전자 장치(Perception and Compute Electronics)는 안정적인 공급 전압을 필요로 한다. 따라서 보호 시스템은 하나의 고장 분기(Faulty Branch)를 격리하면서 관련 없는 중요 기능의 전원까지 불필요하게 제거하지 않아야 하며, 전체 로봇에 하나의 대형 보호 장치를 적용하기보다는 분할 전력 분배 구조(Segmented Distribution Architecture)를 구성하는 것이 바람직하다.

보호 분할(Protection Segmentation)은 고장 격리(Fault Containment)와 정비성(Serviceability)도 향상시킨다. 구동 모듈(Drive Module), 컴퓨팅 시스템(Computing System), 센서, 액추에이터(Actuator), 보조 장비(Auxiliary Equipment), 충전 관련 회로(Charging-Related Circuit)를 별도의 보호 분기로 구성하면 고장을 더욱 효과적으로 국부화하고 진단할 수 있다. 특히 특정 분기의 전원 상실이 제동(Braking), 조향(Steering), 비상 정지(Emergency Stop), 위치 추정(Localization), 통신(Communication), 제어된 종료(Controlled Shutdown)에 영향을 줄 수 있는 경우 보호 아키텍처(Protection Architecture)는 전기적 위험과 시스템 기능을 동시에 반영해야 한다. 따라서 회로 보호(Circuit Protection)는 전체 시스템 아키텍처(System Architecture)의 일부가 된다.

보호 장치 자체도 저항(Resistance), 전압 강하(Voltage Drop), 발열(Heating), 제조 공차(Manufacturing Tolerance), 노화 영향(Aging Effect)을 발생시킨다. 따라서 보호 장치 주변의 퓨즈 홀더(Fuse Holder), 단자, 버스바(Busbar), 커넥터, 크림프 인터페이스(Crimp Interface) 역시 전기적 및 열적 설계(Electrical and Thermal Design)에 포함되어야 한다. 올바른 정격의 퓨즈를 사용하더라도 단자 시스템(Terminal System)의 품질이 좋지 않으면 과도한 국부 발열(Local Heating)이 발생할 수 있다. 따라서 보호 설계는 퓨즈 소자(Fuse Element)를 이상적인 독립 부품으로 취급하는 것이 아니라 전체 전류 경로(Complete Current Path)를 평가해야 한다.

최종 목표는 제어된 고장(Controlled Failure)을 구현하는 것이다. 전기적 고장(Electrical Fault)이 절대로 발생하지 않는다고 가정할 수 없으므로, 비정상적인 에너지(Abnormal Energy)가 배선 시스템 전체로 확산되어 비가역적 손상(Irreversible Damage)을 일으키기 전에 예측 가능한 보호 요소(Protective Element)에서 차단되도록 하니스를 설계해야 한다. 적절한 와이어 보호(Wire Protection)는 도체 크기 선정(Conductor Sizing), 디레이팅(Derating), 시간-전류 협조(Time-Current Coordination), 전원 측 보호 장치 배치(Source-Side Placement), 분기 보호 분할(Branch Segmentation), 고장 전류 분석(Fault-Current Analysis), 기계적 보호, 검증 시험(Validation Testing)을 하나의 일관된 전략으로 통합한다. 이러한 기본 철학은 이후의 퓨즈-와이어 협조(Fuse-Wire Coordination), 최대 비보호 길이(Maximum Unprotected Length), 단락 전류 계산(Short-Circuit Current Calculation), 고전압 하니스 보호(HV Harness Protection)를 상세하게 설계하기 위한 기반이 된다.

## 06.02. Fuse Wire Coordination

![](images/image2.png){width="7.268055555555556in" height="7.268055555555556in"}

퓨즈-와이어 협조(Fuse-Wire Coordination)는 전기 도체(Electrical Conductor)와 보호 장치(Protective Device) 사이에 제어된 관계를 설정하여, 와이어가 허용할 수 없는 열적 상태(Thermal Condition)에 도달하기 전에 퓨즈(Fuse)가 손상 전류(Damaging Current)를 차단하도록 하는 것이다. 목적은 단순히 명목 부하(Nominal Load)에 맞는 퓨즈를 선택하는 것이 아니다. 퓨즈 정격(Fuse Rating), 와이어 허용전류(Wire Ampacity), 절연체 한계(Insulation Limit), 과도 부하 프로파일(Transient Load Profile), 환경 디레이팅(Environmental Derating), 가용 고장 전류(Available Fault Current)가 하나의 보호 시스템(Protection System)으로 함께 작동해야 한다.

기본적인 협조 관계(Coordination Relationship)는 정상 운전 전류(Normal Operating Current)에서 시작한다. 선정된 와이어는 온도, 번들링(Bundling), 전선관(Conduit) 및 기타 적용 가능한 디레이팅 계수(Derating Factor)를 반영한 후에도 예상 부하를 연속적으로 전달할 수 있어야 한다. 퓨즈는 이러한 정상 운전 전류를 불필요한 차단(Nuisance Opening) 없이 통과시켜야 한다. 동시에 퓨즈의 정격과 동작 특성은 지속적인 과부하(Sustained Overload)가 보호 대상 도체를 허용 열 한계(Allowable Thermal Limit) 이상으로 가열하지 못하도록 충분히 낮게 설정되어야 한다.

단순화된 설계 관계는 정상 부하 전류(Normal Load Current)가 퓨즈 정격보다 낮고, 동시에 퓨즈의 보호 능력(Fuse Protection Capability)이 와이어의 안전한 열적 능력(Safe Thermal Capability) 범위 내에 존재하는 형태로 표현할 수 있다. 그러나 이러한 관계를 명목 전류 정격(Nominal Current Rating)만으로 해석해서는 안 된다. 와이어 발열(Wire Heating)과 퓨즈 동작은 시간 의존적 현상(Time-Dependent Phenomenon)이므로 공학적인 협조를 위해서는 하나의 정상 상태 운전점만 확인하는 것이 아니라 관련 전류와 지속시간의 전체 범위를 비교해야 한다.

시간-전류 특성(Time-Current Characteristics)은 전류가 퓨즈 정격값 이상으로 증가할 때 퓨즈가 얼마나 빠르게 차단되는지를 나타낸다. 비교적 작은 과부하는 퓨즈가 용단(Melting)되기까지 수초 또는 수분이 필요할 수 있지만, 심각한 단락(Short Circuit)은 수 밀리초 이내에 차단될 수 있다. 보호 대상 와이어 역시 도체 질량(Conductor Mass), 저항(Resistance), 절연체, 설치 환경(Installation Environment), 방열(Heat Dissipation)에 의해 결정되는 열적 응답(Thermal Response)을 갖는다. 적절한 협조는 해당 와이어의 손상 경계(Wire Damage Boundary)에 도달하기 전에 퓨즈 동작 곡선(Fuse Operating Curve)에 따라 보호가 이루어지도록 보장한다.

두 요소의 열적 거동(Thermal Behavior)은 시간에 따른 전류의 에너지 관련 효과를 나타내는 I²t 개념(I²t Concept)을 통해서도 평가할 수 있다. 짧은 시간 동안 발생하는 고장에서 도체는 온도가 과도하게 상승하기 전에 제한된 양의 열에너지(Thermal Energy)만 견딜 수 있다. 따라서 퓨즈는 충분히 낮은 통과 에너지(Let-Through Energy)로 회로를 차단해야 한다. 이러한 고려는 가용 단락 전류(Available Short-Circuit Current)가 빠르게 매우 높은 수준까지 증가할 수 있는 고전류 배터리 시스템(High-Current Battery System)에서 특히 중요하다.

그러나 퓨즈 선정(Fuse Selection)은 정상적인 과도 전류(Transient Current)도 허용해야 한다. 전기 모터(Electric Motor)는 가속 중 정상 전류의 수 배에 해당하는 전류를 발생시킬 수 있고, DC-DC 컨버터(DC-DC Converter)와 전자 제어기(Electronic Controller)는 커패시터 돌입 전류(Capacitor Inrush)를 발생시킬 수 있으며, 액추에이터(Actuator)는 기계적 부하가 증가하는 동안 일시적인 피크 전류(Peak Current)를 요구할 수 있다. 정상 상태 전류에 지나치게 근접한 퓨즈를 선정하면 이러한 정상적인 상황에서도 퓨즈가 차단될 수 있다. 따라서 협조 설계에서는 정상 과도 전류의 크기와 지속시간을 모두 파악해야 한다.

이러한 차이는 정상 과도 상태(Normal Transient)와 실제 과부하(True Overload)를 구분한다. 수분의 1초 동안 지속되는 모터 가속 전류 펄스(Motor Acceleration Pulse)는 순간 전류가 퓨즈 정격을 초과하더라도 퓨즈가 열관성(Thermal Inertia)을 가지므로 허용될 수 있다. 반면 모터 구속(Stalled Motor), 기계적 장애(Mechanical Obstruction), 제어기 고장(Controller Failure), 비정상 부하(Abnormal Load)로 인해 더 작은 과전류가 지속되는 경우에는 오히려 더 위험할 수 있다. 퓨즈 특성은 첫 번째 조건은 허용하면서 두 번째 조건은 와이어 손상이 발생하기 전에 확실하게 차단해야 한다.

와이어 게이지(Wire Gauge)는 도체의 단면적(Cross-Sectional Area)에 따라 저항과 열용량(Thermal Capacity)이 달라지므로 협조 설계에 직접적인 영향을 미친다. 하니스(Harness)가 큰 피더(Feeder)에서 작은 분기 도체(Branch Conductor)로 전환되는 경우, 피더를 기준으로 선정된 상류 퓨즈(Upstream Fuse)는 더 작은 와이어를 충분히 보호하지 못할 수 있다. 따라서 도체 크기가 감소할 때마다 보호 설계를 다시 검토해야 한다. 일반적으로 하나의 보호 장치에 연결된 도체 중 가장 작은 도체(Smallest Conductor)가 해당 보호 방식의 적합성을 결정하는 제한 요소(Limiting Element)가 된다.

환경 디레이팅(Environmental Derating)은 퓨즈-와이어 협조를 최종 결정하기 전에 반드시 반영해야 한다. 밀집된 번들(Dense Bundle) 안에서 다른 통전 와이어들과 함께 배치된 도체는 자유 공기(Free Air) 중에 독립적으로 배치된 와이어보다 열을 효과적으로 방출하기 어렵다. 높은 주변 온도(Ambient Temperature), 보호 슬리브(Protective Sleeve), 전선관, 밀폐 채널(Sealed Channel), 주변 발열 장비(Heat-Generating Equipment)는 열적 여유(Thermal Margin)를 추가로 감소시킬 수 있다. 따라서 협조 계산에는 제한이 없는 도체의 명목 허용전류(Nominal Ampacity)가 아니라 실제 디레이팅된 와이어 허용 능력(Derated Wire Capability)을 사용해야 한다.

퓨즈의 동작 역시 설치 환경(Installation Environment)의 영향을 받는다. 높은 주변 온도는 열적 동작 특성(Thermal Operating Behavior)을 변화시킬 수 있으며, 퓨즈 홀더(Fuse Holder), 단자(Terminal), 버스바(Busbar), 커넥터 인터페이스(Connector Interface)는 접촉 저항(Contact Resistance)에 의해 추가적인 열을 발생시킨다. 명목 부품 데이터(Nominal Component Data)를 기준으로 적절하게 협조된 것으로 보이는 퓨즈라도 소형 전력 분배 장치(Power Distribution Unit) 내부에 설치되면 다르게 동작할 수 있다. 따라서 열적 검증(Thermal Verification)은 퓨즈와 와이어를 완전한 전기 어셈블리(Electrical Assembly) 내부에 실제로 설치된 상태의 부품으로 고려해야 한다.

협조 설계는 과부하 영역(Overload Region)과 단락 영역(Short-Circuit Region)을 모두 포함해야 한다. 과부하 영역에서는 과도한 전류가 도체를 과열시킬 만큼 오랫동안 지속되는지가 주요 관심 사항이다. 단락 영역에서는 극도로 높은 전류가 거의 순간적으로 손상을 일으킬 수 있는 에너지를 전달할 수 있다. 퓨즈는 가용 고장 전류에 적합한 차단 능력(Interruption Capability)을 가져야 하며, 와이어, 단자, 커넥터 또는 주변 구조물에 과도한 열에너지가 전달되지 않도록 고장을 차단해야 한다.

배터리 구동 자율이동로봇(Battery-Powered AMR)은 저전압 시스템(Low-Voltage System)에서도 매우 높은 고장 전류가 발생할 수 있으므로 특별한 주의가 필요하다. 24 V 또는 48 V 시스템은 고전압 아키텍처(High-Voltage Architecture)보다 위험성이 낮아 보일 수 있지만, 낮은 임피던스(Low Impedance)를 갖는 배터리는 시스템 구성에 따라 심각한 단락 시 수백 또는 잠재적으로 수천 암페어(Ampere)의 전류를 공급할 수 있다. 따라서 퓨즈-와이어 협조는 낮은 시스템 전압이 낮은 전기적 고장 에너지(Electrical Fault Energy)를 의미한다고 가정하지 않고 계산 또는 검증된 가용 고장 전류를 기준으로 수행해야 한다.

여러 보호 장치가 직렬로 존재하는 경우 선택적 협조(Selective Coordination)가 중요해진다. 분기 회로에서 고장이 발생하면 상류의 메인 퓨즈(Main Fuse)가 아니라 해당 분기 퓨즈(Branch Fuse)가 우선 차단되어 고장과 관계없는 로봇 기능이 계속 전원을 공급받을 수 있는 것이 바람직하다. 이를 구현하려면 각 퓨즈와 관련 와이어 사이의 협조뿐만 아니라 하류 및 상류 퓨즈 특성(Downstream and Upstream Fuse Characteristics) 사이의 협조도 필요하다. 이를 통해 국부적인 고장을 가능한 한 고장 발생 지점에 가까운 위치에서 격리하는 보호 계층(Protection Hierarchy)을 구성할 수 있다.

자율이동로봇(AMR)의 경우 이러한 계층에는 배터리 메인 퓨즈(Battery Main Fuse), 전력 분배 보호(Distribution Protection), 그리고 구동 모듈(Drive Module), 컴퓨팅 시스템(Compute System), 센서(Sensor), 액추에이터, 보조 장비(Auxiliary Equipment), 충전 인터페이스(Charging Interface)를 위한 개별 분기 퓨즈(Individual Branch Fuse)가 포함될 수 있다. 각 보호 단계는 바로 하류의 도체를 보호하면서 동시에 상류 보호 장치와 충분한 협조 여유(Coordination Margin)를 유지해야 한다. 안전한 기능적 격리(Functional Isolation)가 가능한 경우 비교적 작은 분기 고장으로 인해 전체 전력 분배 시스템(Power Distribution System)이 불필요하게 정지되지 않도록 아키텍처를 구성해야 한다.

공학적 검증(Engineering Validation)에서는 대표적인 정상 운전(Normal Operation), 기동 및 돌입 전류 이벤트(Startup and Inrush Event), 지속 과부하(Sustained Overload), 발생 가능한 단락 조건(Credible Short-Circuit Condition)을 검토해야 한다. 측정된 전류 프로파일(Measured Current Profile)을 퓨즈 시간-전류 특성과 도체 열 한계(Conductor Thermal Limit)에 비교할 수 있으며, 온도 상승 시험(Temperature-Rise Testing)을 통해 설치 조건과 디레이팅에 대한 가정을 검증할 수 있다. 커넥터, 스플라이스(Splice), 퓨즈 홀더 및 기타 저항 집중부(Resistance Concentration)는 와이어 자체가 이론적인 열적 한계에 도달하기 전에 국부 발열로 인해 실제 설계 한계를 형성할 수 있으므로 특별히 주의해야 한다.

효과적인 퓨즈-와이어 협조는 궁극적으로 의도적인 보호 우선순위(Intentional Protection Priority)를 형성한다. 즉 하니스(Harness)가 고장 요소(Failure Element)가 되기 전에 퓨즈가 제어된 희생 요소(Controlled Sacrificial Element)가 되도록 설계하는 것이다. 이 과정은 부하 분석(Load Analysis), 도체 크기 선정(Conductor Sizing), 환경 디레이팅, 과도 전류 평가(Transient-Current Assessment), 시간-전류 곡선(Time-Current Curve), I²t 거동(I²t Behavior), 고장 전류 계산(Fault-Current Calculation), 선택적 협조, 물리적 검증(Physical Validation)을 통합한다. 해당 장(Chapter)의 구조에서 이러한 협조 원칙은 최대 비보호 길이(Maximum Unprotected Length), 단락 전류(Short-Circuit Current), 고에너지 하니스 시스템(Higher-Energy Harness System)의 보호를 평가하기 위한 기반을 제공한다.

## 06.03. Maximum Unprotected Length

![](images/image3.png){width="7.268055555555556in" height="7.268055555555556in"}

최대 비보호 길이(Maximum Unprotected Length)는 전기 에너지원(Electrical Power Source)과 최초 보호 장치(Protective Device) 사이에서 해당 보호 장치에 의해 고장으로부터 보호되지 않는 도체 구간을 의미한다. 이 구간은 퓨즈(Fuse) 또는 회로 차단기(Circuit Breaker) 이전에 단락(Short Circuit)이 발생하면 배터리(Battery) 또는 전력 버스(Power Bus)에서 직접 에너지가 공급될 수 있으므로 특별한 주의가 필요하다. 따라서 설계 목표는 이러한 비보호 도체 구간(Unprotected Conductor Section)을 가능한 한 짧고 견고하며 물리적으로 안전하게 보호하는 것이다.

일반적인 오해 중 하나는 분기 회로(Branch Circuit)의 어느 위치에든 퓨즈를 설치하면 전체 와이어가 자동으로 보호된다고 생각하는 것이다. 실제로 전기적 보호(Electrical Protection)는 보호 장치의 하류(Downstream)에서만 시작된다. 배터리 케이블(Battery Cable)이 퓨즈에 도달하기 전에 상당한 거리를 지나간다면 배터리 단자와 퓨즈 사이의 모든 도체 구간은 전원 측 고장 에너지(Source Fault Energy)에 노출된다. 따라서 퓨즈의 물리적 위치(Physical Position)는 전류 정격(Current Rating) 및 시간-전류 특성(Time-Current Characteristic)만큼 중요하다.

배터리가 짧은 피더(Feeder)를 통해 퓨즈에 연결되고 이후 보호된 전력 분배 회로(Protected Distribution Circuit)로 연결되는 경우를 생각할 수 있다. 퓨즈 하류에서 단락이 발생하면 고장 전류(Fault Current)가 퓨즈를 통과하므로 퓨즈가 고장을 차단할 수 있다. 그러나 배터리와 퓨즈 사이에서 단락이 발생하면 고장 경로에 직렬로 연결된 보호 요소(Protective Element)가 없기 때문에 전혀 다른 상황이 발생한다. 이러한 차이가 최대 비보호 길이를 제한해야 하는 근본적인 이유이다.

많은 배터리 시스템(Battery System)은 내부 임피던스(Internal Impedance)가 낮기 때문에 이러한 위험이 더욱 커진다. 24 V 또는 48 V 배터리라 하더라도 낮은 저항의 도체(Low-Resistance Conductor)를 통해 연결되면 매우 높은 단락 전류(Short-Circuit Current)를 공급할 수 있다. 그 결과 발생하는 I²R 발열(I²R Heating), 전기 아크(Electrical Arcing), 도체 온도 상승(Conductor Temperature Rise), 국부적인 에너지 방출(Localized Energy Release)은 절연체 또는 주변 재료를 빠르게 손상시킬 수 있다. 따라서 낮은 시스템 전압(Low System Voltage)이 비보호 도체 길이를 관리할 필요성을 제거하는 것은 아니다.

최대 비보호 길이는 모든 전기 시스템에 동일하게 적용되는 하나의 보편적인 거리(Universal Distance)로 해석해서는 안 된다. 허용 가능한 길이는 전원의 특성(Source Characteristics), 가용 고장 전류(Available Fault Current), 도체 크기(Conductor Size), 배선 환경(Routing Environment), 기계적 보호(Mechanical Protection), 절연 특성(Insulation Properties), 커넥터 구성(Connector Arrangement), 적용되는 공학적 요구사항(Engineering Requirements)에 따라 달라진다. 실질적인 원칙은 최초 보호 장치를 합리적으로 가능한 범위에서 전원에 최대한 가깝게 배치하고, 남아 있는 비보호 구간은 위험 기반 설계(Risk-Based Design)를 통해 타당성을 확보하는 것이다.

아직 전기적 보호를 적용할 수 없는 구간에서는 물리적 배선 경로(Physical Routing)가 주요 보호 수단이 된다. 비보호 와이어는 날카로운 모서리(Sharp Edge), 가동 기구(Moving Mechanism), 고온 표면(High-Temperature Surface), 노출된 구조물 인터페이스(Structural Interface), 압착 지점(Pinch Point), 충격이나 마모(Abrasion)에 취약한 영역을 피해야 한다. 견고한 클램프(Clamp), 그로밋(Grommet), 전선관(Conduit), 슬리브(Sleeve), 채널(Channel), 적절한 스트레인 릴리프(Strain Relief)를 사용하면 절연 손상이 보호 장치 이전의 단락으로 발전할 가능성을 줄일 수 있다.

배선 경로는 비보호 양극 도체(Unprotected Positive Conductor)가 접지 구조물(Grounded Structure) 또는 리턴 구조물(Return Structure)에 접촉할 가능성도 최소화해야 한다. 배터리 구동 로봇(Battery-Powered Robot)에서는 접지 아키텍처(Grounding Architecture)에 따라 전도성 프레임(Conductive Frame), 인클로저(Enclosure), 장착 브래킷(Mounting Bracket), 전력 분배 하우징(Power Distribution Housing) 및 기타 금속 구조물이 잠재적인 고장 경로(Fault Path)를 형성할 수 있다. 따라서 기계적 이격(Mechanical Separation)과 절연 장벽(Insulation Barrier)은 짧은 물리적 길이와 함께 전원 측 도체 고장(Source-Side Conductor Fault)의 발생 가능성을 감소시킨다.

도체 단면적(Conductor Cross-Section)이 변경되는 모든 지점에서도 보호 장치의 위치를 고려해야 한다. 적절한 보호가 적용되기 전에 대형 전원 케이블(Large Source Cable)이 더 작은 도체로 전환되면 작은 와이어가 특히 취약해질 수 있다. 마찬가지로 적절한 보호 장치 이전에 버스(Bus) 또는 피더가 여러 경로로 분기되면 다수의 비보호 경로(Unprotected Path)가 형성될 수 있다. 각 분기는 상류 전원(Upstream Source)이 공급할 수 있는 고장 에너지와 해당 도체의 열적 능력(Thermal Capability)을 기준으로 평가해야 한다.

비보호 구간 내부에 위치한 커넥터(Connector)는 단자(Terminal), 접점(Contact), 노출 인터페이스(Exposed Interface), 잠재적인 기계적 고장 지점(Mechanical Failure Point)을 추가하기 때문에 별도의 고려가 필요하다. 느슨한 단자(Loose Terminal)나 손상된 커넥터는 국부적인 저항 발열(Local Resistance Heating)을 발생시키거나 인접한 전도성 구조물과 의도하지 않은 접촉을 만들 수 있다. 따라서 보호 장치 이전의 불필요한 인터페이스는 최소화해야 하며, 불가피한 전원 측 커넥터(Source-Side Connector)는 충분한 전류 용량(Current Capability), 절연(Insulation), 유지력(Retention), 기계적 강건성(Mechanical Robustness)을 가져야 한다.

배터리 위치(Battery Location)와 전력 분배 아키텍처(Power Distribution Architecture)는 보호 장치를 얼마나 전원 가까이에 배치할 수 있는지에 큰 영향을 미친다. 메인 퓨즈(Main Fuse) 또는 배터리 보호 장치(Battery Protection Unit)를 배터리에 직접 인접하여 장착하면 나머지 하니스가 시작되기 전 노출된 피더 길이를 줄일 수 있다. 패키징 제약(Packaging Constraint)으로 인해 배터리와 보호 장치를 떨어뜨려야 하는 경우에는 연결 도체가 사실상 항상 전원이 인가된 비보호 전원 케이블(Permanently Energized Unprotected Source Cable)처럼 동작하므로 강화된 기계적 보호와 엄격하게 관리된 배선 경로를 적용해야 한다.

자율이동로봇(AMR, Autonomous Mobile Robot)은 일반적으로 배터리, 메인 퓨즈, 전력 분배 장치(PDU, Power Distribution Unit), 그리고 구동 모듈(Drive Module), 컴퓨터(Computer), 센서(Sensor), 액추에이터(Actuator), 보조 장비(Auxiliary Equipment)에 전력을 공급하는 여러 보호 분기(Protected Branch)를 포함한다. 이러한 아키텍처에서 배터리와 메인 퓨즈 사이의 구간은 가장 중요한 비보호 영역(Unprotected Region)을 형성한다. 메인 보호 지점(Main Protection Point) 이후에는 추가적인 분기 퓨즈(Branch Fuse)를 통해 국부적인 보호 경계(Local Protection Boundary)를 구성하여 더 높은 용량의 상류 도체에서 발생하는 고장 에너지에 노출되는 하니스 범위를 줄일 수 있다.

충전 회로(Charging Circuit)는 하나 이상의 에너지원에서 전력이 공급될 수 있으므로 동일한 분석이 필요하다. 충전 중 하니스는 온보드 배터리(Onboard Battery), 충전기(Charger), 충전 인터페이스(Charging Interface), 중간 전력 전자장치(Intermediate Power Electronics)에 연결될 수 있다. 설계자는 발생 가능한 모든 통전 상태(Energized State)를 식별하고 각 상태에서 어떤 도체 구간이 비보호 상태로 남는지 판단해야 한다. 정상적인 로봇 운전 중에는 보호되는 구간이라도 외부 충전 장비(External Charging Equipment)가 연결되면 서로 다른 고장 에너지 경로(Fault-Energy Path)를 가질 수 있다.

서비스 및 유지보수 조건(Service and Maintenance Conditions) 역시 평가에 포함해야 한다. 정비 과정에서 커버(Cover)가 제거되거나, 커넥터가 분리되거나, 배터리가 교체되거나, 하니스 위치가 일시적으로 변경될 수 있다. 완전히 조립된 로봇에서는 적절하게 격리된 비보호 도체라도 유지보수 과정에서는 접근 가능하거나 손상에 취약한 상태가 될 수 있다. 따라서 전원 측 배선(Source-Side Wiring)은 예측 가능한 정비 작업으로 인해 통전 도체(Energized Conductor)가 공구(Tool), 섀시 구조물(Chassis Structure), 우발적인 기계적 손상(Accidental Mechanical Damage)에 쉽게 노출되지 않도록 설계해야 한다.

검증(Verification) 과정에서는 에너지원에서 최초로 유효한 보호 장치(Effective Protective Device)까지의 실제 거리를 문서화하고, 설치된 배선 경로가 의도된 설계와 일치하는지 확인해야 한다. 하니스 도면(Harness Drawing), 전기 회로도(Electrical Schematic), 패키징 레이아웃(Packaging Layout), 실제 검사(Physical Inspection)에서 비보호 구간이 일관되게 식별되어야 한다. 특히 배선 경로 변경(Routing Deviation), 선택 사양 장비(Optional Equipment), 생산 공차(Production Tolerance), 서비스 루프(Service Loop), 커넥터 위치는 실제 도체 길이를 명목 설계값보다 증가시킬 수 있으므로 주의해야 한다.

검증은 단순한 거리 측정을 넘어 수행되어야 한다. 엔지니어는 가용 단락 전류, 도체 열적 능력, 절연 강건성(Insulation Robustness), 기계적 구속(Mechanical Containment), 잠재적 고장 접촉 지점(Potential Fault Contact Point), 고장 발생 결과(Consequences of Failure)를 함께 검토해야 한다. 검사 및 시험(Inspection and Testing)을 통해 클램프 유지력(Clamp Retention), 내마모성(Abrasion Resistance), 배선 이격(Routing Clearance), 커넥터 고정 상태(Connector Security), 보호 장치 위치를 확인할 수 있다. 결국 허용 가능한 비보호 길이는 전기적, 열적, 기계적, 패키징 위험 평가(Packaging Risk Assessment)를 종합한 결과로 결정된다.

공학적 목표(Engineering Objective)는 단순히 특정 치수 제한(Dimensional Limit)을 만족하는 것이 아니라 제어되지 않은 전원 에너지(Uncontrolled Source Energy)를 직접 받을 수 있는 도체의 양을 최소화하는 것이다. 효과적인 설계는 보호 장치를 전원에 가깝게 배치하고, 비보호 분기(Unprotected Branching)와 연결부를 최소화하며, 불가피한 전원 측 배선을 강화하고, 실제 설치 구성을 검증한다. 퓨즈-와이어 협조(Fuse-Wire Coordination) 및 단락 전류 계산(Short-Circuit Current Calculation)과 함께 최대 비보호 길이는 안전한 하니스 보호 아키텍처(Safe Harness Protection Architecture)를 구성하는 기본적인 보호 경계(Protection Boundary)가 된다.

## 06.04. Short Circuit Current Calculation

![](images/image4.png){width="7.268055555555556in" height="7.268055555555556in"}

단락 전류 계산(Short-Circuit Current Calculation)은 서로 다른 전위(Electrical Potential)를 가진 도체 사이에 의도하지 않은 저저항 경로(Low-Resistance Path)가 형성될 때 흐를 수 있는 전류의 크기를 결정하는 과정이다. 와이어 하니스 엔지니어링(Wire-Harness Engineering)에서 이 계산은 고장 발생 시 와이어(Wire), 커넥터(Connector), 단자(Terminal), 퓨즈(Fuse), 전력 분배 부품(Distribution Component)이 받을 수 있는 전기적 스트레스(Electrical Stress)를 결정한다. 또한 허용할 수 없는 열적 또는 구조적 손상이 발생하기 전에 고장을 차단할 수 있는 보호 장치를 선정하기 위한 정량적 근거를 제공한다.

가장 단순한 표현은 옴의 법칙(Ohm's Law)을 따르며, 단락 전류는 대략 전원 전압(Source Voltage)을 전체 고장 루프 임피던스(Total Fault-Loop Impedance)로 나눈 값이다. 여기서 중요한 것은 와이어 저항(Wire Resistance)만이 아니라 전체 루프 임피던스(Total Loop Impedance)이다. 배터리 내부 저항(Battery Internal Resistance), 양극 및 리턴 도체(Positive and Return Conductors), 버스바(Busbar), 커넥터, 단자, 컨택터(Contactor), 스플라이스(Splice), 전력 분배 경로(Distribution Path), 그리고 고장 자체가 모두 최종 전류를 제한하는 저항 또는 임피던스에 기여할 수 있다.

단순화된 직류 시스템(DC System)의 경우 이러한 관계는 개념적으로 I_SC = V_SOURCE / Z_LOOP로 표현할 수 있다. 유도성 영향(Inductive Effect)이 작고 저항이 지배적인 경우 Z_LOOP는 전체 루프 저항(Total Loop Resistance)인 R_LOOP로 근사할 수 있다. 방정식 자체는 단순해 보이지만 정확한 계산을 위해서는 현실적인 등가 회로(Equivalent Circuit)를 구성해야 한다. 전원 전압이 낮고 가용 고장 전류(Available Fault Current)가 높은 시스템에서는 불과 몇 밀리옴(mΩ)의 저항을 누락하는 것만으로도 예측 전류가 크게 달라질 수 있다.

따라서 전원 모델(Source Model)은 가장 중요한 요소 중 하나이다. 실제 배터리는 셀(Cell), 내부 연결부(Interconnection), 버스바, 단자 및 전기화학적 거동(Electrochemical Behavior)에 의해 내부 저항이 발생하므로 이상적인 전압원(Ideal Voltage Source)이 아니다. 단순화된 고장 모델(Fault Model)에서는 배터리를 이상적인 전압원과 내부 저항이 직렬로 연결된 형태로 표현한다. 전원 저항(Source Resistance)이 낮을수록 예상 단락 전류(Prospective Short-Circuit Current)가 증가하며, 이것이 고출력 배터리 팩(High-Power Battery Pack)이 24 V 또는 48 V에서도 매우 큰 고장 전류를 공급할 수 있는 이유이다.

배터리 상태(Battery Condition) 역시 계산에 영향을 줄 수 있다. 충전 상태(State of Charge), 온도(Temperature), 셀 화학계(Cell Chemistry), 노화(Aging), 팩 구성(Pack Configuration), 제조 편차(Manufacturing Variation)는 개방 회로 전압(Open-Circuit Voltage)과 내부 저항을 변화시킬 수 있다. 따라서 보호 설계(Protection Design)는 하나의 명목 운전점(Nominal Operating Point)에만 의존해서는 안 된다. 보수적인 최대 전류 조건(Maximum-Current Case)에서는 높은 전원 전압과 신뢰 가능한 최소 전원 저항(Minimum Credible Source Resistance)을 적용할 수 있으며, 추가적인 조건에서는 더 낮은 고장 전류와 이에 따른 느린 퓨즈 동작 가능성을 검토할 수 있다.

도체 저항(Conductor Resistance)은 재료의 비저항(Material Resistivity), 도체 길이(Conductor Length), 단면적(Cross-Sectional Area)을 이용하여 계산하며 필요한 경우 온도 보정(Temperature Correction)을 적용한다. 전용 도체(Dedicated Conductor)를 통해 고장 루프가 형성되는 경우에는 나가는 경로와 리턴 경로를 모두 포함한 전체 전류 경로(Complete Current Path)를 고려해야 한다. 섀시(Chassis) 또는 다른 전도성 구조물(Conductive Structure)이 리턴 경로의 일부를 형성한다면 해당 구조물의 유효 저항(Effective Resistance)과 연결 인터페이스(Connection Interface)도 모델에 포함해야 한다. 따라서 고장 루프 길이(Fault-Loop Length)는 고장 위치까지의 단순한 물리적 거리보다 상당히 길어질 수 있다.

커넥터, 크림프(Crimp), 스플라이스, 퓨즈 홀더(Fuse Holder), 컨택터, 버스바 접합부(Busbar Joint)는 각각 작은 저항을 발생시키지만, 이들이 결합되면 저전압 고전류 시스템(Low-Voltage High-Current System)에서 상당한 영향을 미칠 수 있다. 이러한 저항값은 온도, 노화, 오염(Contamination), 접촉 압력(Contact Pressure), 제조 품질(Manufacturing Quality)에 따라서도 변화한다. 따라서 유용한 단락 모델(Short-Circuit Model)은 도체 저항과 인터페이스 저항(Interface Resistance)을 구분하고, 모든 연결부를 이상적인 영저항 접합(Zero-Resistance Junction)으로 가정하기보다는 불확실한 매개변수(Uncertain Parameter)를 식별해야 한다.

고장 위치(Fault Location)는 가용 단락 전류에 큰 영향을 미친다. 배터리에 가까운 곳에서 발생하는 고장은 일반적으로 하니스 저항(Harness Resistance)이 작기 때문에 긴 분기 회로의 끝부분에서 발생하는 고장보다 더 높은 전류를 발생시킬 수 있다. 이로 인해 서로 다른 보호 문제가 발생한다. 전원 근처의 고장(Near-Source Fault)은 극심한 피크 전류(Peak Current)와 I²t 스트레스(I²t Stress)를 발생시킬 수 있는 반면, 원거리 고장(Remote Fault)은 전류가 낮아 퓨즈 동작 시간이 길어지고 결과적으로 도체에 지속적인 열 부하(Sustained Thermal Loading)를 발생시킬 수 있다.

이러한 관계 때문에 최대 및 최소 신뢰 가능 고장 전류(Maximum and Minimum Credible Fault Current)를 모두 고려하는 것이 중요하다. 최대 고장 전류(Maximum Fault Current)는 퓨즈, 회로 차단기(Circuit Breaker), 컨택터, 커넥터 및 전력 분배 하드웨어(Distribution Hardware)가 충분한 차단 능력(Interrupting Capability)과 내전류 능력(Withstand Capability)을 갖는지 검증하는 데 필요하다. 최소 고장 전류(Minimum Fault Current)는 보호 장치가 원거리 또는 저항성 고장(Resistive Fault)을 충분히 빠르게 감지하고 차단할 수 있는지를 확인하는 데 필요하다. 따라서 보호 시스템은 발생 가능한 전체 고장 전류 범위(Credible Fault-Current Range)에서 안전하게 작동해야 한다.

단락 전류는 퓨즈 시간-전류 특성(Fuse Time-Current Characteristics)과 함께 평가해야 한다. 계산된 고장 전류가 결정되면 제조사의 특성 곡선(Characteristic Curve)을 이용하여 예상 퓨즈 차단 시간(Fuse Clearing Time)을 추정할 수 있다. 이후 이 차단 시간을 도체의 열적 한계(Conductor Thermal Limit) 및 다른 부품의 내전류 한계(Component Withstand Limit)와 비교할 수 있다. 따라서 단락 전류 계산은 단순히 암페어(Ampere) 값을 구하는 것으로 끝나는 것이 아니라 그 결과를 예상 보호 동작(Protection Behavior)과 열적 결과(Thermal Consequence)로 연결해야 한다.

I²t 개념(I²t Concept)은 고장 전류와 열적 스트레스(Thermal Stress)를 연결하는 또 하나의 중요한 방법을 제공한다. 발열은 전류의 제곱에 비례하므로 도체에 가해지는 고장 에너지(Fault Energy)는 전류 증가에 따라 급격하게 증가한다. 보호 장치는 고장 중 통과되는 에너지(Passed Energy)를 와이어 및 연결 부품이 견딜 수 있는 수준으로 제한해야 한다. 따라서 심각한 고장에서는 단순한 퓨즈 명목 전류 정격(Nominal Fuse Current Rating)보다 퓨즈의 프리-아크 I²t(Pre-Arcing I²t) 및 전체 차단 I²t(Clearing I²t) 데이터가 더 중요한 정보를 제공할 수 있다.

자율이동로봇(AMR, Autonomous Mobile Robot)에서는 배터리 메인 피더(Battery Main Feeder), 좌우 구동 모듈(Left and Right Drive Modules), 컴퓨팅 분기(Computing Branch), 센서, 액추에이터(Actuator), 보조 장비(Auxiliary Equipment), 충전 회로(Charging Circuit)에 대해 각각 별도의 계산이 필요할 수 있다. 각 경로는 서로 다른 도체 게이지(Conductor Gauge), 길이, 커넥터, 보호 장치를 갖는다. 배터리에서 측정한 하나의 단락 전류값만으로 모든 위치를 대표할 수 없는 이유는 배터리와 각각의 잠재적 고장 지점 사이의 임피던스가 전력 분배 아키텍처(Power Distribution Architecture) 전체에서 서로 다르기 때문이다.

충전 운전(Charging Operation)은 추가적인 고장 전류원(Fault-Current Source)과 경로를 만들 수 있다. 아키텍처에 따라 온보드 배터리(Onboard Battery), 외부 충전기(External Charger), DC-DC 단계(DC-DC Stage), 충전 인터페이스(Charging Interface)가 고장에 에너지를 공급할 수 있다. 따라서 정상 주행 구성(Normal Driving Configuration)이 모든 상태를 대표한다고 가정하기보다는 관련된 각각의 통전 상태(Energized State)에 대해 등가 회로를 구성해야 한다. 양방향 전력 전자장치(Bidirectional Power Electronics)와 다중 배터리 도메인(Multiple Battery Domains)이 존재하는 경우에는 특히 고장 경계(Fault Boundary)를 신중하게 정의해야 한다.

계산 불확실성(Calculation Uncertainty)은 민감도 분석(Sensitivity Analysis) 또는 최악 조건 분석(Worst-Case Analysis)을 통해 다루어야 한다. 저항 공차(Resistance Tolerance), 배터리 임피던스 변화(Battery Impedance Variation), 도체 온도, 케이블 길이, 접촉 저항(Contact Resistance), 전원 전압을 변화시켜 가능한 고장 전류 범위를 파악할 수 있다. 최대 전류를 발생시키는 매개변수 조건이 반드시 가장 까다로운 보호 조건을 만드는 것은 아니므로 이러한 분석은 특히 중요하다. 더 낮은 고장 전류가 퓨즈 차단 시간을 충분히 증가시켜 오히려 지배적인 와이어 발열 조건(Dominant Wire-Heating Case)이 될 수도 있다.

실제 검증(Practical Validation)에서는 계산 결과를 제어된 측정(Controlled Measurement), 부품 데이터(Component Data), 시스템 수준 시험(System-Level Test)과 비교할 수 있다. 직접적인 단락 시험(Direct Short-Circuit Testing)은 매우 큰 에너지를 수반하므로 적절하게 설계된 시험 시설과 절차를 사용하는 경우에만 수행해야 한다. 많은 개발 프로그램에서는 인원이나 하드웨어를 제어되지 않은 고장 에너지(Uncontrolled Fault Energy)에 불필요하게 노출하지 않으면서 보호 모델을 검증하기 위해 계산, 시뮬레이션(Simulation), 제조사 데이터(Manufacturer Data), 저항 측정(Resistance Measurement), 제한적으로 통제된 검증 시험(Controlled Verification)을 조합하여 사용한다.

완전한 단락 전류 계산(Short-Circuit Current Calculation)은 궁극적으로 전원의 공급 능력(Source Capability), 고장 루프 임피던스(Fault-Loop Impedance), 고장 위치, 보호 장치 동작(Protective-Device Behavior), 도체 열적 능력(Conductor Thermal Capability)을 서로 연결해야 한다. 그 목적은 단순히 발생 가능한 가장 큰 전류를 예측하는 것이 아니라, 발생 가능한 모든 고장(Credible Fault)이 안전하게 차단될 수 있음을 입증하는 것이다. 퓨즈-와이어 협조(Fuse-Wire Coordination) 및 최대 비보호 길이(Maximum Unprotected Length)와 함께 단락 전류 계산은 견고한 와이어 하니스 보호 아키텍처(Robust Wire-Harness Protection Architecture)를 구축하기 위한 정량적 기반(Quantitative Foundation)을 제공한다.

## 06.05. Protection for HV Harness

![](images/image5.png){width="7.268055555555556in" height="7.268055555555556in"}

고전압 하니스 보호(HV Harness Protection)는 기존의 와이어 보호(Conventional Wire Protection)를 전기 에너지(Electrical Energy)와 전압 관련 위험(Voltage-Related Hazard)이 모두 중요해지는 시스템으로 확장한 개념이다. 그 목적은 과부하(Overload) 또는 단락(Short Circuit) 상태에서 도체 과열(Conductor Overheating)을 방지하는 것뿐만 아니라 감전(Electric Shock), 아크(Arcing), 절연 파괴(Insulation Breakdown), 의도하지 않은 통전(Unintended Energization)을 제어하는 것이다. 따라서 보호 시스템은 과전류 보호 장치(Overcurrent Device), 절연(Insulation), 격리(Isolation), 스위칭(Switching), 인터록(Interlock), 배선 경로(Routing), 커넥터(Connector), 기계적 보호(Mechanical Containment)를 통합해야 한다.

고전압 하니스(HV Harness)는 일반적으로 배터리 팩(Battery Pack), 컨택터(Contactor), 프리차지 회로(Pre-Charge Circuit), 전력 분배 장비(Power Distribution Equipment), 인버터(Inverter), 모터 드라이브(Motor Drive), DC-DC 컨버터(DC-DC Converter), 충전기(Charger), 기타 고에너지 부하(High-Energy Load)를 포함하는 에너지 시스템의 일부로 작동한다. 따라서 보호는 개별 케이블만을 대상으로 하는 것이 아니라 전체 아키텍처(Complete Architecture)를 대상으로 검토해야 한다. 모든 통전 경로(Energized Path)는 과도한 전기적 또는 열적 에너지가 시스템 전체로 확산되기 전에 고장을 격리할 수 있도록 명확한 보호 경계(Protection Boundary)를 가져야 한다.

메인 고전압 퓨즈(Main HV Fuse)는 일반적으로 고에너지 전원(High-Energy Source)에 가깝게 배치하여 비보호 도체 길이(Unprotected Conductor Length)를 최소화한다. 이는 저전압 배선(Low-Voltage Wiring)에 적용되는 것과 동일한 전원 측 보호 철학(Source-Side Protection Philosophy)을 따르지만, 보호되지 않은 고전압 고장(Unprotected HV Fault)의 결과는 훨씬 심각할 수 있다. 따라서 배터리와 최초 보호 요소 사이의 케이블 구간은 배선 경로, 절연, 기계적 보호 및 고장 경로를 형성할 수 있는 구조물과의 이격(Separation)을 엄격하게 관리해야 한다.

퓨즈-와이어 협조(Fuse-Wire Coordination)는 고전압 시스템에서도 기본적인 보호 원칙이다. 퓨즈는 연속 운전 전류(Continuous Operating Current)와 정상적인 과도 상태(Transient Event)를 허용하면서, 도체 또는 연결 부품이 열적 내한계(Thermal Withstand Capability)를 초과하기 전에 과부하와 심각한 단락을 차단해야 한다. 이러한 협조에는 시간-전류 특성(Time-Current Characteristics), 도체 열적 한계(Conductor Thermal Limit), 환경 디레이팅(Environmental Derating), 가용 고장 전류(Available Fault Current), I²t 거동(I²t Behavior)에 대한 평가가 필요하다. 또한 퓨즈는 시스템 전압과 예상 고장 전류에 적합한 차단 정격(Interrupting Rating)을 가져야 한다.

전압 정격(Voltage Rating)은 퓨즈 소자가 개방될 때 발생하는 전기 아크(Electrical Arc)를 소호(Extinguishing)하면서 전류를 차단해야 하므로 특히 중요하다. 저전압에서 특정 전류를 안전하게 차단할 수 있는 장치라도 더 높은 직류 전압(DC Voltage)에서 동일한 전류를 안전하게 차단하지 못할 수 있다. 따라서 고전압 보호 장치(HV Protective Device)는 전류 능력(Current Capability)뿐만 아니라 전압 능력(Voltage Capability)을 기준으로 선정해야 한다. 적용되는 직류 차단 정격(DC Interrupting Rating)은 보호 회로에서 발생 가능한 최대 전압과 고장 조건을 충족하거나 초과해야 한다.

컨택터(Contactor)는 고전압 에너지원의 제어된 연결 및 차단(Controlled Connection and Disconnection)을 제공하지만 전용 고장 보호(Dedicated Fault Protection)를 자동으로 대체하는 장치로 취급해서는 안 된다. 컨택터는 운전 스위칭(Operational Switching)과 안전 격리(Safety Isolation)를 담당하는 반면, 퓨즈는 높은 고장 에너지(Fault Energy)에 대한 신속한 보호 기능을 제공한다. 따라서 보호 아키텍처에서는 일반적으로 두 장치를 함께 사용하여 제어 로직(Control Logic)이 비정상 상태를 감지하면 컨택터를 개방하고, 컨택터의 안전한 차단 능력을 초과하는 심각한 고장에서는 퓨즈가 고장 전류를 차단하도록 한다.

프리차지 회로(Pre-Charge Circuit)는 저항(Resistor)과 스위칭 경로(Switching Path)를 통해 고전압 전원을 하류 커패시턴스(Downstream Capacitance)에 일시적으로 연결하므로 별도의 보호 검토가 필요하다. 프리차지 저항(Pre-Charge Resistor), 릴레이(Relay) 또는 컨택터, 배선, 제어 시퀀스(Control Sequence)는 과열 없이 예상 충전 에너지를 견딜 수 있어야 한다. 저항 경로의 단락, 스위칭 장치의 용착(Welded Switching Device), 과도하게 긴 프리차지 시간(Excessive Pre-Charge Duration), 하류 단락과 같은 고장 조건도 고려하여 프리차지 회로가 제어되지 않은 에너지 경로가 되지 않도록 해야 한다.

고전압 인터록 시스템(HV Interlock System)은 고전압 커넥터, 서비스 디스커넥트(Service Disconnect), 커버(Cover), 접근 지점(Access Point)이 올바르게 조립되어 있는지를 감지함으로써 추가적인 보호 계층(Protection Layer)을 제공한다. 고전압 인터록 루프(HV Interlock Loop)는 보호된 고전압 경로의 물리적 건전성(Physical Integrity)이 상실되면 컨택터 개방을 요청할 수 있다. 인터록은 과전류 보호 또는 절연을 대체하는 것이 아니라, 물리적인 접근이나 커넥터 분리로 위험한 상태가 발생할 수 있을 때 시스템이 계속 통전되는 것을 방지하는 역할을 한다.

고전압 아키텍처가 섀시(Chassis) 또는 보호 구조물(Protective Structure)로부터 의도적으로 절연되어 있는 경우 절연 감시(Insulation Monitoring)가 중요해진다. 절연 감시 장치(Insulation Monitoring Device)는 고전압 도체와 섀시 사이의 절연 저항(Isolation Resistance)이 저하되는 것을 감지하여 두 번째 고장이 더욱 위험한 전류 경로를 형성하기 전에 이상 상태를 식별할 수 있다. 따라서 하니스 보호에는 적절한 절연 재료(Insulation Material), 커넥터 실링(Connector Sealing), 배선 이격(Routing Clearance), 오염 관리(Contamination Control), 그리고 시스템 아키텍처에서 필요한 경우 절연 상태 감시가 포함된다.

고전압 커넥터(HV Connector)는 연결되는 케이블과 동일한 보호 철학을 지원해야 한다. 전압 정격, 전류 용량(Current Capacity), 연면거리(Creepage Distance), 공간거리(Clearance Distance), 접촉 저항(Contact Resistance), 실링(Sealing), 기계적 유지력(Mechanical Retention), 접촉 방지(Touch Protection), 인터록 기능은 모두 시스템과 호환되어야 한다. 케이블이 과전류로부터 적절하게 보호되더라도 커넥터의 접촉 저항이 증가하거나, 실링 성능이 상실되거나, 부분적으로 분리되거나, 통전된 전도부(Energized Conductive Part)에 의도하지 않은 접근이 가능해지면 시스템은 여전히 위험해질 수 있다.

기계적 보호(Mechanical Protection)는 절연 손상이 기계적으로 시작된 결함을 전기적 고장(Electrical Fault)으로 전환시킬 수 있기 때문에 특히 중요하다. 고전압 케이블(HV Cable)은 마모(Abrasion), 압착(Crushing), 반복 굽힘(Repeated Bending), 날카로운 모서리(Sharp Edge), 충격(Impact), 과도한 인장력(Excessive Tension), 고온 표면(High-Temperature Surface)으로부터 보호되어야 한다. 클램프(Clamp), 전선관(Conduit), 슬리브(Sleeve), 그로밋(Grommet), 스트레인 릴리프(Strain Relief), 제어된 굽힘 반경(Controlled Bend Radius)은 로봇 또는 차량의 수명 동안 절연 건전성(Insulation Integrity)을 유지하는 데 도움을 준다. 또한 배선 경로는 구동 모듈(Drive Module), 매니퓰레이터(Manipulator), 기타 가동 어셈블리(Moving Assembly)에서 발생하는 진동과 움직임도 고려해야 한다.

저전압 전력(Low-Voltage Power), 통신(Communication), 신호 배선(Signal Wiring)과의 이격은 안전성과 시스템 건전성(System Integrity)을 모두 향상시킨다. 고전압 도체는 적절한 물리적 이격과 교차 지점(Crossing) 또는 공유 인터페이스(Shared Interface)의 보호를 갖는 통제된 배선 경로를 따라야 한다. 설계에서는 고전압 절연 고장(HV Insulation Failure)이 저전압 회로, 통신 네트워크, 센서 배선 또는 접근 가능한 구조물을 통전시킬 가능성을 줄여야 한다. 명확한 하니스 식별(Harness Identification)과 일관된 배선 경로 역시 제조, 검사, 유지보수 및 비상 대응(Emergency Response)의 안전성을 향상시킨다.

고장 전류 계산(Fault-Current Calculation)은 고전압 전력 분배 네트워크(HV Distribution Network)의 여러 위치에서 발생 가능한 고장을 평가해야 한다. 배터리 근처의 고장은 루프 임피던스(Loop Impedance)가 작기 때문에 매우 높은 전류를 발생시킬 수 있지만, 먼 위치의 고장은 더 낮은 전류와 더 긴 퓨즈 차단 시간(Fuse Clearing Time)을 발생시킬 수 있다. 따라서 최대 및 최소 신뢰 가능 고장 전류(Maximum and Minimum Credible Fault Current)가 모두 중요하다. 최대 전류는 차단 및 내전류 능력(Interrupting and Withstand Capability)을 검증하는 조건이며, 최소 고장 전류는 보호 장치가 신뢰성 있게 충분히 빠르게 동작할 수 있는지를 검증하는 조건이 된다.

보호 시스템은 다중 통전 상태(Multiple Energized States)도 고려해야 한다. 추진(Propulsion), 충전(Charging), 회생 운전(Regenerative Operation), 유지보수(Maintenance), 외부 전원 연결(External Power Connection) 상태에서는 서로 다른 부품에서 에너지가 공급되고 서로 다른 방향으로 흐를 수 있다. 인버터와 직류 링크 커패시터(DC-Link Capacitor)는 배터리 컨택터가 개방된 후에도 저장 에너지(Stored Energy)를 유지할 수 있다. 따라서 보호 분석에서는 모든 주요 에너지원을 식별하고 정상 종료(Normal Shutdown), 비상 격리(Emergency Isolation), 고장 조건에서 고전압 하니스의 각 구간이 어떻게 비통전 상태(De-Energized State)가 되는지를 판단해야 한다.

시스템 종료 후 잔류 전압(Residual Voltage)은 제어된 방전(Controlled Discharge)이 필요하다. 인버터, 컨버터, 충전기 및 기타 고전압 전자장치 내부의 커패시터는 주 전원이 차단된 이후에도 충전 상태를 유지할 수 있다. 방전 회로(Discharge Circuit)는 이러한 저장 전압을 시스템에서 정의한 요구 시간(System-Defined Time) 내에 보다 안전한 수준으로 낮출 수 있다. 따라서 하니스 안전은 메인 컨택터를 개방하는 것뿐만 아니라 커넥터 또는 정비 가능한 부품(Serviceable Component)을 비통전 상태로 판단하기 전에 위험한 저장 에너지(Hazardous Stored Energy)가 제거되었는지를 확인하는 것에도 의존한다.

보호 분할(Protection Segmentation)은 고장 전파(Fault Propagation)를 제한하고 시스템 가용성(System Availability)을 향상시킬 수 있다. 구동 시스템(Traction Drive), 보조 컨버터(Auxiliary Converter), 충전 장비(Charging Equipment), 기타 주요 부하에 전력을 공급하는 별도의 고전압 분기는 해당 도체 크기와 고장 노출(Fault Exposure)에 따라 전용 보호 장치를 사용할 수 있다. 적절한 분할을 적용하면 국부적인 고장을 격리하여 다른 분기가 불필요하게 과도한 에너지에 노출되는 것을 방지할 수 있다. 도체 용량이 감소하거나 전력 분배 토폴로지(Distribution Topology)가 크게 변경되는 모든 지점에서는 새로운 보호 협조 검토(Protection-Coordination Review)를 수행해야 한다.

고전압 하니스 보호 시스템의 검증(Validation)은 전기적 분석(Electrical Analysis), 물리적 검사(Physical Inspection), 제어된 시험(Controlled Testing)을 결합하여 수행한다. 엔지니어는 도체 온도 상승(Conductor Temperature Rise), 퓨즈 협조(Fuse Coordination), 고장 루프 임피던스(Fault-Loop Impedance), 절연 저항(Insulation Resistance), 유전체 건전성(Dielectric Integrity), 커넥터 온도(Connector Temperature), 인터록 동작(Interlock Operation), 컨택터 격리(Contactor Isolation), 프리차지 동작(Pre-Charge Behavior), 방전 성능(Discharge Performance)을 검증해야 한다. 전기적 보호에 대한 가정은 실제 하니스가 의도된 구성과 일치할 때만 유효하므로 배선 경로, 클램프, 보호 피복(Protective Covering), 이격 및 정비 접근성(Service Access) 역시 검사해야 한다.

효과적인 고전압 하니스 보호는 궁극적으로 저장된 전기 에너지(Stored Electrical Energy)와 위험한 고장(Unsafe Failure) 사이에 여러 개의 상호 협조된 보호 장벽(Coordinated Protection Barriers)을 형성한다. 퓨즈는 고장 에너지를 제한하고, 컨택터는 제어된 격리를 제공하며, 인터록은 물리적 건전성의 변화를 감지하고, 절연은 의도하지 않은 전류 경로를 방지하며, 감시 시스템(Monitoring System)은 성능 저하(Degradation)를 식별하고, 기계적 보호는 운전 중 이러한 보호 장벽을 유지한다. 이러한 기능을 단락 전류 계산(Short-Circuit Current Calculation), 최소 비보호 길이(Minimum Unprotected Length), 보호 협조(Protection Coordination), 검증과 통합함으로써 고에너지 로봇 전기 시스템(High-Energy Robotic Electrical System)을 위한 견고한 보호 아키텍처(Robust Protection Architecture)를 구축할 수 있다.
