**Volume 02. Wire Harness Engineering**

# Chapter 05. Derating

## 05.01. Bundle Derating Factor

![](images/image1.png){width="7.268055555555556in" height="7.268055555555556in"}

번들 디레이팅(Bundle Derating)은 여러 개의 통전 전선(Energized Wire)이 하나의 와이어 하니스(Wire Harness) 안에서 서로 가깝게 묶여 있을 때 허용 가능한 도체 전류(Allowable Conductor Current)를 감소시키는 것을 의미한다. 이 장의 구성에서는 와이어 게이지 선정(Wire Gauge Selection) 이후, 그리고 온도(Temperature), 전선관(Conduit), 환경별 보정(Environment-Specific Correction) 이전에 번들 디레이팅을 배치한다. 이는 개별 조건에서 선정된 전선이라도 실제 설치 구성이 결정된 이후에는 추가적인 전류 용량(Current Capacity) 감소가 필요할 수 있음을 의미한다.

단일 도체(Single Conductor)는 내부에서 발생한 열을 절연체(Insulation)와 주변 공기를 통해 외부로 방출한다. 그러나 여러 도체가 하나의 번들(Bundle)로 묶이면 각각의 도체가 열원(Heat Source)이 되는 동시에 인접 전선에서 발생하는 열의 영향을 받는다. 따라서 번들 내부 도체에서 외부 환경으로 이어지는 유효 열전달 경로(Effective Thermal Path)의 열저항이 증가하며, 동일한 전류가 흐르더라도 독립적으로 설치된 전선보다 도체 온도(Conductor Temperature)가 높아질 수 있다.

번들 디레이팅 계수(Bundle Derating Factor)는 이러한 열적 불이익(Thermal Penalty)을 기본 허용 전류에 적용하는 승수(Multiplier)로 표현한다. 개념적으로 독립된 도체의 허용 전류가 \\(I_{base}\\)라면 번들 조건이 반영된 전류 용량은 \\(I_{bundle}=I_{base}\\times K_{bundle}\\)로 표현할 수 있으며, 여기서 \\(K_{bundle}\\)은 일반적으로 1 이하이다. 계수가 작을수록 열적 상호작용(Thermal Interaction)이 심하다는 것을 의미하며, 그에 따라 허용 가능한 전류를 더 크게 감소시켜야 한다.

적절한 디레이팅 계수(Derating Factor)는 단순히 번들의 크기만으로 결정되지 않는다. 동시에 부하가 인가되는 도체의 수, 각 도체의 전류 수준(Current Level), 도체 크기, 절연 시스템(Insulation System), 전선 간격, 번들 직경(Bundle Diameter), 주변 온도(Ambient Temperature), 공기 흐름(Airflow), 듀티 사이클(Duty Cycle), 주변 보호재 등이 모두 열 축적에 영향을 준다. 따라서 동일한 수의 전선을 포함하는 두 하니스라도 전기적 부하나 실제 설치 조건이 다르면 열적 거동(Thermal Behavior)은 크게 달라질 수 있다.

동시 부하(Simultaneous Loading)는 특히 중요하다. 하니스에 포함된 모든 전선이 지속적으로 최대 설계 전류를 전달하는 것은 아니기 때문이다. 통신 회로(Communication Circuit), 센서(Sensor), 간헐적으로 작동하는 액추에이터(Intermittent Actuator), 제어 신호(Control Signal), 대기 전원 회로(Standby Power Branch)는 지속적으로 통전되는 추진 또는 전력 분배 도체보다 훨씬 적은 열을 발생시킬 수 있다. 따라서 열 설계에서는 번들 내부의 전체 전선 수와 동시에 작동하는 열적으로 유의미한 도체(Thermally Significant Conductor)의 수를 구분해야 한다.

번들 내부에서 도체가 위치하는 열적 위치(Thermal Position) 역시 중요하다. 번들 외부 표면에 가까운 도체는 주변 환경으로 열을 상대적으로 쉽게 방출할 수 있지만, 중심부에 위치한 도체는 다른 절연층과 발열 도체에 둘러싸여 있다. 따라서 번들의 중심 영역(Central Region)이 열적으로 가장 불리한 조건(Thermal Worst Case)이 될 수 있다. 모든 전선이 동일한 외부 주변 온도에 노출된다는 이유만으로 모든 도체가 동일한 온도를 가진다고 가정해서는 안 된다.

와이어 게이지(Wire Gauge)와 절연 구조(Insulation Construction) 역시 번들의 열적 성능에 영향을 준다. 대형 도체는 단위 길이당 저항이 낮더라도 높은 전류가 흐르면 상당한 총 열량을 발생시킬 수 있으며, 소형 도체는 높은 전기저항(Electrical Resistance)으로 인해 빠른 온도 상승이 발생할 수 있다. 절연체의 두께와 열적 특성(Thermal Characteristics)은 도체에서 번들 표면으로 전달되는 열에 영향을 주므로, 도체 구조는 단순한 패키징 요소가 아니라 디레이팅 평가(Derating Assessment)의 핵심 요소로 다루어야 한다.

보호 피복(Protective Covering)은 도체와 주변 공기 사이에 추가적인 열저항(Thermal Resistance)을 형성하여 번들 내부의 온도 상승을 더욱 심화시킬 수 있다. 테이프 래핑(Tape Wrapping), 브레이드 슬리브(Braided Sleeve), 코루게이트 튜브(Corrugated Tubing), 전선관(Conduit) 등의 하니스 보호재는 자연 대류(Convection)를 제한하고 번들 내부에 열을 가둘 수 있다. 따라서 번들 내부의 열적 상호작용과 외부 피복에 의한 열적 영향은 서로 연관되어 있지만 별개의 요소이며, 최종 열 설계에서는 두 영향을 함께 고려해야 한다.

주변 온도(Ambient Temperature) 역시 개념적으로 번들 디레이팅과 구분해야 한다. 번들 디레이팅은 여러 도체를 묶음으로써 발생하는 추가적인 열적 상호작용을 나타내는 반면, 고온 디레이팅(High-Temperature Derating)은 주변 환경 온도 상승으로 인해 감소하는 열적 여유(Thermal Margin)를 고려한다. 따라서 모터(Motor), 인버터(Inverter), 배터리(Battery), 제동 부품(Braking Component), 밀폐된 전자장치 구획 근처에 위치한 하니스에는 두 가지 보정이 모두 필요할 수 있으며, 하나의 계수를 다른 계수의 대체값으로 사용해서는 안 된다.

실제 설계 과정(Practical Design Process)은 도체 특성과 적용 가능한 온도 한계(Temperature Limit)를 기준으로 허용 전류를 설정하는 것에서 시작한다. 이후 현실적인 동시 부하 조건을 파악하고 실제 번들 구성을 정의한다. 번들 보정(Bundle Correction)은 관련 온도 및 설치 보정(Installation Correction)과 함께 적용하며, 이후 최종 도체 온도 여유, 전압 강하(Voltage Drop), 보호 협조(Protection Coordination), 기계적 패키징(Mechanical Packaging)을 서로 독립적인 계산이 아닌 통합 설계(Integrated Design)의 관점에서 검토해야 한다.

여러 디레이팅 계수(Derating Factor)를 단순히 곱하는 방식은 보수적인 공학적 방법(Conservative Engineering Method)으로 활용할 수 있지만, 각 계수가 서로 호환되는 가정(Compatible Assumption)을 기반으로 하는지 확인해야 한다. 지나치게 보수적인 계수 조합은 불필요하게 큰 도체, 무거운 하니스, 대형 커넥터(Connector), 증가된 굽힘 반경(Bend Radius), 높은 비용을 초래할 수 있다. 반대로 지나치게 낙관적인 계수는 과도한 온도 상승과 절연체 열화(Insulation Aging)를 유발할 수 있으므로 각 계수의 수치뿐 아니라 그 계수에 적용된 가정을 함께 검토해야 한다.

과도 부하(Transient Load)는 열적 응답(Thermal Response)이 시간에 따라 달라지므로 추가적인 검토가 필요하다. 짧은 시간 동안 가속 전류(Acceleration Current)를 전달하는 모터 도체는 동일한 전류를 지속적으로 전달하는 도체와 상당히 다른 온도 상승 특성을 보일 수 있다. 따라서 번들 디레이팅은 듀티 사이클(Duty Cycle)과 도체의 열 시정수(Thermal Time Constant)를 함께 고려하여 해석해야 한다. 부하 지속 시간이 충분히 짧다면 최대 전기 전류(Peak Electrical Current)가 반드시 연속 전류(Continuous Current)와 동일한 열적 영향을 의미하지는 않는다.

측정(Measurement)은 해석 및 계산 과정에서 설정한 가정을 검증하는 중요한 수단이다. 실제 양산 조건을 반영한 와이어 종류, 번들 치수, 보호 피복, 클램프(Clamp), 라우팅(Routing), 전기적 부하를 이용하여 대표적인 하니스 샘플을 제작할 수 있다. 온도 센서(Temperature Sensor)는 예상되는 핫스폿(Hot Spot), 특히 번들 중심부의 도체와 열적으로 제한된 구간에 배치해야 한다. 안정화된 최악 조건(Worst-Case Operating Condition)에서 시험함으로써 계산된 디레이팅이 충분한 열적 여유를 제공하는지 확인할 수 있다.

로보틱스(Robotics)와 자율이동로봇(AMR, Autonomous Mobile Robot)에서는 고전류 구동 배선(High-Current Drive Wiring), 배터리 전력 분배(Battery Power Distribution), 컴퓨팅 전원(Compute Power), 센서 배선(Sensor Wiring), 통신선(Communication Line), 보조 회로(Auxiliary Circuit)가 제한된 라우팅 공간을 공유할 수 있기 때문에 번들 디레이팅이 특히 중요하다. 소형화된 섀시 패키징(Compact Chassis Packaging)은 공기 흐름을 제한하고 긴 하니스 구간을 좁은 통로로 통과하도록 만들 수 있으므로 실제 AMR 환경을 반영한 열적 검토가 필요하다.

번들 설계(Bundle Design)는 궁극적으로 단순한 전선 개수 규칙이 아니라 시스템 수준의 열 문제(System-Level Thermal Problem)로 다루어야 한다. 도체 선정(Conductor Selection)은 전기적 손실을 결정하고, 라우팅은 열전달 조건을 결정하며, 보호 장치(Protection Device)는 비정상 상태에서의 에너지를 제한하고, 패키징은 발생한 열이 주변 환경으로 얼마나 효과적으로 방출되는지를 결정한다. 따라서 견고한 디레이팅 설계는 이러한 요소를 통합하여 정상 운전과 신뢰 가능한 최악 부하 조건에서 하니스가 허용 온도 범위 이내를 유지하도록 해야 한다.

최종적인 공학적 목표는 단순히 가능한 가장 낮은 디레이팅 계수를 적용하는 것이 아니라 실제 설치 조건에 대해 근거가 명확한 전류 용량(Defensible Current Capacity)을 확립하는 것이다. 열적 여유가 충분하지 않다면 도체 단면적(Conductor Cross-Sectional Area)을 증가시키거나, 고전류 회로를 분리하고, 번들 밀도(Bundle Density)를 낮추며, 환기(Ventilation)를 개선하거나 보호 피복을 변경할 수 있다. 또한 하니스를 열원으로부터 멀리 배치하거나 시스템 동작으로 입증된 경우 동시 부하 가정을 수정할 수도 있다. 따라서 번들 디레이팅은 전기적 사이징(Electrical Sizing)과 실제 하니스 아키텍처(Harness Architecture)를 연결하는 반복적인 설계 메커니즘(Iterative Design Mechanism)으로 이해해야 한다.

## 05.02. High Temperature Derating

![](images/image2.png){width="7.268055555555556in" height="7.268055555555556in"}

고온 디레이팅(High-Temperature Derating)은 도체의 일반적인 허용 전류(Ampacity)를 설정할 때 사용한 기준 조건(Reference Condition)보다 높은 주변 온도(Ambient Temperature)에서 전선이 작동할 경우 허용 가능한 전류를 감소시키는 것을 의미한다. 주변 온도가 상승하면 전선 내부에서 발생한 열을 외부로 방출하는 데 이용할 수 있는 온도 차이가 감소한다. 따라서 실온에서 특정 전류를 안전하게 전달하는 전선이라도 고온 영역에 설치되면 허용 가능한 도체 또는 절연체 온도를 초과할 수 있다.

전선의 열적 한계(Thermal Limitation)는 기본적으로 도체(Conductor)와 절연 시스템(Insulation System)이 요구되는 전기적 및 기계적 성능을 유지하면서 견딜 수 있는 최대 온도에 의해 결정된다. 작동 중 도체 온도(Operating Conductor Temperature)는 개념적으로 주변 온도와 전류에 의해 발생하는 온도 상승의 합으로 볼 수 있다. 주변 온도가 허용 가능한 재료 온도에 가까워질수록 도체 저항에 의한 줄 발열(Joule Heating)에 사용할 수 있는 열적 여유(Thermal Margin)는 점차 감소한다.

단순화된 열적 관계(Thermal Relationship)는 \\(T_{conductor}=T_{ambient}+\\Delta T_{current}\\)로 표현할 수 있다. 여기서 \\(T_{ambient}\\)는 해당 위치의 주변 환경 온도를 나타내며, \\(\\Delta T_{current}\\)는 실제 설치 조건에서 전기적 부하에 의해 발생하는 온도 상승을 의미한다. 설계 요구사항은 예상되는 모든 운전 조건에서 최종 도체 온도가 충분한 공학적 여유(Engineering Margin)를 확보하면서 적용 가능한 최대 온도 이하로 유지되도록 하는 것이다.

고온 디레이팅은 기준 허용 전류에 적용되는 온도 보정 계수(Temperature Correction Factor)로 표현할 수 있다. \\(I_{base}\\)가 지정된 기준 조건에서의 허용 전류라면 보정된 전류 용량은 개념적으로 \\(I_{temp}=I_{base}\\times K_{temp}\\)로 나타낼 수 있다. 주변 온도가 상승할수록 \\(K_{temp}\\)는 감소하며, 이는 도체가 허용 온도를 초과하지 않으면서 내부에서 발생한 열을 방출할 수 있는 능력이 점차 감소한다는 것을 의미한다.

적절한 보정 계수(Correction Factor)는 주변 온도만으로 선정할 수 없다. 전선 절연 등급(Wire Insulation Class), 도체 재료(Conductor Material), 허용 연속 온도(Allowable Continuous Temperature), 전류 듀티 사이클(Current Duty Cycle), 공기 흐름(Airflow), 라우팅(Routing), 번들 구성(Bundle Configuration), 인클로저 조건(Enclosure Condition), 주변 열원(Nearby Heat Source) 등이 실제 열적 상태에 영향을 준다. 따라서 온도 보정을 적용하기 전에 최초 허용 전류값이 어떤 기준 조건을 바탕으로 설정되었는지를 이해해야 한다.

전기저항(Electrical Resistance) 역시 도체 온도가 상승함에 따라 증가한다. 구리(Copper)와 같은 금속 도체에서는 온도가 높아지면 저항이 증가하고, 동일한 전류에서도 \\(I\^2R\\) 손실이 증가한다. 이는 중요한 열적 피드백 메커니즘(Thermal Feedback Mechanism)을 형성한다. 주변 온도가 상승하면 도체 온도가 높아지고, 도체 온도 상승은 저항을 증가시키며, 증가한 저항은 다시 추가적인 열을 발생시킨다. 따라서 높은 정확도가 필요한 경우 열 해석(Thermal Analysis)에서 온도에 따른 저항 변화를 고려해야 한다.

절연체 온도 정격(Insulation Temperature Rating)은 중요한 상한 경계(Upper Boundary)를 설정하지만 이를 권장 정상 작동 온도로 해석해서는 안 된다. 최대 재료 정격에 가까운 온도에서 지속적으로 작동하면 절연체 노화(Insulation Aging)가 가속되고 기계적 유연성(Mechanical Flexibility)이 저하되며 장기 신뢰성(Long-Term Reliability)이 감소할 수 있다. 실제 하니스 설계에서는 제조 편차, 국부 핫스폿(Local Hot Spot), 과도 조건(Transient Condition), 노화, 오염 및 불확실성을 고려하여 절대 재료 한계보다 충분히 낮은 온도 여유를 확보하는 것이 일반적이다.

전체적인 실내 또는 차량 온도보다 국부 온도(Local Temperature)가 더 중요하다. 동일한 전류를 전달하는 하나의 하니스도 여러 열 영역(Thermal Zone)을 통과할 수 있으며, 모터(Motor), 인버터(Inverter), DC-DC 컨버터(DC-DC Converter), 제동 부품(Braking Component), 배터리(Battery), 배기 계통과 유사한 열원 또는 밀폐된 전자장치 구획 주변의 짧은 구간만 최악의 열 조건을 경험할 수 있다. 따라서 전류 용량은 평균 환경 온도가 아니라 라우팅 경로에서 예상할 수 있는 가장 높은 온도 구간을 기준으로 평가해야 한다.

열전달(Heat Transfer)은 공기 흐름과 설치 형상(Installation Geometry)의 영향도 크게 받는다. 움직이는 공기에 노출된 전선은 밀폐된 구획이나 좁게 제한된 채널에 설치된 동일한 전선보다 열을 효과적으로 방출할 수 있다. 따뜻한 구조물 표면에 접하거나 가까이 라우팅된 하니스는 전도(Conduction)와 복사(Radiation)를 통해 추가적인 열을 받을 수도 있다. 따라서 고온 디레이팅은 주변 공기 온도만을 유일한 외부 열 입력으로 간주하지 않고 실제 설치 환경을 반영해야 한다.

고온 디레이팅(High-Temperature Derating)과 번들 디레이팅(Bundle Derating)은 서로 다른 물리적 영향을 다루지만 동시에 발생할 수 있다. 온도 디레이팅(Temperature Derating)은 외부 환경에 의해 열적 여유가 감소하는 현상을 고려하는 반면, 번들 디레이팅은 서로 인접한 통전 도체(Energized Conductor) 사이의 열적 상호작용(Thermal Interaction)을 고려한다. 고온 인클로저 내부에 조밀하게 배치된 하니스에는 두 가지 보정이 모두 필요할 수 있으며, 열전달을 제한하는 슬리브(Sleeve), 전선관(Conduit), 보호 피복(Covering)의 영향도 추가로 고려해야 한다.

여러 보정 계수가 필요한 경우 개념적인 공학식은 \\(I_{allow}=I_{base}\\times K_{temp}\\times K_{bundle}\\times K_{install}\\)로 표현할 수 있으며, 각 계수는 온도, 번들링(Bundling), 설치 효과(Installation Effect)를 나타낸다. 이러한 표현은 설계 체계를 구성하는 데 유용하지만 각 계수의 기준 가정을 확인하지 않고 기계적으로 곱해서는 안 된다. 일부 경험적 전류 정격(Empirical Current Rating)에는 특정 설치 조건이 이미 반영되어 있을 수 있으므로 의도하지 않은 중복 디레이팅(Double Derating)이 발생할 수 있다.

연속 부하(Continuous Load)와 과도 부하(Transient Load) 역시 구분해야 한다. 지속적으로 통전되는 전력 도체(Power Conductor)는 시간이 지나면서 주변 환경과 열적 평형(Thermal Equilibrium)에 가까워질 수 있으므로 높은 주변 온도가 지배적인 제한 조건이 될 수 있다. 반면 짧은 시간 동안 작동하는 액추에이터(Actuator)나 모터 전류는 도체가 정상상태 온도(Steady-State Temperature)에 도달하기 전에 종료될 수 있다. 따라서 열적 평가에서는 열 시정수(Thermal Time Constant)와 실제 듀티 사이클을 고려하여 피크 전류(Peak Current), RMS 등가 부하(RMS-Equivalent Loading), 연속 전류 중 어떤 값을 기준으로 사용할 것인지 결정해야 한다.

열 사이클링(Thermal Cycling)은 로봇 하니스(Robotic Harness)에서 추가적으로 고려해야 할 요소이다. 대기 상태(Standby), 가속(Acceleration), 높은 컴퓨팅 부하(High Compute Load), 충전(Charging), 정상 주행 사이의 반복적인 상태 변화는 도체, 단자(Terminal), 커넥터(Connector), 주변 재료를 반복적으로 가열하고 냉각할 수 있다. 최대 온도가 명목상의 한계 이내에 있더라도 반복적인 열 사이클은 기계적 접속부(Mechanical Interface)와 장기 내구성(Long-Term Durability)에 영향을 줄 수 있으므로 온도 평가는 최대 온도뿐 아니라 대표적인 운전 프로파일(Operating Profile)도 함께 고려해야 한다.

검증(Validation)은 실제 열 환경을 가능한 한 충실하게 재현해야 한다. 양산 조건을 반영한 전선, 번들 배열, 보호 피복, 커넥터, 클램프(Clamp), 라우팅 경로 및 전기적 부하를 사용하여 예상되는 최악의 주변 온도 조건에서 시스템을 작동시키고 예상 핫스폿의 온도를 측정할 수 있다. 연속 회로는 열적 평형에 충분히 가까워질 수 있도록 적절한 시간을 확보해야 하며, 과도 회로는 실제 운전 조건을 반영한 반복 듀티 사이클을 이용하여 평가해야 한다.

온도 측정 위치(Temperature Measurement Location)는 신중하게 선정해야 한다. 가장 높은 온도의 도체가 반드시 접근하기 쉬운 하니스 외부 표면과 일치하는 것은 아니기 때문이다. 특히 고밀도 번들(Dense Bundle)이나 밀폐된 라우팅에서는 외부 보호 피복에만 센서를 설치하면 내부 도체 온도를 과소평가할 수 있다. 번들 중심부의 도체, 고전류 분기(High-Current Branch), 커넥터 전환부(Connector Transition), 공기 흐름이 제한된 영역, 주변 열원 인근을 측정하면 선정한 디레이팅 전략이 충분한 열적 여유를 유지하는지 보다 확실하게 검증할 수 있다.

자율이동로봇(AMR, Autonomous Mobile Robot)과 모바일 로봇(Mobile Robot)에서는 전체적인 운용 환경이 비교적 온화해 보이더라도 고온 디레이팅이 중요하다. 구동 모터(Drive Motor), 모터 컨트롤러(Motor Controller), 배터리 팩(Battery Pack), DC-DC 컨버터, GPU 기반 컴퓨팅 모듈(GPU-Based Compute Module), 충전 하드웨어(Charging Hardware), 소형 전력 분배 장치(Compact Power-Distribution Assembly)는 섀시 내부에 국부적인 고온 영역을 형성할 수 있다. 제한된 환기와 높은 패키징 밀도로 인해 내부 하니스 온도는 외부 주변 온도보다 상당히 높아질 수 있다.

열적 문제를 완화하기 위해 반드시 도체 크기를 증가시켜야 하는 것은 아니다. 하니스를 열원으로부터 멀리 재배치하고, 고온 표면과의 이격 거리(Separation Distance)를 증가시키며, 공기 흐름을 개선하거나 번들 밀도(Bundle Density)를 낮출 수 있다. 또한 더 높은 온도 등급의 절연체를 선택하고, 보호 피복을 변경하며, 손실이 큰 배선 경로를 단축하거나 지속적으로 부하가 인가되는 전력 회로를 다른 도체와 분리할 수 있다. 최적의 해결책은 열 성능과 전압 강하(Voltage Drop), 질량(Mass), 유연성(Flexibility), 패키징, 비용 및 정비성(Serviceability)을 함께 고려하여 결정해야 한다.

고온 디레이팅은 궁극적으로 설계 마지막 단계에서 독립적인 보정값을 추가하는 방식이 아니라 통합 와이어 사이징 프로세스(Integrated Wire-Sizing Process)의 일부로 다루어야 한다. 전류 용량(Current Capacity), 전압 강하, 번들 발열(Bundle Heating), 설치 제약(Installation Restriction), 보호 협조(Protection Coordination), 절연 성능(Insulation Capability), 예상 수명(Expected Lifetime)은 서로 영향을 주고받는다. 견고한 설계는 신뢰 가능한 최악의 열 조건을 정의하고 적절한 보정 가정을 적용한 후, 의도된 전체 운용 수명 동안 충분한 온도 여유가 유지되는지를 검증해야 한다.

## 05.03. Conduit and Sleeve Effect

![](images/image3.png){width="7.268055555555556in" height="7.268055555555556in"}

전선관(Conduit)과 보호 슬리브(Protective Sleeve)는 기계적 보호(Mechanical Protection), 마모 저항(Abrasion Resistance), 환경 밀봉(Environmental Sealing), 배선 정리 및 라우팅 제어(Routing Control)를 위해 와이어 하니스(Wire Harness) 시스템에서 널리 사용된다. 그러나 이러한 보호층은 도체 주변의 열 환경(Thermal Environment)도 변화시킨다. 전선을 주변 공기로부터 부분적으로 차단함으로써 열 방출(Heat Dissipation)을 감소시킬 수 있으며, 이에 따라 연속 운전 조건에서 도체가 안전하게 전달할 수 있는 허용 전류가 감소할 수 있다.

피복되지 않은 전선(Uncovered Wire)은 내부에서 발생한 열을 절연체(Insulation)를 통해 주변 환경으로 전달하며, 이 과정에는 전도(Conduction), 대류(Convection), 복사(Radiation)가 작용한다. 동일한 전선이 코루게이트 전선관(Corrugated Conduit), 브레이드 슬리브(Braided Sleeving), 튜빙(Tubing) 또는 다른 보호 피복 내부에 배치되면 열전달 경로에 추가적인 재료가 포함된다. 그 결과 전류와 외부 주변 온도가 동일하더라도 열저항(Thermal Resistance)이 증가하여 도체 온도가 상승할 수 있다.

이러한 영향은 개념적으로 설치 보정 계수(Installation Correction Factor)를 통해 표현할 수 있다. \\(I_{base}\\)가 정의된 기준 설치 조건에서의 허용 전류를 나타낸다면, 밀폐 효과(Enclosure Effect)를 고려한 전류 용량은 \\(I_{install}=I_{base}\\times K_{install}\\)로 표현할 수 있다. 전선관이나 슬리브가 기준 조건보다 냉각을 제한하는 경우 \\(K_{install}\\)은 일반적으로 1 이하이며, 적절한 값은 실제 구조와 설치 조건에 따라 결정된다.

모든 보호 피복(Protective Covering)이 동일한 열적 불이익(Thermal Penalty)을 발생시키는 것은 아니다. 개방형 브레이드 슬리브(Open Braided Sleeve)는 단단하게 감긴 테이프 시스템(Tape System)이나 폐쇄형 폴리머 전선관(Closed Polymer Conduit)보다 더 많은 공기 교환을 허용할 수 있다. 코루게이트 튜빙(Corrugated Tubing)은 도체 주변에 밀폐된 공기층을 형성할 수 있으며, 두꺼운 벽의 튜빙은 추가적인 열저항을 발생시킬 수 있다. 따라서 열전도율(Thermal Conductivity), 두께, 표면 특성 및 피복률이 서로 다른 재료는 각기 다른 도체 온도 특성을 나타낸다.

전선관 충전율(Conduit Fill Ratio)도 중요한 변수이다. 소수의 도체만 서로 떨어져 배치된 대형 전선관은 어느 정도 내부 공기 흐름을 유지하고 열전달을 위한 더 큰 유효 표면적을 제공할 수 있다. 반면 높은 충전율의 전선관에서는 도체 사이의 거리가 가까워지고 사용 가능한 공기 공간이 감소하며 인접 전선 사이의 열적 상호작용(Thermal Interaction)이 증가한다. 따라서 전선관 크기는 단순히 기계적 수용 여부만으로 결정해서는 안 되며 고전류 회로가 포함되는 경우 열적 거동도 고려해야 한다.

인클로저(Enclosure) 내부에서 동시에 통전되는 도체의 수는 온도 상승에 큰 영향을 미친다. 신호선(Signal Wire)이나 부하가 작은 센서 회로는 상대적으로 적은 열을 발생시킬 수 있지만, 배터리 전력 분배(Battery Distribution), 모터 전원(Motor Supply), 액추에이터(Actuator), 히터(Heater), 컴퓨팅 전원(Compute Power) 도체에서는 상당한 \\(I\^2R\\) 손실이 발생할 수 있다. 따라서 공학적 평가에서는 물리적인 전체 도체 수와 동시에 작동하는 열적으로 중요한 도체(Thermally Significant Conductor)의 수 및 부하 수준을 구분해야 한다.

번들 디레이팅(Bundle Derating)과 전선관 또는 슬리브 효과는 밀접하게 연관되어 있지만 설치 조건의 서로 다른 측면을 나타낸다. 번들 디레이팅은 인접한 통전 도체 사이의 열적 상호작용을 다루는 반면, 전선관 및 슬리브 보정은 주변 보호재가 추가함으로써 발생하는 열전달 제한을 다룬다. 번들로 묶인 도체가 열 방출을 제한하는 전선관 내부에 설치되면 두 가지 메커니즘이 동시에 존재할 수 있으므로 동일한 열적 영향을 의도하지 않게 중복 계산하지 않도록 평가해야 한다.

주변 온도(Ambient Temperature)는 또 다른 상호작용 조건이다. 시원하고 환기가 잘되는 영역에 설치된 전선관은 비교적 작은 열 보정만으로 만족스러운 성능을 유지할 수 있지만, 동일한 전선관 어셈블리(Assembly)가 고온 인클로저 내부에 배치되면 도체 온도가 상당히 높아질 수 있다. 따라서 최종 설계에서는 온도 디레이팅(Temperature Derating), 번들 디레이팅(Bundle Derating), 설치 디레이팅(Installation Derating)을 함께 고려해야 할 수 있다.

구조물 표면을 따라 이루어지는 라우팅(Routing)은 관련 재료와 표면 온도에 따라 열전달을 개선하거나 악화시킬 수 있다. 차가운 금속 섀시(Metallic Chassis)와 접촉하면 추가적인 전도성 열전달 경로가 형성될 수 있지만, 따뜻한 모터 하우징(Motor Housing), 배터리 인클로저(Battery Enclosure), 전력전자 구조물(Power-Electronics Structure)에 인접하면 외부에서 추가적인 열이 유입될 수 있다. 전선관 자체도 접촉 면적을 변화시키므로 보호재만 독립적으로 평가하지 않고 전체 라우팅 형상을 고려해야 한다.

보호 피복은 일반적으로 기계적인 이유를 우선하여 선정된다. 코루게이트 전선관은 마모와 충격으로부터 보호할 수 있고, 브레이드 슬리브는 유연성과 내마모성(Wear Resistance)을 향상시킬 수 있으며, 특수 튜빙(Specialized Tubing)은 환경적 또는 화학적 보호를 제공할 수 있다. 따라서 열 성능은 다목적 설계(Multi-Objective Design)의 여러 요구사항 중 하나이다. 냉각 성능만을 개선하기 위해 보호재를 제거하면 하니스의 다른 부분에서 허용할 수 없는 기계적, 환경적 또는 수명 관련 위험이 발생할 수 있다.

인클로저 효과를 평가할 때는 연속 부하(Continuous Load)와 과도 부하(Transient Load)를 구분해야 한다. 지속적으로 부하가 인가되는 도체는 열적 평형(Thermal Equilibrium)에 접근할 충분한 시간을 가지므로 제한된 열 방출이 상당한 온도 상승을 유발할 수 있다. 단시간 전류는 도체와 주변 전선관이 정상상태 온도(Steady-State Temperature)에 도달하기 전에 종료될 수 있다. 그러나 냉각 간격이 충분하지 않으면 반복되는 과도 부하에 의해 열이 축적될 수 있다.

커넥터(Connector)와 분기 영역(Branch Region)은 전선관의 형상이 이러한 위치에서 자주 변화하므로 특별한 주의가 필요하다. 여러 전선이 커넥터에 들어가기 전에 집중되거나, 하나의 슬리브가 다른 보호층과 겹치거나, 테이프가 원래 환기가 가능했던 번들을 밀폐할 수 있다. 이러한 전환부(Transition)는 주 하니스 구간보다 높은 열저항을 갖는 국부 영역을 형성할 수 있다. 따라서 전체 라우팅 경로에서 피복 변화, 번들 직경, 도체 집중도 및 공기 흐름의 변화를 고려해야 한다.

실제 공학적 평가(Engineering Evaluation)는 도체 크기, 회로 전류, 듀티 사이클(Duty Cycle), 절연체 온도 한계(Insulation Temperature Limit), 예상 동시 부하(Simultaneous Loading)를 정의하는 것에서 시작한다. 이후 계획된 전선관, 슬리브, 테이프 또는 튜빙 구성과 함께 충전율, 라우팅 형상, 주변 온도 및 공기 흐름 조건을 적용한다. 최종 설치 상태에서는 도체 온도, 전압 강하(Voltage Drop), 보호 협조(Protection Coordination), 기계적 패키징(Mechanical Packaging), 유연성 및 예상 수명(Expected Lifetime)을 검토해야 한다.

여러 보정이 필요한 경우 허용 전류는 개념적으로 \\(I_{allow}=I_{base}\\times K_{bundle}\\times K_{temp}\\times K_{install}\\)로 정리할 수 있다. 이 식은 공학적 명확성을 위해 번들링(Bundling), 주변 온도 및 설치 효과를 분리하여 나타낸다. 그러나 보정 계수들은 서로 호환되는 기준 조건을 바탕으로 해야 한다. 허용 전류 사양(Ampacity Specification)이나 시험 결과에 이미 밀폐 또는 번들 조건이 반영되어 있다면 추가적인 일반 보정 계수를 적용함으로써 불필요한 중복 디레이팅(Double Derating)이 발생할 수 있다.

단순한 보정 계수만으로 세부적인 열적 거동을 예측하기 어려울 수 있으므로 높은 수준으로 밀폐된 하니스에서는 실험적 검증(Experimental Validation)이 특히 중요하다. 실제 양산 조건을 반영한 도체, 전선관, 슬리브, 테이프, 클램프(Clamp), 커넥터 및 라우팅 형상을 이용하여 대표적인 하니스를 제작할 수 있다. 최악의 주변 온도 조건에서 실제적인 동시 부하를 적용하고 정상상태 또는 대표적인 과도 운전 사이클 동안 온도를 측정할 수 있다.

온도 측정(Temperature Measurement)은 열이 가장 많이 축적될 가능성이 있는 위치를 포함해야 한다. 높은 충전율의 전선관 중심부에 있는 도체, 고전류 분기, 슬리브 중첩 영역, 테이프로 감싼 전환부, 커넥터 백셸(Connector Backshell) 영역 및 외부 열원 인근 구간이 주요 측정 대상이 될 수 있다. 전선관의 표면 온도만으로는 내부에서 가장 뜨거운 도체 온도를 정확하게 나타내지 못할 수 있으므로 실제 어셈블리의 열적 한계를 확인할 수 있는 검증 방법을 사용해야 한다.

자율이동로봇(AMR, Autonomous Mobile Robot)과 모바일 로봇(Mobile Robot)에서는 하니스가 모터, 모터 컨트롤러(Motor Controller), 배터리, DC-DC 컨버터(DC-DC Converter), 컴퓨터, 센서 및 통신 장비가 포함된 제한된 섀시 공간을 통과하는 경우가 많기 때문에 전선관과 슬리브의 영향이 중요해질 수 있다. 진동(Vibration), 반복 운동(Repetitive Movement), 날카로운 구조물, 정비 작업 및 오염으로부터 노출된 배선을 보호해야 하지만 이러한 보호 구조가 이미 밀집된 패키징 내부에서 냉각을 제한할 수도 있다.

기계적 보호를 포기하지 않고도 열 문제를 완화할 수 있다. 설계자는 전선관 직경을 증가시키고, 충전율을 낮추며, 고전류 도체를 분리하거나 열적으로 더 유리한 보호 피복을 사용할 수 있다. 또한 환기를 개선하고, 밀폐되는 구간을 단축하거나, 하니스를 열원에서 멀리 재배치할 수 있다. 도체 단면적(Conductor Cross-Sectional Area)을 증가시키면 저항이 감소하여 \\(I\^2R\\) 발열을 줄일 수 있지만, 하니스 직경, 질량, 굽힘 반경(Bend Radius), 커넥터 크기 및 비용 증가도 함께 고려해야 한다.

전선관 및 슬리브 효과(Conduit and Sleeve Effect)는 궁극적으로 전선 자체의 고정된 특성이 아니라 설치 조건에 따라 결정되는 열적 특성(Installation-Dependent Thermal Characteristic)으로 다루어야 한다. 도체는 패키징 방식과 관계없이 하나의 보편적으로 유효한 전류 용량을 갖는 것이 아니다. 안전한 하니스 설계를 위해서는 전기적 부하, 도체 구조, 번들 구성, 보호 피복, 주변 환경, 라우팅 및 냉각 조건을 통합적으로 평가하여 의도된 전체 운용 수명 동안 충분한 온도 여유(Thermal Margin)가 유지되도록 해야 한다.

## 05.04. Derating Table by Environment

![](images/image4.png){width="7.268055555555556in" height="7.268055555555556in"}

환경별 디레이팅 표(Environmental Derating Table)는 전선의 기준 허용 전류(Reference Ampacity)를 실제 설치 환경에 적합한 허용 전류(Allowable Current)로 변환하기 위한 체계적인 방법을 제공한다. 디레이팅(Derating) 장에서 이 주제는 앞서 설명한 번들(Bundle), 고온(High Temperature), 전선관 또는 슬리브(Conduit or Sleeve)의 영향을 통합하여 실제 설계에 적용하기 위한 단계이다. 목적은 하나의 보편적인 계수를 지정하는 것이 아니라 서로 다른 하니스 환경에 대해 반복 가능한 공학적 판단 체계를 구축하는 것이다.

디레이팅 표(Derating Table)는 일반적으로 명확하게 정의된 기준 조건(Reference Condition)에서 시작한다. 기본 전류 정격(Base Current Rating)은 특정 주변 온도(Ambient Temperature), 독립 또는 자유 통풍 상태의 배선, 특정 절연 등급(Insulation Class), 정의된 도체 구조(Conductor Construction)를 가정할 수 있다. 환경 계수(Environmental Factor)는 이러한 기준 조건에 대해서만 의미를 가지므로 기준 가정을 알 수 없는 상태에서 보정값을 적용하면 안전하지 않은 낙관적 판단이나 불필요하게 보수적인 설계가 발생할 수 있다.

일반적인 관계는 개념적으로 \\(I_{allow}=I_{base}\\times K_{environment}\\)로 표현할 수 있다. 여기서 \\(I_{base}\\)는 기준 허용 전류이며, \\(K_{environment}\\)는 실제 설치 환경에 필요한 보정값을 의미한다. 보다 상세한 평가에서는 환경 계수를 온도(Temperature), 번들링(Bundling), 설치(Installation)에 해당하는 \\(K_{temp}\\), \\(K_{bundle}\\), \\(K_{install}\\)과 같은 개별 항목으로 분해하여 적용할 수 있다.

자유 공기 설치(Free-Air Installation)는 도체 표면이 주변 공기와 직접 열을 교환할 수 있기 때문에 일반적으로 가장 유리한 열 환경(Thermal Environment) 중 하나를 제공한다. 적절한 간격과 환기(Ventilation)가 유지되면 내부에서 발생하는 \\(I\^2R\\) 열을 비교적 효과적으로 방출할 수 있다. 이러한 조건을 기준 사례로 사용할 수 있지만, 자유 공기 상태의 전류 용량을 밀집된 로봇 섀시 내부에 설치된 전선에 그대로 적용해서는 안 된다.

경량 번들 하니스(Lightly Bundled Harness)는 인접한 통전 도체가 서로 영향을 주기 때문에 추가적인 열적 상호작용(Thermal Interaction)을 발생시킨다. 보정 수준은 단순한 전체 전선 수가 아니라 동시에 부하가 인가되는 회로 수, 전류, 도체 크기, 간격 및 듀티 사이클(Duty Cycle)에 따라 달라진다. 다수의 신호선을 포함하는 하니스와 연속 고전류 전력 도체가 대부분을 차지하는 물리적으로 유사한 번들은 서로 다른 보정값이 필요할 수 있다.

고밀도 번들(Dense Bundle)은 내부 도체가 냉각 공기에 접근하기 어렵고 추가적인 열원에 둘러싸이기 때문에 더욱 제한적인 환경을 형성한다. 번들 중심부는 열적으로 가장 불리한 조건(Thermal Worst Case)이 될 수 있다. 따라서 환경별 디레이팅 표에서는 느슨하게 정리된 배선(Loosely Organized Wiring)과 조밀하게 패키징된 하니스(Dense Harness)를 구분해야 하며, 단순히 번들이라는 이유만으로 모든 설치에 동일한 계수를 적용해서는 안 된다.

전선관(Conduit), 튜빙(Tubing), 테이프 래핑(Tape Wrapping), 보호 슬리브(Protective Sleeve)는 또 다른 환경 범주를 형성한다. 이러한 재료는 마모, 오염 및 기계적 손상으로부터 중요한 보호 기능을 제공하지만 열저항(Thermal Resistance)을 증가시키고 대류(Convection)를 제한할 수 있다. 필요한 보정값은 피복 종류, 재료, 두께, 전선관 충전율(Conduit Fill Ratio), 공기 흐름 및 도체 부하에 따라 달라진다. 개방형 브레이드 보호재(Open Braided Protection)는 밀폐형 폴리머 튜빙이나 여러 겹의 테이프 구조와 다른 열적 특성을 나타낼 수 있다.

밀폐된 전기 구획(Enclosed Electrical Compartment)은 환기와 사용 가능한 방열 능력(Heat-Sink Capacity)이 모두 제한될 수 있기 때문에 더 큰 디레이팅을 요구할 수 있다. 전력전자 장치(Power Electronics), 컴퓨터, 컨버터(Converter), 배터리 및 모터 컨트롤러(Motor Controller)는 국부적인 공기와 구조물 온도를 외부 주변 온도보다 높일 수 있다. 따라서 로보틱스(Robotics)의 디레이팅 표에서는 실내 온도나 외부 공기 온도를 실제 설치 환경으로 가정하지 말고 하니스가 위치하는 지점의 온도를 사용해야 한다.

고온 영역(High-Temperature Zone)에서는 국부 주변 온도가 도체 또는 절연체 온도 한계에 가까워질수록 점진적으로 더 큰 보정이 필요하다. 남아 있는 열적 여유(Thermal Margin)는 전류에 의해 추가적으로 발생하는 온도 상승을 얼마나 허용할 수 있는지를 결정한다. 따라서 모터(Motor)나 인버터(Inverter) 근처를 통과하는 전선은 동일한 부하를 전달하더라도 더 낮은 온도의 센서 구획에 위치한 동일한 전선과 다른 허용 전류를 적용해야 할 수 있다.

공기 흐름이 적거나 밀폐된 환경(Low-Airflow and Sealed Environment)은 초기 주변 온도가 높지 않더라도 별도로 고려해야 한다. 도체와 주변 장비에서 발생한 열이 시간에 따라 축적되면 국부 온도가 초기 온도보다 상승할 수 있기 때문이다. 따라서 연속 운전 시스템(Continuous Operating System)의 환경 분류는 기동 직후 측정된 온도만을 기준으로 하지 않고 정상상태(Steady State) 또는 신뢰 가능한 최악 조건(Worst-Case Condition)의 온도를 반영해야 한다.

가동 하니스 구간(Moving Harness Section)에는 열적 디레이팅만으로 표현할 수 없는 추가적인 제약이 존재한다. 로봇 관절(Robot Joint), 조향 모듈(Steering Module), 서스펜션 인터페이스(Suspension Interface), 매니퓰레이터(Manipulator), 이동형 케이블 체인(Moving Cable Chain)에서는 열전달 특성을 변화시키는 유연 도체(Flexible Conductor)와 보호 피복이 필요할 수 있다. 따라서 적절한 환경별 표는 열 보정값을 제시하면서 굽힘 반경(Bend Radius), 반복 굴곡 수명(Repetitive Flex Life), 마모 및 기계적 변형(Mechanical Strain)이 별도의 설계 요구사항임을 함께 고려해야 한다.

옥외 설치(Outdoor Installation)에서는 태양 복사(Solar Radiation), 계절별 온도 변화, 수분 노출, 먼지, 바람 및 변화하는 운전 조건이 추가된다. 직사광선은 하니스 표면 온도를 측정된 공기 온도보다 높게 만들 수 있으며, 반대로 공기 흐름은 특정 조건에서 냉각 성능을 개선할 수 있다. 따라서 옥외 로봇(Outdoor Robot)의 환경 디레이팅은 하나의 명목상 외기 온도가 아니라 실제 설치 환경에서 발생 가능한 열적 범위(Thermal Envelope)를 기준으로 설정해야 한다.

실제 디레이팅 표에서는 프로젝트별 보정값을 지정하기 전에 환경을 정성적으로 유리(Favorable), 보통(Moderate), 제한적(Restrictive), 가혹(Severe) 조건으로 분류할 수 있다. 환기가 잘되고 부하가 작은 배선은 유리한 조건에 해당할 수 있으며, 고밀도 번들, 밀폐된 전선관 또는 높은 국부 온도는 제한적인 조건에 해당할 수 있다. 높은 주변 온도, 고밀도 번들링, 제한된 공기 흐름 및 보호 인클로저가 동시에 존재하는 경우에는 여러 열적 메커니즘이 결합된 가혹 조건으로 분류할 수 있다.

이러한 환경 분류(Environmental Classification)를 보편적인 수치 표준으로 해석해서는 안 된다. 실제 계수는 적용되는 전선 사양(Wire Specification), 제조사 데이터(Manufacturer Data), 검증된 공학 규칙(Validated Engineering Rule), 공인 표준(Recognized Standard) 또는 대표적인 열 시험(Thermal Testing)을 근거로 결정해야 한다. 일반적인 표는 어떤 보정 요소를 고려해야 하는지를 보여주는 의사결정 프레임워크(Decision Framework)로 사용하는 것이 가장 적절하며, 수치값은 특정 프로젝트의 도체 시스템과 기준 조건까지 추적 가능해야 한다.

여러 환경 메커니즘이 동시에 존재하는 경우 보정 계수는 개념적으로 \\(I_{allow}=I_{base}\\times K_{temp}\\times K_{bundle}\\times K_{install}\\)로 구성할 수 있다. 이러한 방식은 최종 전류 용량이 기준값과 달라지는 이유를 투명하게 문서화하는 데 도움이 된다. 그러나 계수를 곱하기 전에 원본 데이터가 각 메커니즘을 독립적으로 취급하고 있는지 확인해야 한다. 일부 공개된 허용 전류값에는 이미 번들 또는 인클로저 조건이 포함되어 있을 수 있기 때문이다.

환경별 디레이팅 표에서는 연속 운전(Continuous Operation)과 과도 운전(Transient Operation)도 구분해야 한다. 연속 전력 회로는 열적 평형에 접근할 수 있기 때문에 제한적인 환경의 영향을 크게 받는다. 간헐적으로 작동하는 액추에이터(Intermittent Actuator)는 열 질량(Thermal Mass)에 의해 온도 상승이 지연되므로 단시간 동안 더 높은 전류를 허용할 수 있다. 그러나 반복적인 과도 운전에서는 열이 축적될 수 있으므로 동적 로봇 부하에 표 기반 보정을 적용할 때도 듀티 사이클과 열 시정수(Thermal Time Constant)를 고려해야 한다.

검증(Validation)은 디레이팅 표에 포함된 가정을 실제 증거로 전환하는 과정이다. 대표적인 하니스 어셈블리(Harness Assembly)는 도체 크기, 동시 부하, 번들 밀도, 보호 피복, 라우팅, 공기 흐름 및 최악 주변 조건을 실제 설치 상태와 유사하게 재현해야 한다. 이후 번들 중심부 도체, 고전류 분기, 커넥터 전환부(Connector Transition), 밀폐 구간 및 예상 핫스폿(Hot Spot)의 온도를 측정하여 선정한 환경 분류와 보정 가정이 충분한 열적 여유를 제공하는지 확인할 수 있다.

자율이동로봇(AMR, Autonomous Mobile Robot)에서는 하나의 차량 내부에도 여러 종류의 디레이팅 환경이 동시에 존재할 수 있다. 배터리와 모터 배선은 고전류 영역에 위치할 수 있고, 컴퓨팅 모듈(Compute Module)은 따뜻하고 밀폐된 구획을 형성할 수 있으며, 센서 분기(Sensor Branch)는 낮은 전류로 작동할 수 있다. 또한 이동형 구동 모듈(Drive Module)에는 유연성과 보호 기능을 갖춘 하니스가 필요할 수 있다. 따라서 차량 전체에 하나의 디레이팅 계수를 적용하면 중요한 국부 차이가 사라져 배선의 과대 설계 또는 불충분한 열 보호가 발생할 수 있다.

효과적인 AMR 하니스 설계에서는 라우팅을 여러 열 영역(Thermal Zone)으로 구분하고 각 구간에 적절한 환경 분류를 지정할 수 있다. 동일한 전기 회로가 하나의 경로를 따라 자유 공기(Free Air), 번들(Bundle), 슬리브(Sleeve), 고온 영역을 차례로 통과할 수도 있다. 직렬 경로에서는 동일한 전류가 흐르기 때문에 가장 제한적인 신뢰 가능한 구간이 필요한 도체 크기를 결정할 수 있으며, 이러한 제한을 제거하려면 라우팅 또는 패키징을 다시 설계해야 할 수 있다.

최종 환경별 디레이팅 표(Environmental Derating Table)는 전기적 사이징(Electrical Sizing)과 실제 설치 환경을 연결하는 공학적 의사결정 도구(Engineering Decision Tool)로 기능해야 한다. 표에는 기준 허용 전류, 관련 환경, 적용 가능한 보정값, 최종 허용 전류 및 검증 근거(Validation Basis)가 포함되어야 한다. 올바르게 사용하면 이러한 표를 통해 도체 선정과 실제 하니스 조건 사이의 추적성(Traceability)을 확보할 수 있으며, 다음 단계의 AMR 전용 디레이팅 적용(AMR-Specific Derating Application)을 위한 기반을 제공할 수 있다.

## 05.05. AMR Derating Application

![](images/image5.png){width="7.268055555555556in" height="7.268055555555556in"}

AMR 디레이팅 적용(AMR Derating Application)은 일반적인 전선 허용 전류(Wire Ampacity) 규칙을 자율이동로봇(AMR, Autonomous Mobile Robot)의 실제 설치 조건에 적합한 전류 한계로 변환하는 과정이다. 고정형 전기 캐비닛과 달리 AMR은 배터리 전원, 구동 모터(Traction Motor), 모터 컨트롤러(Motor Controller), 컴퓨팅 하드웨어(Computing Hardware), 센서, 통신 장비, 충전 회로(Charging Circuit), 가동 하니스(Moving Harness)를 소형 플랫폼 내부에 통합한다. 각 영역은 서로 다른 열 환경(Thermal Environment)을 형성할 수 있으므로 도체 크기는 차량 전체에 하나의 전류 정격을 적용하는 대신 실제 라우팅 조건을 반영하여 선정해야 한다.

이 과정은 로봇의 전기적 부하 프로파일(Electrical Load Profile)을 정의하는 것에서 시작한다. 각 회로는 연속 전류(Continuous Current), 예상 운전 전류(Expected Operating Current), 과도 또는 피크 전류(Transient or Peak Current), 듀티 사이클(Duty Cycle), 다른 회로와의 동시 부하(Simultaneous Loading)를 기준으로 특성화해야 한다. 구동 모터는 가속 시 큰 전류를 요구할 수 있는 반면 컴퓨터는 비교적 안정적인 연속 부하를 형성한다. 센서와 통신 장치는 일반적으로 소비 전류가 작지만 많은 회로가 동일한 경로를 공유하면 번들 발열(Bundle Heating)에 영향을 줄 수 있다.

배터리 전력 분배 경로(Battery Distribution Path)는 일반적으로 AMR 하니스에서 열적으로 가장 중요한 구간 중 하나이다. 배터리 케이블은 공통 상위 도체를 통해 추진, 컴퓨팅, 제어, 센싱 및 보조 부하에 전력을 공급할 수 있다. 따라서 이러한 케이블은 하나의 서브시스템이 소비하는 명목 전류가 아니라 신뢰 가능한 최대 동시 부하(Maximum Credible Simultaneous Demand)를 기준으로 평가해야 한다. 퓨즈 협조(Fuse Coordination), 전압 강하(Voltage Drop), 커넥터 전류 용량(Connector Current Capability), 도체 온도가 선정된 전선 크기와 일관성을 유지해야 한다.

구동 및 조향 회로(Traction and Steering Circuit)는 로봇의 움직임에 따라 전기적 부하가 크게 변하기 때문에 특별한 검토가 필요하다. 가속, 경사로 등판(Slope Climbing), 화물 운반(Payload Transport), 회전, 장애물 탈출(Obstacle Recovery), 제동 과정에서는 정상 순항 상태보다 훨씬 높은 전류가 발생할 수 있다. 이러한 피크를 자동으로 연속 부하로 간주해서는 안 되지만 지속 시간과 반복 빈도에 따라 열이 축적될 수 있다. 따라서 하나의 최대 전류값보다 실제 임무 프로파일(Mission Profile)을 사용하는 것이 열 설계에 더욱 유용하다.

컴퓨팅 회로(Compute Circuit)는 이와 다른 부하 패턴을 갖는다. 엣지 컴퓨터(Edge Computer), GPU, 네트워크 스위치(Network Switch), 저장장치(Storage Device), 인지 프로세서(Perception Processor)는 상당한 전력을 지속적으로 소비하면서 전원 하니스가 통과하는 동일한 인클로저 내부에서 열을 발생시킬 수 있다. 따라서 하니스는 자체적인 \\(I\^2R\\) 발열뿐 아니라 전자장치가 형성하는 높은 국부 주변 온도의 영향도 받는다. 이 때문에 컴퓨팅 구획은 모터 회로보다 전류가 낮더라도 중요한 열 영역(Thermal Zone)이 될 수 있다.

따라서 AMR은 설치 조건에 따라 여러 열 영역으로 구분해야 한다. 대표적인 영역으로는 배터리 구획(Battery Compartment), 전력 분배 영역(Power-Distribution Area), 모터 컨트롤러 영역, 컴퓨팅 인클로저(Compute Enclosure), 센서 마스트(Sensor Mast), 섀시 라우팅 채널(Chassis Routing Channel), 구동 모듈(Drive Module), 충전 인터페이스(Charging Interface) 등이 있다. 각 영역은 국부 온도, 공기 흐름(Airflow), 번들 밀도(Bundle Density), 보호 피복(Protective Covering), 주변 열원, 움직임 및 예상 동시 전기 부하를 기준으로 분류할 수 있다.

하나의 회로가 여러 열 영역을 통과할 수도 있다. 예를 들어 모터 전원 케이블(Motor Supply Cable)은 비교적 낮은 온도의 배터리 구획에서 시작하여 조밀한 중앙 하니스 번들로 들어간 다음 보호 전선관(Protective Conduit)을 통과하고 높은 온도의 모터 컨트롤러 근처에서 종단될 수 있다. 직렬 경로 전체에는 동일한 전류가 흐르지만 열 환경은 경로에 따라 달라진다. 따라서 신뢰 가능한 가장 제한적인 구간(Most Restrictive Credible Section)이 전체 회로에 필요한 도체 크기를 결정할 수 있다.

허용 전류는 개념적으로 \\(I_{allow}=I_{base}\\times K_{temp}\\times K_{bundle}\\times K_{install}\\)로 정리할 수 있다. 온도 계수(Temperature Factor)는 국부 주변 조건을 나타내고, 번들 계수(Bundle Factor)는 동시에 통전되는 도체 사이의 열적 상호작용을 나타내며, 설치 계수(Installation Factor)는 전선관, 슬리브(Sleeve), 보호 피복 또는 인클로저 형상에 의한 열전달 제한을 나타낸다. 이러한 계수는 유용한 공학적 체계를 제공하지만 기준 허용 전류(Reference Ampacity)에 적용된 가정과 서로 호환되어야 한다.

번들 구성(Bundle Composition)은 실제 로봇 운전 모드(Operating Mode)를 기준으로 검토해야 한다. 정상 순항 중에는 모터, 컴퓨팅, 센싱 및 통신 회로가 동시에 작동할 수 있다. 가속 또는 경사로 등판 중에는 추진 부하(Propulsion Load)가 지배적일 수 있으며, 충전 중에는 구동 회로가 비활성 상태인 반면 충전 및 배터리 관리 회로(Battery-Management Circuit)에 높은 전류가 흐를 수 있다. 따라서 서로 다른 운전 모드는 서로 다른 최악의 열 조합을 만들 수 있으며, 각 하니스 구간을 지배하는 조합을 파악해야 한다.

가동 구간(Moving Section)은 AMR에 특화된 추가적인 제약을 발생시킨다. 조향 어셈블리(Steering Assembly), 서스펜션 시스템(Suspension System), 휠 모듈(Wheel Module), 매니퓰레이터(Manipulator) 또는 기타 관절형 부품에 연결된 하니스는 전기적 부하를 전달하면서 반복적인 굽힘과 진동을 견뎌야 한다. 도체 크기를 증가시키면 저항과 온도 상승을 줄일 수 있지만 직경과 굽힘 강성(Bending Stiffness)이 증가한다. 따라서 열적 개선은 최소 굽힘 반경(Minimum Bend Radius), 굴곡 수명(Flex Life), 기계적 변형, 패키징 공간 및 커넥터 호환성과 균형을 이루어야 한다.

보호 피복(Protective Covering)은 모바일 로봇에서 진동, 마모, 이물질, 수분, 날카로운 구조물 및 정비 작업으로부터 하니스를 보호해야 하기 때문에 자주 사용된다. 코루게이트 전선관(Corrugated Conduit), 브레이드 슬리브(Braided Sleeve), 테이프 및 튜빙(Tubing)은 기계적 내구성을 향상시키지만 냉각을 제한할 수 있다. 따라서 기계적으로 견고한 AMR 하니스에서도 특히 고전류 도체가 높은 충전율의 보호 피복 내부에 배치될 경우 추가적인 설치 디레이팅(Installation Derating)이 필요할 수 있다.

전압 강하(Voltage Drop)는 열적 디레이팅과 함께 평가해야 한다. 두 요구조건 모두 필요한 도체 단면적(Conductor Cross-Sectional Area)에 영향을 주기 때문이다. 전선이 디레이팅 적용 후 온도 한계를 만족하더라도 배터리에서 부하까지의 긴 전력 경로에서 과도한 전압 손실을 발생시킬 수 있다. 특히 저전압 시스템(Low-Voltage System)에서는 작은 절대 전압 강하도 공급 전압의 상당한 비율을 차지할 수 있으며 모터, 컨트롤러, 컴퓨터 또는 센서 성능을 저하시킬 수 있다.

회로 보호(Circuit Protection) 역시 디레이팅된 도체 용량과 적절하게 협조되어야 한다. 퓨즈(Fuse) 또는 회로 차단기(Circuit Breaker)는 정상적인 과도 운전을 불필요하게 차단하지 않으면서 비정상적인 과부하나 단락 조건에서 전선을 보호해야 한다. 환경 디레이팅(Environmental Derating)으로 도체의 안전한 연속 전류 용량이 감소한다면 보호 장치 설정을 전선의 자유 공기 정격(Free-Air Rating)만으로 결정해서는 안 된다. 따라서 열적 설치 조건과 보호 철학(Protection Philosophy)을 하나의 통합 시스템으로 검토해야 한다.

충전 회로(Charging Circuit)는 로봇이 정지된 상태에서 지속적인 고전류가 흐를 수 있기 때문에 또 다른 중요한 열 조건을 형성한다. 차량의 움직임이 감소하면 정상 주행 상태보다 내부 부품 주변의 공기 흐름도 감소할 수 있다. 배터리 온도, 충전기 손실(Charger Loss), 접촉 저항(Contact Resistance), 밀폐된 충전 하드웨어 역시 국부 온도를 증가시킬 수 있다. 따라서 AMR의 최악 열 조건을 결정할 때 충전 상태(Charging State)를 독립적인 운전 모드로 평가해야 한다.

옥외 AMR(Outdoor AMR)은 제어된 실내 시설에서만 운용되는 로봇보다 넓은 환경 범위(Environmental Envelope)를 고려해야 한다. 태양열(Solar Heating), 높은 계절 주변 온도, 저온 시동(Cold Start), 방진 구조(Dust Protection), 방수 피복(Waterproof Covering), 변화하는 공기 흐름이 하니스 온도에 영향을 줄 수 있다. 수분과 오염에 대한 보호를 위해 필요한 밀폐 구조는 열 방출을 감소시킬 수 있으므로 환경 내구성(Environmental Robustness)과 전기적 전류 용량을 독립적으로 평가해서는 안 된다.

실제 AMR 디레이팅 매트릭스(AMR Derating Matrix)는 각 하니스 구간을 회로 종류, 기준 허용 전류, 국부 온도, 번들 조건, 보호 피복, 듀티 사이클 및 적용 가능한 보정 계수와 연결할 수 있다. 이렇게 계산된 허용 전류를 예상 전기 부하와 비교할 수 있다. 이러한 매트릭스는 시스템 수준의 전력 요구사항에서 개별 도체 선정까지의 추적성(Traceability)을 확보하며, 열적 여유가 부족한 구간을 쉽게 식별할 수 있도록 한다.

열적 여유가 부족한 경우 도체 크기를 증가시키는 것만이 유일한 해결책은 아니다. 추진 케이블(Propulsion Cable)을 다른 번들에서 분리하거나, 전선관 직경을 증가시키고, 충전율(Fill Ratio)을 낮추며, 고전류 경로를 단축하고, 공기 흐름을 개선할 수 있다. 또한 컨트롤러나 모터와 같은 열원으로부터 배선을 멀리 이동시키거나 더 높은 온도 등급의 절연체를 선택하고 보호 피복을 변경할 수도 있다. 경우에 따라 전체 회로의 전선 크기를 증가시키는 것보다 라우팅 변경이 더욱 효과적일 수 있다.

열 검증(Thermal Validation)은 하니스에 임의의 일정 전류만 인가하는 대신 대표적인 로봇 운전 모드를 재현해야 한다. 장시간 순항, 반복적인 가속과 감속, 최대 화물 운전(Maximum Payload Operation), 경사로 등판, 높은 컴퓨팅 사용률(High Compute Utilization), 충전 및 최대 동시 발열을 발생시킬 것으로 예상되는 조합 등이 유용한 시험 조건이다. 시험은 열 축적을 확인할 수 있을 만큼 충분히 지속해야 하며, 연속 부하의 경우 대표적인 열적 평형 상태에 접근할 수 있어야 한다.

온도 측정(Temperature Measurement)은 접근하기 쉬운 외부 표면만이 아니라 예상되는 최악 위치를 중심으로 수행해야 한다. 중요한 위치에는 고밀도 번들의 중심 전선, 배터리 전력 분배 도체, 모터 분기, 커넥터 전환부(Connector Transition), 전선관 내부 구간, 컴퓨팅 구획, 충전 인터페이스 및 모터 컨트롤러나 기타 열원에 인접한 영역이 포함된다. 내부 도체 온도는 슬리브나 전선관 표면 온도보다 높을 수 있으므로 측정 전략에서는 이러한 차이를 고려해야 한다.

검증 결과(Validation Result)는 다시 디레이팅 가정에 반영되어야 한다. 측정 온도가 예상 한계보다 충분히 낮다면 설계가 불필요하게 보수적일 수 있으며, 이로 인해 하니스 질량, 비용 및 강성이 증가할 수 있다. 반대로 측정 온도가 설계 한계에 가까워진다면 추가적인 열적 여유나 개선 대책이 필요하다. 목표는 가능한 가장 큰 도체를 사용하는 것이 아니라 전기적 성능, 열 안전성(Thermal Safety), 기계적 내구성, 패키징 효율(Packaging Efficiency), 정비성(Serviceability) 사이에서 검증된 균형을 확보하는 것이다.

최종 AMR 하니스 설계는 디레이팅을 전기 아키텍처(Electrical Architecture)와 실제 물리적 설치를 연결하는 시스템 수준의 공학 프로세스(System-Level Engineering Process)로 다루어야 한다. Chapter 05에서 설명한 번들 효과(Bundle Effect), 고온 영역, 전선관 및 슬리브에 의한 제한, 환경별 보정(Environment-Specific Correction)은 로봇 수준에서 하나로 통합된다. 이러한 적용은 개별 보정 메커니즘을 추적 가능한 설계 방법으로 변환함으로써 의도된 전체 운용 수명 동안 안전하고 신뢰성 높으며 실용적인 AMR 배선 시스템을 구현하는 것으로 디레이팅 장을 완성한다.
