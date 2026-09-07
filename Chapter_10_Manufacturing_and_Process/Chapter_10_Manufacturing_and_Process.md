**Volume 02. Wire Harness Engineering**


# Chapter 10. Manufacturing and Process

##  

## 10.01. Automatic Cut Strip Crimp

![](images/image1.png){width="7.268055555555556in" height="7.268055555555556in"}

Automatic cut-strip-crimp processing integrates three fundamental wire-harness manufacturing operations into a controlled production sequence: cutting wire to a specified length, removing insulation from the conductor ends, and mechanically attaching terminals by crimping. Within wire harness manufacturing, this process provides the transition from bulk wire and loose terminals to repeatable terminated leads that can later be assembled into connectors and complete harnesses.

The process normally begins with production data defining the wire type, conductor cross-sectional area, insulation characteristics, finished wire length, strip length, terminal part number, and required crimp configuration. Automated equipment converts these engineering specifications into machine parameters. Correct data management is essential because even a mechanically stable machine can continuously produce incorrect parts when the selected wire, terminal, applicator, or dimensional program does not match the released harness definition.

Wire cutting establishes the dimensional foundation of the manufactured lead. A feeding mechanism advances wire from a reel through rollers or belts while an encoder or comparable measuring system determines the required length. The cutting mechanism must produce a clean end without excessively deforming the insulation or conductor. Feed accuracy, wire straightness, roller pressure, blade condition, and acceleration characteristics can influence finished length, particularly when flexible or small-gauge wires are processed at high production speeds.

Stripping removes a controlled section of insulation while preserving the conductor strands underneath. The stripping blades must penetrate sufficiently to separate the insulation but must not nick, cut, scrape, or excessively compress the conductor. Strip length must also correspond to the terminal geometry so that the conductor is positioned correctly inside the conductor crimp while the insulation enters the insulation-support region. Incorrect stripping can therefore create defects that become difficult to detect after the terminal has been crimped.

Crimping creates a permanent mechanical and electrical connection by plastically deforming the terminal wings around the conductor. During automatic processing, the stripped wire is positioned relative to a terminal supplied from a reel or carrier strip, and an applicator forms the terminal using a controlled press stroke. The resulting connection depends on the combined behavior of terminal material, conductor strands, tooling geometry, press setup, crimp height, wire position, and the consistency of the preceding stripping operation.

The conductor crimp and insulation crimp perform different functions. The conductor crimp establishes the principal electrical interface and mechanical retention between the terminal and conductor, while the insulation crimp supports the insulated portion of the wire and reduces mechanical stress near the conductor termination. These regions must therefore be evaluated separately. Excessive compression can damage strands or insulation, whereas insufficient compression can produce high resistance, poor pull strength, unstable contact behavior, or premature fatigue.

Crimp height is one of the most important process characteristics because it provides a practical indication of conductor compression. It is typically controlled for a defined combination of wire size, terminal, and tooling rather than treated as a universal value. Crimp width, terminal geometry, conductor brush position, bellmouth formation, insulation position, and terminal deformation provide additional evidence of process quality. These characteristics are subsequently examined more deeply through crimp cross-section analysis.

Automatic equipment requires precise synchronization between wire feeding, cutting, stripping, terminal feeding, positioning, and press operation. A small timing or alignment error can propagate through the sequence and create repeated defects at production speed. For example, inaccurate strip length can change conductor insertion depth, while unstable terminal feeding can shift the crimp position. Process engineering must consequently consider the entire machine sequence as one coupled manufacturing system rather than treating cutting, stripping, and crimping as independent operations.

Tooling condition strongly influences process capability. Cutting and stripping blades gradually wear, terminal applicators accumulate contamination and mechanical wear, and crimp tooling can lose dimensional consistency after extended production. Preventive maintenance should therefore be based on production quantity, measured condition, and historical process behavior. Tool identification and configuration control are equally important because visually similar terminals may require different applicators, anvils, punches, feed adjustments, or crimp settings.

Production monitoring provides a means of detecting process drift before defective leads propagate into harness assembly. Depending on the equipment and quality strategy, monitored variables can include finished wire length, strip dimensions, crimp force signatures, crimp height measurements, terminal presence, wire presence, and machine alarms. Statistical evaluation of measured characteristics can reveal gradual movement toward specification limits and enables corrective action before the process produces a significant quantity of nonconforming material.

Crimp force monitoring evaluates the force behavior generated during terminal deformation and can identify deviations associated with missing strands, incorrect wire insertion, missing wire, incorrect terminals, or abnormal material conditions. It should not be interpreted as a complete substitute for dimensional and destructive inspection. A force signature indicates whether the forming event differs from an established process pattern, while crimp-height measurement, pull testing, visual inspection, and cross-section analysis provide complementary evidence of actual termination quality.

Machine setup and changeover are particularly important when one production system processes multiple wire-terminal combinations. The operator or manufacturing system must verify the correct wire reel, terminal reel, applicator, program, blade configuration, and inspection criteria before production release. First-off samples are commonly used to demonstrate that the configured process produces acceptable dimensions and termination characteristics before continuous production begins, reducing the risk of systematic defects caused by an incorrect setup.

Traceability connects the manufactured lead to the conditions under which it was produced. Production records may associate a batch with wire and terminal lots, machine identification, applicator identification, tooling status, operator or setup information, process parameters, inspection results, and manufacturing time. Such records become valuable when a later harness inspection identifies a defect because engineers can determine whether the issue is isolated or potentially affects other products manufactured under the same conditions.

Automatic processing improves throughput and repeatability, but automation does not eliminate manufacturing variation. Incoming material tolerances, conductor construction, insulation hardness, terminal dimensional variation, reel handling, tooling wear, machine temperature, contamination, and setup differences can all influence the final termination. A capable manufacturing process therefore combines automation with defined process windows, controlled tooling, preventive maintenance, measurement-system discipline, inspection, and systematic response to abnormal trends.

The manufacturing sequence also influences downstream harness operations. Accurate lead lengths simplify harness-board placement, consistent strip and crimp geometry improves connector insertion, and correctly formed insulation crimps improve mechanical durability during routing and service. Conversely, dimensional variation introduced during automatic processing can appear later as connector-position errors, excessive tension, insufficient slack, assembly difficulty, or reliability problems. Manufacturing quality must therefore be evaluated against the complete harness design intent.

For robotics and AMR harnesses, process consistency becomes particularly important because terminated wires may operate near motors, batteries, sensors, computing systems, and moving mechanical assemblies. Electrical resistance, mechanical retention, and strain resistance must remain predictable despite vibration and repeated operating cycles. Automatic cut-strip-crimp manufacturing provides the repeatable production foundation, while subsequent harness-board assembly, standardized work instructions, and first-article inspection extend that control to the completed harness manufacturing process.

자동 절단-탈피-압착(Automatic Cut-Strip-Crimp) 공정은 와이어 하니스(Wire Harness) 제조의 세 가지 기본 작업인 지정 길이로 와이어를 절단(Cutting)하고, 도체 끝단의 절연체를 제거하는 탈피(Stripping)를 수행하며, 압착(Crimping)을 통해 터미널(Terminal)을 기계적으로 체결하는 작업을 하나의 제어된 생산 순서로 통합한다. 이 공정은 벌크 와이어(Bulk Wire)와 개별 터미널을 반복 생산이 가능한 터미널 체결 리드(Terminated Lead)로 변환하며, 이후 커넥터(Connector)와 완성 하니스(Harness) 조립의 기반이 된다.

공정은 일반적으로 와이어 종류, 도체 단면적(Conductor Cross-Sectional Area), 절연 특성, 완성 와이어 길이, 탈피 길이(Strip Length), 터미널 부품 번호 및 필요한 압착 구성을 정의한 생산 데이터에서 시작한다. 자동화 장비(Automated Equipment)는 이러한 엔지니어링 사양을 기계 파라미터(Machine Parameter)로 변환한다. 따라서 와이어, 터미널, 어플리케이터(Applicator), 치수 프로그램이 승인된 하니스 정의와 일치하도록 정확한 데이터 관리가 필요하다.

와이어 절단(Wire Cutting)은 제조되는 리드의 치수 정확성을 결정하는 기초 공정이다. 공급 메커니즘(Feeding Mechanism)이 롤러 또는 벨트를 통해 릴(Reel)의 와이어를 이송하고, 엔코더(Encoder) 등의 측정 시스템으로 필요한 길이를 결정한다. 절단 장치는 절연체나 도체를 과도하게 변형시키지 않으면서 깨끗한 절단면을 만들어야 한다. 공급 정확도, 와이어 직진성, 롤러 압력, 블레이드 상태 및 가감속 특성은 특히 유연하거나 작은 규격의 와이어를 고속으로 처리할 때 완성 길이에 영향을 줄 수 있다.

탈피(Stripping)는 내부 도체 가닥(Conductor Strand)을 보존하면서 일정 길이의 절연체를 제거하는 작업이다. 탈피 블레이드(Stripping Blade)는 절연체를 분리할 만큼 충분히 침투해야 하지만 도체를 찍거나 절단하거나 긁거나 과도하게 압축해서는 안 된다. 또한 탈피 길이는 터미널 형상과 일치해야 하며, 도체가 도체 압착부(Conductor Crimp)에 정확히 위치하면서 절연체는 절연 지지 영역에 들어가야 한다. 잘못된 탈피는 터미널 압착 이후 발견하기 어려운 결함을 발생시킬 수 있다.

압착(Crimping)은 터미널 윙(Terminal Wing)을 도체 주위에서 소성 변형(Plastic Deformation)시켜 영구적인 기계적·전기적 연결을 형성한다. 자동 공정에서는 탈피된 와이어가 릴 또는 캐리어 스트립(Carrier Strip)에서 공급되는 터미널에 맞춰 위치하고, 어플리케이터가 제어된 프레스 스트로크(Press Stroke)를 이용하여 터미널을 성형한다. 연결 품질은 터미널 재질, 도체 가닥, 금형 형상, 프레스 설정, 압착 높이(Crimp Height), 와이어 위치 및 선행 탈피 공정의 일관성에 의해 결정된다.

도체 압착부(Conductor Crimp)와 절연 압착부(Insulation Crimp)는 서로 다른 기능을 수행한다. 도체 압착부는 터미널과 도체 사이의 핵심 전기적 접속과 기계적 유지력을 형성하고, 절연 압착부는 와이어의 절연 부분을 지지하여 단자부 근처의 기계적 응력을 줄인다. 따라서 두 영역은 별도로 평가해야 한다. 과도한 압축은 도체 가닥이나 절연체를 손상시킬 수 있고, 압축이 부족하면 높은 저항, 낮은 인장 강도(Pull Strength), 불안정한 접촉 또는 조기 피로 파손이 발생할 수 있다.

압착 높이(Crimp Height)는 도체 압축 상태를 실용적으로 나타낼 수 있기 때문에 가장 중요한 공정 특성 중 하나이다. 이는 보편적인 단일 값이 아니라 특정 와이어 크기, 터미널 및 금형 조합에 대해 관리된다. 압착 폭(Crimp Width), 터미널 형상, 도체 브러시 위치(Conductor Brush Position), 벨마우스(Bellmouth) 형성, 절연체 위치 및 터미널 변형 상태 역시 공정 품질을 판단하는 중요한 근거를 제공한다. 이러한 특성은 이후 압착 단면 분석(Crimp Cross-Section Analysis)을 통해 더욱 상세하게 평가된다.

자동화 장비는 와이어 공급, 절단, 탈피, 터미널 공급, 위치 결정 및 프레스 작동 사이의 정밀한 동기화(Synchronization)를 필요로 한다. 작은 타이밍 또는 정렬 오차도 전체 공정 순서를 따라 전파되어 생산 속도에 비례하는 반복 결함을 만들 수 있다. 예를 들어 부정확한 탈피 길이는 도체 삽입 깊이를 변화시키며, 불안정한 터미널 공급은 압착 위치를 이동시킬 수 있다. 따라서 공정 엔지니어링(Process Engineering)은 절단, 탈피 및 압착을 독립된 작업이 아니라 하나의 결합된 제조 시스템으로 관리해야 한다.

금형 상태(Tooling Condition)는 공정 능력(Process Capability)에 직접적인 영향을 준다. 절단 및 탈피 블레이드는 점진적으로 마모되고, 터미널 어플리케이터에는 오염과 기계적 마모가 축적되며, 압착 금형(Crimp Tooling)은 장기간 생산 후 치수 일관성이 저하될 수 있다. 따라서 예방 정비(Preventive Maintenance)는 생산 수량, 측정된 상태 및 과거 공정 특성을 기반으로 수행해야 한다. 외형이 유사한 터미널도 서로 다른 어플리케이터, 앤빌(Anvil), 펀치(Punch), 공급 조정 또는 압착 설정을 요구할 수 있으므로 금형 식별과 구성 관리(Configuration Control)도 중요하다.

생산 모니터링(Production Monitoring)은 불량 리드가 하니스 조립 공정으로 전달되기 전에 공정 드리프트(Process Drift)를 검출하는 수단을 제공한다. 장비와 품질 관리 전략에 따라 완성 와이어 길이, 탈피 치수, 압착력 신호(Crimp Force Signature), 압착 높이 측정값, 터미널 존재 여부, 와이어 존재 여부 및 장비 알람 등을 감시할 수 있다. 측정 특성의 통계적 평가는 규격 한계를 향해 점진적으로 이동하는 경향을 발견하고 대량의 부적합품이 발생하기 전에 시정 조치를 수행할 수 있도록 한다.

압착력 모니터링(Crimp Force Monitoring)은 터미널 변형 과정에서 발생하는 힘의 특성을 평가하며, 도체 가닥 누락, 부정확한 와이어 삽입, 와이어 누락, 잘못된 터미널 또는 비정상적인 재료 상태와 관련된 편차를 검출할 수 있다. 그러나 이를 치수 검사나 파괴 검사(Destructive Inspection)를 완전히 대체하는 방법으로 사용해서는 안 된다. 압착력 신호는 성형 과정이 정상 공정 패턴과 다른지를 나타내며, 압착 높이 측정, 인장 시험(Pull Testing), 육안 검사 및 단면 분석이 실제 체결 품질을 보완적으로 검증한다.

하나의 생산 시스템에서 여러 와이어-터미널 조합을 처리하는 경우 장비 설정과 교체 작업(Changeover)이 특히 중요하다. 작업자 또는 제조 시스템은 생산을 시작하기 전에 올바른 와이어 릴, 터미널 릴, 어플리케이터, 프로그램, 블레이드 구성 및 검사 기준을 확인해야 한다. 초품 샘플(First-Off Sample)은 일반적으로 연속 생산에 들어가기 전에 설정된 공정이 허용 가능한 치수와 체결 특성을 만들어내는지 확인하는 데 사용되며, 잘못된 설정으로 인한 체계적 결함의 위험을 감소시킨다.

추적성(Traceability)은 제조된 리드와 해당 리드가 생산된 공정 조건을 연결한다. 생산 기록에는 와이어 및 터미널 로트(Lot), 장비 식별 정보, 어플리케이터 식별 정보, 금형 상태, 작업자 또는 설정 정보, 공정 파라미터, 검사 결과 및 제조 시간 등이 포함될 수 있다. 이후 하니스 검사에서 결함이 발견되었을 때 이러한 기록을 이용하면 해당 문제가 개별적인 문제인지 또는 동일한 조건에서 제조된 다른 제품에도 영향을 줄 가능성이 있는지를 판단할 수 있다.

자동화 공정은 생산성(Throughput)과 반복성(Repeatability)을 향상시키지만 제조 편차를 완전히 제거하지는 않는다. 입고 재료 공차, 도체 구조, 절연체 경도, 터미널 치수 편차, 릴 취급, 금형 마모, 장비 온도, 오염 및 설정 차이 등이 최종 체결 상태에 영향을 줄 수 있다. 따라서 안정적인 제조 공정은 자동화와 함께 정의된 공정 윈도(Process Window), 금형 관리, 예방 정비, 측정 시스템 관리, 검사 및 비정상 경향에 대한 체계적인 대응을 결합해야 한다.

자동 공정은 이후의 하니스 제조 작업에도 직접적인 영향을 미친다. 정확한 리드 길이는 하니스 보드(Harness Board) 배치를 용이하게 하고, 일관된 탈피 및 압착 형상은 커넥터 삽입성을 향상시키며, 적절하게 형성된 절연 압착부는 배선 및 정비 과정의 기계적 내구성을 높인다. 반대로 자동 공정에서 발생한 치수 편차는 이후 커넥터 위치 오류, 과도한 장력, 부족한 여유 길이, 조립 어려움 또는 신뢰성 문제로 나타날 수 있다. 따라서 제조 품질은 전체 하니스 설계 의도(Harness Design Intent)를 기준으로 평가해야 한다.

로보틱스(Robotics) 및 자율이동로봇(AMR, Autonomous Mobile Robot) 하니스에서는 터미널 처리된 와이어가 모터, 배터리, 센서, 컴퓨팅 시스템 및 움직이는 기계 구조물 주변에서 동작할 수 있으므로 공정 일관성이 특히 중요하다. 전기 저항, 기계적 유지력 및 변형 저항은 진동과 반복적인 동작 주기에서도 예측 가능한 수준으로 유지되어야 한다. 자동 절단-탈피-압착(Automatic Cut-Strip-Crimp)은 이러한 반복 생산의 기반을 제공하며, 이후 하니스 보드 조립, 표준 작업 지침(Standardized Work Instruction) 및 초도품 검사(First Article Inspection)를 통해 완성 하니스까지 제조 관리가 확장된다.

##  

## 10.02. Crimp Quality Cross Section

![](images/image2.png){width="7.268055555555556in" height="7.268055555555556in"}

Crimp quality cross-section analysis is a destructive inspection method used to evaluate the internal geometry of a crimped terminal after the conductor and terminal wings have been mechanically compressed together. While external inspection can identify visible deformation, conductor position, bellmouth, or insulation-related defects, a prepared cross-section reveals how individual conductor strands, terminal wings, and compressed material actually interact inside the crimp. It is therefore an important verification method within wire harness manufacturing.

A cross-section is normally prepared by cutting the crimped terminal at a defined location through the conductor crimp region. The sample must be sectioned without introducing excessive mechanical deformation that could alter the geometry being inspected. After cutting, the exposed surface is typically prepared so that the boundaries of conductor strands, terminal material, voids, and compressed regions can be clearly distinguished. Consistent sample preparation is essential because poor preparation can create artifacts that may be incorrectly interpreted as manufacturing defects.

The inspection plane must represent the region intended for evaluation. A section taken too close to the bellmouth, transition region, or terminal edge may not represent the stable compression geometry of the conductor crimp. For this reason, manufacturing specifications normally define where the terminal should be sectioned. Repeatable section positioning enables measurements from different production samples, machines, applicators, and manufacturing lots to be compared under equivalent geometric conditions.

Crimp height is one of the primary characteristics associated with cross-sectional quality. It represents the final compressed height of the conductor crimp and provides an indirect indication of the degree of compression applied to the wire-terminal combination. A crimp height that is too large may indicate insufficient compression, while an excessively small value can indicate over-compression. The acceptable range must be established for the specific terminal, conductor size, conductor construction, and tooling combination rather than treated as a universal requirement.

Crimp width provides complementary information about terminal deformation. During crimping, the terminal wings move around the conductor and are formed by the punch and anvil geometry. The resulting width, together with crimp height, helps characterize the final shape of the compressed connection. Unexpected width can indicate tooling problems, incorrect terminal selection, positioning errors, or abnormal forming behavior, especially when the measured geometry differs systematically from validated production samples.

The arrangement of conductor strands inside the crimp is another major inspection characteristic. Individual strands should be contained within the intended conductor crimp region and compressed into a stable structure without excessive strand damage. Missing strands reduce the effective conductor area, while displaced or cut strands can reduce mechanical retention and alter electrical performance. Cross-sectional inspection makes these conditions visible even when the external appearance of the terminal appears acceptable.

Compression must be sufficient to create intimate mechanical contact between conductor strands and the terminal while avoiding destructive deformation. Under-compression can leave excessive internal gaps and produce an unstable connection with increased electrical resistance or reduced pull strength. Over-compression can severely deform conductor strands, reduce their effective cross-sectional area, damage the terminal, or introduce stress concentrations. Cross-section analysis therefore evaluates not simply whether compression occurred, but whether an appropriate compressed structure was produced.

Terminal wing formation is particularly important because the wings must wrap and form around the conductor in the geometry intended by the terminal design. Cross-sectional examination can reveal asymmetric wing formation, insufficient closure, excessive overlap, abnormal curling, or contact between regions that should remain separated. Such patterns can indicate applicator alignment problems, incorrect crimp settings, worn tooling, incorrect wire positioning, or a mismatch between the terminal and conductor.

Symmetry provides useful information about the mechanical condition of the crimping process. A correctly aligned punch, anvil, terminal, and conductor generally produces a repeatable cross-sectional pattern appropriate to the terminal design. Significant asymmetry may indicate that the terminal entered the tooling incorrectly, the conductor was displaced before compression, or the tooling alignment has changed. Trending cross-sectional geometry over time can therefore help distinguish isolated material variation from progressive equipment-related process drift.

Internal voids must be interpreted in relation to conductor construction, terminal geometry, and the validated crimp specification. The objective is not necessarily to eliminate every microscopic space between strands, but to achieve the intended degree and distribution of compression. Large or abnormal void regions may indicate insufficient compression, incorrect conductor fill, missing strands, or an unsuitable wire-terminal combination. Evaluation criteria should therefore rely on defined engineering requirements rather than subjective visual expectations.

Cross-section analysis should be considered together with external crimp characteristics such as conductor brush position, bellmouth formation, insulation position, terminal deformation, and the relationship between the conductor crimp and insulation crimp. These features describe different parts of the termination process. A cross-section can confirm the internal conductor connection, while external inspection verifies whether the wire entered and exited the terminal correctly and whether adjacent terminal features were formed without damage.

Electrical and mechanical performance are closely related to the internal structure revealed by the cross-section. Effective compression increases contact between conductor strands and terminal surfaces, supporting a stable low-resistance interface. At the same time, the crimp must provide sufficient mechanical retention to withstand handling, routing, vibration, and service loads. Pull testing provides direct mechanical evidence, while resistance measurement can evaluate electrical behavior; cross-section inspection explains the geometric condition responsible for those measured results.

Cross-sectional inspection is especially valuable during machine setup, tooling qualification, first-off approval, process validation, and investigation of abnormal production results. When an applicator, punch, anvil, terminal, wire type, or crimp setting changes, representative samples can be sectioned to confirm that the resulting internal geometry remains acceptable. This provides evidence that dimensional machine settings translate into the physical terminal-conductor structure required by the manufacturing specification.

Crimp force monitoring and cross-section inspection perform complementary roles. Force monitoring can operate during production and detect changes in the crimping event, such as missing strands, incorrect insertion, abnormal terminal conditions, or other deviations from an established force signature. Cross-section inspection is destructive and therefore normally applied to selected samples rather than every product, but it provides direct geometric evidence. Combining both approaches improves detection of both continuous process drift and internal structural defects.

Inspection results become more valuable when integrated with manufacturing traceability. Cross-section images and measurements can be associated with wire lot, terminal lot, machine identification, applicator identification, tooling condition, crimp settings, production date, and first-article records. When a later defect occurs, these records help determine whether the abnormality originated from material variation, tooling wear, machine setup, operator changeover, or another manufacturing condition affecting a specific production population.

For robotics and AMR harnesses, reliable crimp geometry is important because electrical connections may experience vibration, repeated movement, temperature variation, and long operating cycles near motors, batteries, sensors, and computing systems. Cross-section analysis provides manufacturing evidence that the terminal-conductor interface was formed correctly before the lead enters harness assembly. Together with automatic cut-strip-crimp control, standardized work instructions, and first-article inspection, it forms part of an end-to-end strategy for producing reliable wire harnesses.

압착 품질 단면 분석(Crimp Quality Cross-Section Analysis)은 도체(Conductor)와 터미널 윙(Terminal Wing)이 기계적으로 압축된 이후 압착 터미널(Crimped Terminal)의 내부 형상을 평가하는 파괴 검사(Destructive Inspection) 방법이다. 외관 검사를 통해 눈에 보이는 변형, 도체 위치, 벨마우스(Bellmouth), 절연 관련 결함을 확인할 수 있는 반면, 준비된 단면에서는 개별 도체 가닥, 터미널 윙 및 압축된 재료가 압착 내부에서 실제로 어떻게 결합되어 있는지를 확인할 수 있다. 따라서 와이어 하니스(Wire Harness) 제조에서 중요한 검증 방법이다.

단면은 일반적으로 도체 압착 영역(Conductor Crimp Region)의 정해진 위치에서 압착된 터미널을 절단하여 준비한다. 검사할 형상이 변형되지 않도록 시편(Sample)을 절단하는 과정에서 과도한 기계적 변형이 발생하지 않아야 한다. 절단 이후에는 도체 가닥, 터미널 재료, 공극(Void) 및 압축 영역의 경계를 명확하게 구분할 수 있도록 노출된 표면을 준비한다. 시편 준비 과정이 불량하면 제조 결함으로 잘못 해석될 수 있는 인공적인 흔적(Artifact)이 발생할 수 있으므로 일관된 시편 준비가 중요하다.

검사 단면(Inspection Plane)은 평가하려는 영역을 대표해야 한다. 벨마우스, 전이 영역(Transition Region) 또는 터미널 가장자리에 지나치게 가까운 위치에서 절단하면 안정적인 도체 압착 형상을 대표하지 못할 수 있다. 따라서 제조 사양(Manufacturing Specification)에서는 일반적으로 터미널을 절단해야 하는 위치를 정의한다. 반복 가능한 단면 위치를 사용하면 서로 다른 생산 시편, 장비, 어플리케이터(Applicator) 및 제조 로트(Manufacturing Lot)의 측정 결과를 동일한 형상 조건에서 비교할 수 있다.

압착 높이(Crimp Height)는 단면 품질과 관련된 주요 특성 중 하나이다. 이는 도체 압착부의 최종 압축 높이를 나타내며 와이어-터미널 조합에 적용된 압축 정도를 간접적으로 보여준다. 압착 높이가 지나치게 크면 압축 부족(Under-Compression)을 의미할 수 있으며, 지나치게 작으면 과도한 압축(Over-Compression)을 나타낼 수 있다. 허용 범위는 보편적인 요구값이 아니라 특정 터미널, 도체 크기, 도체 구조 및 금형(Tooling) 조합에 대해 설정되어야 한다.

압착 폭(Crimp Width)은 터미널 변형 상태에 대한 보완적인 정보를 제공한다. 압착 과정에서 터미널 윙은 도체 주위로 이동하며 펀치(Punch)와 앤빌(Anvil)의 형상에 의해 성형된다. 최종적으로 형성된 폭은 압착 높이와 함께 압축된 연결부의 최종 형상을 나타낸다. 특히 측정된 형상이 검증된 생산 시편과 체계적으로 다를 경우 비정상적인 압착 폭은 금형 문제, 잘못된 터미널 선택, 위치 오차 또는 비정상적인 성형 거동을 나타낼 수 있다.

압착부 내부의 도체 가닥 배열(Conductor Strand Arrangement) 역시 중요한 검사 특성이다. 개별 가닥은 의도된 도체 압착 영역 내부에 위치하고 과도한 가닥 손상 없이 안정적인 구조로 압축되어야 한다. 가닥 누락(Missing Strand)은 유효 도체 단면적을 감소시키며, 위치가 벗어나거나 절단된 가닥은 기계적 유지력을 감소시키고 전기적 성능을 변화시킬 수 있다. 단면 검사를 이용하면 터미널의 외관이 정상적으로 보이는 경우에도 이러한 내부 상태를 확인할 수 있다.

압축(Compression)은 도체 가닥과 터미널 사이에 긴밀한 기계적 접촉을 형성할 수 있을 정도로 충분해야 하지만 파괴적인 변형은 방지해야 한다. 압축 부족은 과도한 내부 공극을 남겨 전기 저항 증가 또는 인장 강도(Pull Strength) 저하를 동반하는 불안정한 연결을 만들 수 있다. 반대로 과도한 압축은 도체 가닥을 심하게 변형시키고 유효 단면적을 감소시키며 터미널 손상이나 응력 집중(Stress Concentration)을 발생시킬 수 있다. 따라서 단면 분석은 단순히 압축 여부가 아니라 적절한 압축 구조가 형성되었는지를 평가한다.

터미널 윙 성형(Terminal Wing Formation)은 터미널 설계에서 의도한 형상에 따라 윙이 도체 주위를 감싸면서 형성되어야 하므로 특히 중요하다. 단면 검사를 통해 비대칭 윙 성형, 불충분한 폐쇄, 과도한 중첩, 비정상적인 말림(Curling) 또는 서로 분리되어야 하는 영역 사이의 접촉 등을 확인할 수 있다. 이러한 형태는 어플리케이터 정렬 문제, 잘못된 압착 설정, 금형 마모, 부정확한 와이어 위치 또는 터미널과 도체 사이의 부적절한 조합을 나타낼 수 있다.

대칭성(Symmetry)은 압착 공정의 기계적 상태를 판단하는 유용한 정보를 제공한다. 정확하게 정렬된 펀치, 앤빌, 터미널 및 도체는 일반적으로 해당 터미널 설계에 적합한 반복 가능한 단면 형상을 생성한다. 심각한 비대칭은 터미널이 금형 내부로 잘못 진입했거나 압축 전에 도체 위치가 이동했거나 금형 정렬 상태가 변화했음을 의미할 수 있다. 따라서 시간에 따른 단면 형상의 경향 분석(Trending)을 통해 일시적인 재료 편차와 점진적인 장비 관련 공정 드리프트(Process Drift)를 구분할 수 있다.

내부 공극(Internal Void)은 도체 구조, 터미널 형상 및 검증된 압착 사양과의 관계를 고려하여 해석해야 한다. 목적은 도체 가닥 사이의 모든 미세한 공간을 반드시 제거하는 것이 아니라 의도된 압축 정도와 압축 분포를 달성하는 것이다. 크거나 비정상적인 공극 영역은 압축 부족, 부정확한 도체 충전(Conductor Fill), 가닥 누락 또는 부적절한 와이어-터미널 조합을 나타낼 수 있다. 따라서 평가 기준은 주관적인 외관 판단이 아니라 정의된 엔지니어링 요구사항(Engineering Requirement)을 기반으로 해야 한다.

단면 분석은 도체 브러시 위치(Conductor Brush Position), 벨마우스 형성, 절연체 위치, 터미널 변형 및 도체 압착부와 절연 압착부(Insulation Crimp) 사이의 관계와 같은 외부 압착 특성과 함께 고려해야 한다. 이러한 특성들은 터미널 체결 공정의 서로 다른 부분을 설명한다. 단면 검사는 내부 도체 연결 상태를 확인할 수 있으며, 외관 검사는 와이어가 터미널 내부로 올바르게 진입하고 빠져나오는지와 인접한 터미널 형상이 손상 없이 형성되었는지를 검증한다.

전기적·기계적 성능은 단면을 통해 확인되는 내부 구조와 밀접하게 관련된다. 효과적인 압축은 도체 가닥과 터미널 표면 사이의 접촉을 증가시켜 안정적이고 낮은 저항의 인터페이스(Low-Resistance Interface)를 형성한다. 동시에 압착부는 취급, 배선, 진동 및 실제 사용 환경의 하중을 견딜 수 있는 충분한 기계적 유지력을 제공해야 한다. 인장 시험(Pull Testing)은 직접적인 기계적 성능을 제공하고 저항 측정(Resistance Measurement)은 전기적 특성을 평가하며, 단면 검사는 이러한 측정 결과를 발생시키는 내부 형상 조건을 설명한다.

단면 검사는 장비 설정(Machine Setup), 금형 검증(Tooling Qualification), 초품 승인(First-Off Approval), 공정 검증(Process Validation) 및 비정상적인 생산 결과의 원인 조사에서 특히 유용하다. 어플리케이터, 펀치, 앤빌, 터미널, 와이어 종류 또는 압착 설정이 변경되면 대표 시편을 절단하여 내부 형상이 허용 가능한 상태로 유지되는지 확인할 수 있다. 이를 통해 기계의 치수 설정이 제조 사양에서 요구하는 실제 터미널-도체 구조로 구현되었음을 검증할 수 있다.

압착력 모니터링(Crimp Force Monitoring)과 단면 검사는 상호 보완적인 역할을 수행한다. 압착력 모니터링은 생산 중에 동작하면서 가닥 누락, 부정확한 삽입, 비정상적인 터미널 상태 또는 기존 압착력 신호(Crimp Force Signature)에서 벗어나는 변화를 감지할 수 있다. 단면 검사는 파괴 검사이므로 일반적으로 모든 제품이 아닌 선택된 시편에 적용되지만 직접적인 내부 형상 정보를 제공한다. 두 방법을 함께 사용하면 지속적인 공정 드리프트와 내부 구조 결함을 보다 효과적으로 검출할 수 있다.

검사 결과는 제조 추적성(Manufacturing Traceability)과 통합할 때 더욱 높은 가치를 가진다. 단면 이미지와 측정 결과를 와이어 로트(Wire Lot), 터미널 로트(Terminal Lot), 장비 식별 정보, 어플리케이터 식별 정보, 금형 상태, 압착 설정, 생산 날짜 및 초도품 기록(First-Article Record)과 연계할 수 있다. 이후 결함이 발생하면 이러한 기록을 이용하여 이상이 재료 편차, 금형 마모, 장비 설정, 작업자 교체 작업(Changeover) 또는 특정 생산군에 영향을 미친 다른 제조 조건에서 발생했는지 판단할 수 있다.

로보틱스(Robotics) 및 자율이동로봇(AMR, Autonomous Mobile Robot) 하니스에서는 전기 연결부가 모터, 배터리, 센서 및 컴퓨팅 시스템 주변에서 진동, 반복 운동, 온도 변화 및 장기간의 작동 주기에 노출될 수 있으므로 신뢰성 있는 압착 형상이 중요하다. 단면 분석은 리드(Lead)가 하니스 조립으로 이동하기 전에 터미널-도체 인터페이스가 올바르게 형성되었다는 제조상의 근거를 제공한다. 자동 절단-탈피-압착(Automatic Cut-Strip-Crimp) 관리, 표준 작업 지침(Standardized Work Instruction), 초도품 검사(First Article Inspection)와 함께 신뢰성 높은 와이어 하니스를 생산하기 위한 종단 간 품질 전략(End-to-End Quality Strategy)을 구성한다.

##  

## 10.03. Harness Board Layout

![](images/image3.png){width="7.268055555555556in" height="7.268055555555556in"}

A harness board provides the physical manufacturing reference used to assemble individual wires, branches, connectors, splices, protective coverings, and attachment components into the final wire harness geometry. Within the manufacturing sequence, it converts the electrical and mechanical harness design into a repeatable assembly arrangement. The board allows operators to position components according to controlled dimensions before wrapping, clipping, inspection, and final removal of the completed harness.

Harness board layout begins with the released harness definition rather than with operator interpretation. Engineering information such as connector locations, branch points, wire lengths, splice locations, breakout directions, protective materials, clamps, grommets, and dimensional tolerances must be translated into physical board features. The layout should represent the intended installed geometry sufficiently well that a harness assembled on the board can later be routed into the robot, vehicle, machine, or equipment without excessive tension or dimensional adjustment.

The board normally represents the harness in a flattened manufacturing form rather than reproducing every three-dimensional installed condition. Complex routing paths are transformed into practical two-dimensional assembly geometry while preserving critical lengths, branch relationships, breakout directions, and interface positions. This requires careful consideration because an inappropriate flattening method can produce correct board dimensions but incorrect installed behavior when branches must rotate, bend, or enter connectors from specific directions.

Reference points establish the dimensional framework of the layout. Major connectors, terminals, branch junctions, splices, grommets, clips, and other controlled features are positioned relative to defined datums. These references enable dimensional verification and reduce accumulated error across long harness paths. Critical interface points should receive greater positional control than flexible intermediate sections because connector mating, mounting clips, pass-through features, and service interfaces often have limited installation tolerance.

Fixtures and routing aids physically maintain the harness geometry during assembly. Pins, posts, forks, connector holders, clamps, and dedicated nests can guide main trunks and branches while preventing uncontrolled movement. Their placement should constrain the harness sufficiently for repeatable manufacturing without introducing unrealistic tension or sharp bending. Fixtures must also allow operators to install and remove the harness efficiently without damaging insulation, terminals, connectors, sleeves, or other protective components.

Connector holders are particularly important because connector orientation affects branch direction and downstream installation. A connector positioned at the correct location but rotated incorrectly can create wire twisting or unfavorable breakout geometry when installed in the product. The board should therefore control connector position and, where necessary, orientation. Adequate working space around each connector is also required for wire insertion, secondary-lock operation, inspection, labeling, and other assembly activities.

Branch points define where the main harness trunk divides into smaller routing paths. Their locations and breakout angles influence both dimensional accuracy and installed mechanical stress. Board layout should maintain the specified branch length while providing sufficient transition distance for the wire bundle to change direction naturally. Excessively sharp branch geometry can encourage tight bending, local compression, tape accumulation, or strain near splices and connector exits.

Splice locations require deliberate board positioning because multiple wires may converge into a relatively stiff local structure. The board should provide enough space for the splice and any associated insulation, sealing, heat-shrink material, or protective covering while maintaining the intended distance from branch points, connectors, and high-flex regions. Consistent splice positioning also improves repeatability during downstream inspection and helps ensure that rigid sections do not appear at mechanically unfavorable installation locations.

Harness dimensions must distinguish between controlled interface dimensions and flexible routing dimensions. Not every section requires the same tolerance. Dimensions between fixed connectors, mounting clips, grommets, or other installation interfaces can be functionally critical, whereas intermediate bundle paths may tolerate greater variation. A well-designed board therefore concentrates dimensional control where variation affects installation, electrical connection, serviceability, or mechanical durability rather than attempting to rigidly constrain every millimeter of the harness.

Wire and bundle slack must be intentionally managed. Too little length can generate tensile loading during assembly or installation, while excessive length can produce loops, interference, abrasion, or inconsistent packaging. The board should establish the intended relationship between nominal length and necessary manufacturing or installation allowance. This becomes especially important around moving mechanisms, service loops, connector interfaces, and components where tolerance accumulation can otherwise create unexpected tension.

Protective coverings influence board layout because braid sleeves, tape wrapping, corrugated conduit, grommets, and other protection components require installation space and defined start and stop positions. The preceding packaging and protection design therefore becomes manufacturing information on the harness board. Operators must be able to identify where coverings begin, overlap, terminate, or transition without relying on subjective judgment, particularly where protection boundaries correspond to abrasion, temperature, vibration, or environmental exposure zones.

The assembly sequence should influence fixture placement. Components installed early must remain accessible after additional wires and branches are added, while later operations such as taping, sleeve installation, connector completion, labeling, and clipping require adequate hand and tool access. A geometrically accurate board can still be inefficient if fixtures obstruct the normal assembly sequence. Layout engineering therefore combines dimensional control with manufacturing ergonomics and process flow.

Visual management can reduce assembly errors by making the intended configuration immediately recognizable. Clearly identified connector positions, branch paths, splice locations, component references, protection boundaries, and inspection points help operators distinguish similar features. The board should support the corresponding work instruction rather than become an uncontrolled substitute for it. Production information must remain consistent with released drawings, bills of material, process specifications, and revision-controlled manufacturing documentation.

Error prevention can be incorporated into the physical layout through poka-yoke principles. Connector nests can restrict incorrect orientation, fixture geometry can distinguish similar branches, and dedicated locations can help prevent missing clips or components. Such features are especially valuable when a harness contains repeated connectors, symmetrical branches, or similar wire groups. The objective is to make incorrect assembly difficult while allowing the correct assembly sequence to remain simple and efficient.

Board design must also consider inspection. Critical dimensions should remain measurable, connector and terminal conditions should remain visible where required, and inspectors should be able to verify component presence, branch orientation, protection placement, labels, clips, and other controlled features. Inspection access becomes particularly important before wrapping or coverings hide underlying wires and splices. Intermediate inspection points may therefore be integrated into the assembly sequence rather than relying only on final inspection.

Change control is essential because the harness board represents physical manufacturing information. A design revision that changes a connector, branch length, splice position, protective covering, clip, or routing interface may require corresponding fixture modification. Board identification, revision status, fixture calibration or verification records, and released manufacturing documentation should remain synchronized so that obsolete layouts cannot continue producing harnesses after the engineering definition has changed.

For robotics and AMR applications, harness board accuracy directly supports installation into compact and mechanically active systems. Harnesses may connect batteries, motor controllers, sensors, computing devices, communication networks, charging interfaces, and moving drive modules within limited packaging space. A controlled board layout helps ensure that manufactured harnesses repeatedly fit these interfaces while maintaining the routing, slack, protection, and mechanical relationships established during harness engineering.

Harness board assembly ultimately connects upstream automatic cut-strip-crimp processing and crimp quality verification with downstream standardized work and first-article inspection. Accurate terminated leads alone do not guarantee a correct harness if their spatial relationships are assembled incorrectly. The harness board provides the manufacturing geometry that integrates those individual components into a controlled product, forming a central link between wire preparation, assembly process control, inspection, and reliable final harness production.

하니스 보드(Harness Board)는 개별 와이어, 분기부(Branch), 커넥터(Connector), 스플라이스(Splice), 보호재(Protective Covering), 고정 부품(Attachment Component)을 최종 와이어 하니스(Wire Harness) 형상으로 조립하기 위해 사용하는 물리적인 제조 기준이다. 제조 공정에서 하니스 보드는 전기적·기계적 하니스 설계를 반복 가능한 조립 형상으로 변환한다. 작업자는 보드에서 부품을 관리된 치수에 따라 배치한 후 래핑(Wrapping), 클립 장착, 검사 및 완성된 하니스의 최종 분리를 수행할 수 있다.

하니스 보드 레이아웃(Harness Board Layout)은 작업자의 주관적인 판단이 아니라 승인된 하니스 정의(Released Harness Definition)를 기반으로 시작해야 한다. 커넥터 위치, 분기점, 와이어 길이, 스플라이스 위치, 분기 방향(Breakout Direction), 보호재, 클램프(Clamp), 그로밋(Grommet), 치수 공차 등의 엔지니어링 정보를 실제 보드의 물리적 요소로 변환해야 한다. 보드에서 조립된 하니스가 로봇, 차량, 기계 또는 장비에 설치될 때 과도한 장력이나 치수 조정 없이 배선될 수 있도록 의도된 설치 형상을 충분히 반영해야 한다.

보드는 일반적으로 모든 3차원 설치 상태를 그대로 재현하는 것이 아니라 하니스를 평면화된 제조 형상(Flattened Manufacturing Form)으로 표현한다. 복잡한 배선 경로를 실용적인 2차원 조립 형상으로 변환하면서 중요한 길이, 분기 관계, 분기 방향 및 인터페이스 위치를 유지한다. 부적절하게 평면화하면 보드상의 치수는 정확하더라도 실제 설치 과정에서 분기가 회전하거나 굽혀져야 하거나 특정 방향으로 커넥터에 진입해야 할 때 잘못된 설치 형상이 발생할 수 있으므로 주의해야 한다.

기준점(Reference Point)은 레이아웃의 치수 체계를 설정한다. 주요 커넥터, 터미널(Terminal), 분기 접합부, 스플라이스, 그로밋, 클립(Clip) 및 기타 관리 대상 형상은 정의된 데이텀(Datum)을 기준으로 배치한다. 이러한 기준은 치수 검증을 가능하게 하고 긴 하니스 경로에서 누적 오차를 감소시킨다. 커넥터 체결, 장착 클립, 관통부 및 정비 인터페이스는 설치 공차가 제한적인 경우가 많으므로 유연한 중간 구간보다 중요한 인터페이스 지점에 더욱 엄격한 위치 관리가 필요하다.

치구(Fixture)와 배선 가이드(Routing Aid)는 조립 과정에서 하니스 형상을 물리적으로 유지한다. 핀(Pin), 포스트(Post), 포크(Fork), 커넥터 홀더(Connector Holder), 클램프 및 전용 네스트(Nest)를 사용하여 메인 트렁크(Main Trunk)와 분기를 안내하고 불필요한 움직임을 방지할 수 있다. 반복 가능한 제조가 가능하도록 충분히 구속하면서도 비현실적인 장력이나 급격한 굽힘이 발생하지 않아야 한다. 또한 절연체, 터미널, 커넥터, 슬리브(Sleeve) 등의 보호 부품을 손상시키지 않고 효율적으로 하니스를 설치하고 분리할 수 있어야 한다.

커넥터 홀더(Connector Holder)는 커넥터 방향이 분기 방향과 이후 설치 상태에 영향을 주기 때문에 특히 중요하다. 커넥터가 올바른 위치에 있더라도 잘못된 방향으로 회전되어 있으면 실제 제품에 설치할 때 와이어 비틀림이나 부적절한 분기 형상이 발생할 수 있다. 따라서 보드는 커넥터 위치와 필요한 경우 방향까지 관리해야 한다. 또한 와이어 삽입, 2차 잠금장치(Secondary Lock) 조작, 검사, 라벨링(Labeling) 및 기타 조립 작업을 수행할 수 있도록 커넥터 주변에 충분한 작업 공간이 필요하다.

분기점(Branch Point)은 메인 하니스 트렁크가 여러 개의 작은 배선 경로로 나뉘는 위치를 정의한다. 분기 위치와 분기 각도(Breakout Angle)는 치수 정확성과 실제 설치 상태의 기계적 응력 모두에 영향을 준다. 보드 레이아웃은 지정된 분기 길이를 유지하면서 와이어 번들(Wire Bundle)이 자연스럽게 방향을 변경할 수 있도록 충분한 전이 거리(Transition Distance)를 제공해야 한다. 지나치게 급격한 분기 형상은 과도한 굽힘, 국부 압축, 테이프 집중 또는 스플라이스와 커넥터 출구 주변의 변형을 유발할 수 있다.

스플라이스 위치(Splice Location)는 여러 와이어가 비교적 강성이 높은 하나의 국부 구조로 결합될 수 있으므로 의도적으로 배치해야 한다. 보드에는 스플라이스와 관련 절연재, 실링(Sealing), 열수축재(Heat-Shrink Material), 보호재 등을 설치할 충분한 공간을 제공하면서 분기점, 커넥터 및 반복 굽힘 영역(High-Flex Region)으로부터 의도된 거리를 유지해야 한다. 일관된 스플라이스 위치는 후속 검사 반복성을 향상시키며 강성이 높은 구간이 기계적으로 불리한 설치 위치에 형성되는 것을 방지하는 데 도움이 된다.

하니스 치수는 관리 대상 인터페이스 치수(Controlled Interface Dimension)와 유연한 배선 치수(Flexible Routing Dimension)를 구분해야 한다. 모든 구간에 동일한 공차가 필요한 것은 아니다. 고정된 커넥터, 장착 클립, 그로밋 또는 기타 설치 인터페이스 사이의 치수는 기능적으로 중요할 수 있지만 중간 번들 경로는 상대적으로 더 큰 편차를 허용할 수 있다. 따라서 적절한 보드는 모든 하니스 구간을 과도하게 구속하기보다 설치, 전기 연결, 정비성 또는 기계적 내구성에 영향을 미치는 위치를 중심으로 치수를 관리한다.

와이어 및 번들의 여유 길이(Slack)는 의도적으로 관리해야 한다. 길이가 부족하면 조립 또는 설치 과정에서 인장 하중(Tensile Load)이 발생할 수 있고, 길이가 지나치게 길면 루프(Loop), 간섭, 마모 또는 불균일한 패키징(Packaging)이 발생할 수 있다. 보드는 공칭 길이(Nominal Length)와 필요한 제조 또는 설치 여유량 사이의 관계를 설정해야 한다. 이는 움직이는 기구, 서비스 루프(Service Loop), 커넥터 인터페이스 및 공차 누적으로 예상하지 못한 장력이 발생할 수 있는 부품 주변에서 특히 중요하다.

보호재(Protective Covering)는 브레이드 슬리브(Braid Sleeve), 테이프 래핑(Tape Wrapping), 주름관(Corrugated Conduit), 그로밋 및 기타 보호 부품의 설치 공간과 명확한 시작·종료 위치가 필요하기 때문에 보드 레이아웃에 영향을 준다. 따라서 선행 단계의 패키징 및 보호 설계(Packaging and Protection Design)는 하니스 보드에서 제조 정보로 구현된다. 특히 보호 경계가 마모, 온도, 진동 또는 환경 노출 영역과 연계되는 경우 작업자가 주관적으로 판단하지 않고 보호재의 시작, 중첩, 종료 및 전환 위치를 확인할 수 있어야 한다.

조립 순서(Assembly Sequence)는 치구 배치에 반영되어야 한다. 초기 단계에 설치되는 부품은 이후 추가 와이어와 분기가 배치된 후에도 필요한 접근성이 확보되어야 하며, 후속 공정인 테이핑(Taping), 슬리브 설치, 커넥터 완성, 라벨링 및 클립 장착에도 충분한 작업 공간이 필요하다. 치수상 정확한 보드라도 치구가 정상적인 조립 순서를 방해한다면 생산 효율성이 떨어질 수 있다. 따라서 레이아웃 엔지니어링(Layout Engineering)은 치수 관리뿐 아니라 제조 인체공학(Manufacturing Ergonomics)과 공정 흐름(Process Flow)을 함께 고려해야 한다.

시각적 관리(Visual Management)는 작업자가 의도된 구성을 즉시 파악하도록 하여 조립 오류를 감소시킬 수 있다. 커넥터 위치, 분기 경로, 스플라이스 위치, 부품 참조 정보, 보호 경계 및 검사 지점을 명확하게 표시하면 유사한 형상을 쉽게 구별할 수 있다. 보드는 해당 작업 지침(Work Instruction)을 지원해야 하며 작업 지침을 대신하는 비관리 문서가 되어서는 안 된다. 생산 정보는 승인된 도면, 자재 명세서(Bill of Material), 공정 사양 및 개정 관리(Revision Control)가 이루어지는 제조 문서와 일치해야 한다.

오류 방지(Error Prevention)는 포카요케(Poka-Yoke) 원리를 이용하여 물리적인 보드 레이아웃에 적용할 수 있다. 커넥터 네스트는 잘못된 방향으로 장착되는 것을 방지할 수 있고, 치구 형상은 서로 유사한 분기를 구별할 수 있으며, 전용 장착 위치를 통해 클립이나 부품의 누락을 방지할 수 있다. 이러한 기능은 반복되는 커넥터, 대칭적인 분기 또는 서로 유사한 와이어 그룹을 포함하는 하니스에서 특히 효과적이다. 목적은 올바른 조립은 단순하고 효율적으로 유지하면서 잘못된 조립은 어렵게 만드는 것이다.

보드 설계는 검사(Inspection)도 고려해야 한다. 중요 치수를 측정할 수 있어야 하고, 필요한 경우 커넥터 및 터미널 상태를 확인할 수 있어야 하며, 검사자가 부품 존재 여부, 분기 방향, 보호재 위치, 라벨, 클립 및 기타 관리 항목을 검증할 수 있어야 한다. 특히 래핑이나 보호재가 내부 와이어와 스플라이스를 가리기 전에 검사 접근성을 확보하는 것이 중요하다. 따라서 중간 검사 지점(Intermediate Inspection Point)을 최종 검사에만 의존하지 않고 조립 순서 자체에 포함할 수 있다.

하니스 보드는 물리적인 제조 정보(Physical Manufacturing Information)를 나타내므로 변경 관리(Change Control)가 필수적이다. 커넥터, 분기 길이, 스플라이스 위치, 보호재, 클립 또는 배선 인터페이스가 설계 변경되면 이에 따라 치구도 수정해야 할 수 있다. 보드 식별 정보, 개정 상태(Revision Status), 치구 교정 또는 검증 기록, 승인된 제조 문서는 서로 동기화되어야 하며, 엔지니어링 정의가 변경된 이후에도 구형 레이아웃을 이용하여 하니스가 계속 생산되는 것을 방지해야 한다.

로보틱스(Robotics) 및 자율이동로봇(AMR, Autonomous Mobile Robot)에서는 하니스 보드의 정확성이 제한된 공간과 기계적 움직임이 존재하는 시스템에 하니스를 설치하는 데 직접적으로 기여한다. 하니스는 배터리, 모터 컨트롤러(Motor Controller), 센서, 컴퓨팅 장치, 통신 네트워크, 충전 인터페이스 및 움직이는 구동 모듈(Drive Module)을 연결할 수 있다. 관리된 보드 레이아웃은 제조된 하니스가 이러한 인터페이스에 반복적으로 정확하게 장착되면서 설계 단계에서 설정한 배선, 여유 길이, 보호 및 기계적 관계를 유지하도록 한다.

하니스 보드 조립(Harness Board Assembly)은 궁극적으로 상류 공정의 자동 절단-탈피-압착(Automatic Cut-Strip-Crimp)과 압착 품질 검증(Crimp Quality Verification)을 하류 공정의 표준 작업(Standardized Work) 및 초도품 검사(First Article Inspection)와 연결한다. 정확하게 제작된 터미널 체결 리드(Terminated Lead)라도 공간적 관계가 잘못 조립되면 올바른 하니스를 보장할 수 없다. 하니스 보드는 개별 부품을 관리된 하나의 제품으로 통합하는 제조 형상을 제공하며, 와이어 준비, 조립 공정 관리, 검사 및 신뢰성 높은 최종 하니스 생산을 연결하는 핵심 역할을 수행한다.

##  

## 10.04. Work Instruction Standard

![](images/image4.png){width="7.268055555555556in" height="7.268055555555556in"}

A work instruction standard defines the controlled manufacturing information required for operators to assemble a wire harness consistently, safely, and according to the released engineering definition. Within the manufacturing process, it translates drawings, bills of material, harness-board layouts, process specifications, and quality requirements into practical production steps. It provides a common reference so that assembly results depend on an approved process rather than individual operator interpretation.

A work instruction should identify the product, harness part number, applicable revision, manufacturing operation, required materials, tools, fixtures, and inspection requirements. This information establishes exactly which configuration is being manufactured. Clear document identification is especially important when visually similar harness variants exist because an operator may otherwise assemble the correct components according to an obsolete or incorrect product configuration.

The instruction must correspond to the current released engineering data. Wire types, connector part numbers, terminals, seals, splices, sleeves, tapes, conduits, clips, labels, and other components referenced during assembly should remain consistent with the approved bill of material and drawings. When engineering changes occur, the work instruction must be reviewed and updated so that manufacturing documentation does not continue directing production according to superseded design information.

Manufacturing steps should follow the actual assembly sequence. The instruction may begin with prepared leads from the automatic cut-strip-crimp process and proceed through harness-board loading, branch formation, splice integration, connector insertion, protection installation, taping, clipping, labeling, inspection, and final removal. Presenting operations in their intended sequence reduces unnecessary handling and prevents later operations from obstructing components that should have been installed or inspected earlier.

Each operation should describe what must be performed and the conditions necessary for acceptable execution. Instructions should define relevant positions, dimensions, orientations, tool settings, material application boundaries, or other controlled parameters rather than relying on vague expressions such as "assemble correctly." The level of detail should be sufficient for trained operators to reproduce the process while avoiding unnecessary information that obscures critical manufacturing requirements.

Visual references can support work instructions when complex connector orientations, branch directions, routing paths, protection boundaries, or component locations are difficult to communicate using text alone. However, visual information should remain consistent with the released configuration and revision. A photograph or illustration that clearly shows an obsolete connector, clip position, or routing direction can create manufacturing errors even when the accompanying written instruction has been updated.

Harness-board information and work instructions perform complementary functions. The board physically establishes connector positions, branches, dimensions, splice locations, and routing geometry, while the work instruction explains the sequence and method used to build the harness on that board. Operators should not be required to infer assembly requirements solely from fixture positions. Likewise, written instructions cannot compensate for a board whose physical configuration does not match the released harness geometry.

Critical process parameters should be clearly distinguishable from general explanatory information. These parameters can include specified dimensions, component orientation, insertion condition, tape overlap, sleeve start and stop positions, tightening requirements, tool settings, or inspection criteria. Highlighting process-critical information helps operators recognize characteristics that directly influence electrical performance, mechanical durability, packaging, installation, or subsequent quality acceptance.

Connector assembly requires particularly clear instructions because terminals, seals, cavity positions, secondary locks, and connector orientation can create hidden errors. The instruction should provide sufficient information to place each circuit into its intended location and confirm completion of the required locking condition. When connectors contain similar cavities or repeated wire colors, manufacturing controls should reduce dependence on memory and prevent incorrect circuit insertion or incomplete terminal engagement.

Protection installation also requires controlled instructions. Tape wrapping, braid sleeves, corrugated conduit, heat-shrink material, grommets, and other protective elements should be applied according to defined locations and process requirements. Start and stop positions, overlap regions, transitions, and interface conditions may influence abrasion resistance, flexibility, sealing, thermal protection, or packaging. The work instruction translates these engineering requirements into repeatable shop-floor operations.

Quality checkpoints should be positioned where defects can be detected before subsequent operations conceal them. For example, wire routing, splice condition, connector insertion, or component presence may be easier to verify before tape or sleeve covers the assembly. Integrating intermediate inspection into the work sequence reduces the need for destructive rework and improves defect containment. Final inspection then verifies characteristics that remain applicable to the completed harness.

Acceptance criteria must be sufficiently objective that different trained operators or inspectors reach consistent conclusions. Where dimensional limits, visual conditions, or process requirements are defined by another controlled specification, the work instruction should reference the appropriate requirement rather than creating an independent conflicting criterion. This approach maintains a clear relationship between engineering requirements, manufacturing execution, and quality verification.

Tools and equipment referenced by the instruction must correspond to the intended manufacturing process. Where special applicators, torque tools, insertion tools, fixtures, test equipment, or inspection devices are required, their identification and applicable settings should be controlled. Using the correct component with an incorrect tool can still create an unacceptable harness, making tooling configuration part of the manufacturing definition rather than merely an operator preference.

Error-proofing, or poka-yoke, should be incorporated wherever practical. Instructions can reinforce physical error-prevention features by showing correct connector orientation, distinguishing similar branches, identifying mandatory clips, or defining verification steps before irreversible operations. Effective error prevention combines clear documentation with fixture design, component identification, tool control, and process sequencing so that incorrect assembly becomes difficult to perform or easy to detect.

Revision control is fundamental to the work instruction standard. Every production location should use the currently released revision, while obsolete versions must be removed from active use or clearly prevented from being selected. Revision history should allow manufacturing personnel to understand when relevant process information changed. Synchronization among engineering drawings, bills of material, harness boards, work instructions, inspection documents, and production systems prevents configuration mismatch.

Operator training is connected to work instructions but should not be treated as a substitute for them. Training develops the skills required to perform crimp-related handling, connector assembly, routing, wrapping, inspection, and other manufacturing operations, while the instruction defines the specific process for the product being manufactured. A robust system therefore combines qualified personnel with controlled documentation instead of relying on undocumented experience or individual memory.

Traceability can link execution of the work instruction to the manufactured harness. Depending on production requirements, records may identify the product serial or lot, instruction revision, operator, workstation, date, equipment, inspection results, and relevant process status. When a defect is later discovered, these records help determine which manufacturing definition was used and whether other harnesses produced under the same conditions may require investigation.

Work instructions should also support continuous manufacturing improvement without allowing uncontrolled process changes. Repeated assembly difficulty, excessive rework, ambiguous steps, ergonomic problems, or recurring defects can indicate that the instruction, fixture, product design, or process requires improvement. Proposed changes should be reviewed and released through the established change-control process so that improvements become standardized rather than remaining informal operator practices.

For robotics and AMR harnesses, standardized work is particularly important because compact packaging can combine power, motor, sensor, communication, computing, charging, and moving-module circuits within one assembly. Incorrect routing or component placement can affect mechanical clearance, serviceability, electromagnetic behavior, or durability. Clear work instructions help preserve the relationships established by electrical architecture, routing engineering, packaging design, and harness-board layout during physical production.

The work instruction standard therefore connects upstream automatic cut-strip-crimp processing, crimp quality verification, and harness-board layout with downstream first article inspection. Each stage controls a different aspect of manufacturing: prepared lead quality, terminal integrity, assembly geometry, standardized execution, and final verification. Together they create a controlled manufacturing chain in which engineering intent can be repeatedly transformed into reliable wire harnesses for robotics and other electrical systems.

작업 지침 표준(Work Instruction Standard)은 작업자가 와이어 하니스(Wire Harness)를 일관되고 안전하게, 그리고 승인된 엔지니어링 정의(Released Engineering Definition)에 따라 조립하기 위해 필요한 관리된 제조 정보(Controlled Manufacturing Information)를 정의한다. 제조 공정에서는 도면, 자재 명세서(Bill of Material), 하니스 보드 레이아웃(Harness Board Layout), 공정 사양(Process Specification), 품질 요구사항을 실제 생산 단계로 변환한다. 이를 통해 조립 결과가 작업자의 개인적인 판단이 아니라 승인된 공정에 따라 결정되도록 공통 기준을 제공한다.

작업 지침(Work Instruction)에는 제품, 하니스 부품 번호, 적용 개정판(Revision), 제조 작업, 필요한 재료, 공구, 치구(Fixture), 검사 요구사항을 명확하게 식별해야 한다. 이러한 정보는 정확히 어떤 제품 구성을 제조하는지를 정의한다. 외관이 유사한 여러 하니스 변형 모델이 존재하는 경우에는 명확한 문서 식별이 특히 중요하며, 그렇지 않으면 작업자가 올바른 부품을 사용하면서도 구형 또는 잘못된 제품 구성에 따라 조립할 수 있다.

작업 지침은 현재 승인된 엔지니어링 데이터(Released Engineering Data)와 일치해야 한다. 조립 과정에서 참조하는 와이어 종류, 커넥터 부품 번호, 터미널(Terminal), 실(Seal), 스플라이스(Splice), 슬리브(Sleeve), 테이프, 주름관(Conduit), 클립(Clip), 라벨(Label) 및 기타 부품은 승인된 자재 명세서와 도면에 일치해야 한다. 엔지니어링 변경이 발생하면 작업 지침도 검토하고 개정하여 폐기된 설계 정보에 따라 생산이 계속 진행되는 것을 방지해야 한다.

제조 단계는 실제 조립 순서(Assembly Sequence)를 따라야 한다. 작업 지침은 자동 절단-탈피-압착(Automatic Cut-Strip-Crimp) 공정에서 준비된 리드(Lead)부터 시작하여 하니스 보드 장착, 분기 형성, 스플라이스 통합, 커넥터 삽입, 보호재 설치, 테이핑(Taping), 클립 장착, 라벨링(Labeling), 검사 및 최종 분리 순서로 진행할 수 있다. 작업을 의도된 순서로 제시하면 불필요한 취급을 줄이고 이후 공정 때문에 먼저 설치하거나 검사해야 할 부품에 접근하지 못하는 문제를 방지할 수 있다.

각 작업은 수행해야 하는 내용과 적합한 작업 수행에 필요한 조건을 설명해야 한다. 작업 지침에서는 단순히 "올바르게 조립한다"와 같은 모호한 표현에 의존하지 않고 관련 위치, 치수, 방향, 공구 설정, 재료 적용 경계 또는 기타 관리 파라미터(Controlled Parameter)를 정의해야 한다. 세부 수준은 숙련된 작업자가 공정을 반복적으로 재현할 수 있을 만큼 충분해야 하지만, 중요한 제조 요구사항을 가릴 정도로 불필요한 정보가 포함되어서는 안 된다.

복잡한 커넥터 방향, 분기 방향, 배선 경로, 보호 경계 또는 부품 위치를 텍스트만으로 전달하기 어려운 경우 시각적 참조 자료(Visual Reference)를 작업 지침에 활용할 수 있다. 그러나 시각 정보 역시 승인된 제품 구성 및 개정판과 일치해야 한다. 사진이나 그림에 구형 커넥터, 잘못된 클립 위치 또는 이전 배선 방향이 표시되어 있다면 함께 제공되는 문서가 최신 상태이더라도 제조 오류를 발생시킬 수 있다.

하니스 보드 정보(Harness Board Information)와 작업 지침은 서로 보완적인 기능을 수행한다. 하니스 보드는 커넥터 위치, 분기, 치수, 스플라이스 위치 및 배선 형상을 물리적으로 설정하며, 작업 지침은 해당 보드에서 하니스를 제작하는 순서와 방법을 설명한다. 작업자가 치구 위치만을 보고 조립 요구사항을 추정하도록 해서는 안 된다. 마찬가지로 물리적 구성이 승인된 하니스 형상과 일치하지 않는 보드를 문서화된 작업 지침만으로 보완할 수도 없다.

중요 공정 파라미터(Critical Process Parameter)는 일반적인 설명 정보와 명확하게 구분되어야 한다. 여기에는 지정 치수, 부품 방향, 삽입 상태, 테이프 중첩량, 슬리브 시작 및 종료 위치, 체결 요구사항, 공구 설정 또는 검사 기준 등이 포함될 수 있다. 공정에 중요한 정보를 명확하게 표시하면 작업자가 전기적 성능, 기계적 내구성, 패키징(Packaging), 설치 또는 후속 품질 판정에 직접적인 영향을 미치는 특성을 쉽게 인식할 수 있다.

커넥터 조립(Connector Assembly)은 터미널, 실, 캐비티 위치(Cavity Position), 2차 잠금장치(Secondary Lock), 커넥터 방향과 관련하여 외부에서 쉽게 확인하기 어려운 오류가 발생할 수 있으므로 특히 명확한 지침이 필요하다. 작업 지침은 각 회로(Circuit)를 지정된 위치에 삽입하고 필요한 잠금 상태가 완성되었는지 확인할 수 있는 충분한 정보를 제공해야 한다. 유사한 캐비티나 반복되는 와이어 색상이 존재하는 경우 제조 관리 방법을 통해 작업자의 기억에 대한 의존성을 줄이고 잘못된 회로 삽입이나 불완전한 터미널 체결을 방지해야 한다.

보호재 설치(Protection Installation) 역시 관리된 작업 지침을 필요로 한다. 테이프 래핑(Tape Wrapping), 브레이드 슬리브(Braid Sleeve), 주름관(Corrugated Conduit), 열수축재(Heat-Shrink Material), 그로밋(Grommet) 및 기타 보호 요소는 정의된 위치와 공정 요구사항에 따라 적용해야 한다. 시작 및 종료 위치, 중첩 영역, 전환부 및 인터페이스 조건은 내마모성, 유연성, 실링(Sealing), 열 보호 또는 패키징에 영향을 줄 수 있다. 작업 지침은 이러한 엔지니어링 요구사항을 반복 가능한 생산 현장 작업으로 변환한다.

품질 확인 지점(Quality Checkpoint)은 후속 작업으로 결함이 가려지기 전에 검출할 수 있는 위치에 설정해야 한다. 예를 들어 와이어 배선, 스플라이스 상태, 커넥터 삽입 또는 부품 존재 여부는 테이프나 슬리브로 조립체를 덮기 전에 확인하는 것이 더 용이할 수 있다. 중간 검사(Intermediate Inspection)를 작업 순서에 통합하면 파괴적인 재작업(Destructive Rework)의 필요성을 줄이고 결함의 확산을 억제할 수 있다. 최종 검사에서는 완성된 하니스에 적용되는 특성을 다시 검증한다.

합격 기준(Acceptance Criteria)은 서로 다른 숙련 작업자나 검사자가 일관된 판단을 내릴 수 있을 정도로 객관적이어야 한다. 치수 한계, 외관 상태 또는 공정 요구사항이 다른 관리 사양(Controlled Specification)에 정의되어 있다면 작업 지침에서 별도의 상충되는 기준을 새로 만들기보다 해당 요구사항을 참조해야 한다. 이러한 방법을 통해 엔지니어링 요구사항, 제조 실행(Manufacturing Execution), 품질 검증(Quality Verification) 사이의 명확한 관계를 유지할 수 있다.

작업 지침에 지정된 공구와 장비는 의도된 제조 공정과 일치해야 한다. 특수 어플리케이터(Applicator), 토크 공구(Torque Tool), 삽입 공구(Insertion Tool), 치구, 시험 장비 또는 검사 장치가 필요한 경우 해당 장비의 식별 정보와 적용 설정을 관리해야 한다. 올바른 부품을 사용하더라도 잘못된 공구를 적용하면 부적합한 하니스가 만들어질 수 있으므로 공구 구성(Tooling Configuration)도 작업자의 선택 사항이 아니라 제조 정의의 일부로 관리해야 한다.

오류 방지(Error-Proofing), 즉 포카요케(Poka-Yoke)는 가능한 영역에 적극적으로 적용해야 한다. 작업 지침은 올바른 커넥터 방향 표시, 유사한 분기의 구분, 필수 클립의 식별 또는 되돌릴 수 없는 작업 이전의 검증 단계 등을 통해 물리적인 오류 방지 기능을 강화할 수 있다. 효과적인 오류 방지는 명확한 문서와 함께 치구 설계, 부품 식별, 공구 관리 및 공정 순서를 결합하여 잘못된 조립은 수행하기 어렵게 만들거나 쉽게 검출할 수 있도록 한다.

개정 관리(Revision Control)는 작업 지침 표준의 핵심 요소이다. 모든 생산 위치에서는 현재 승인된 개정판을 사용해야 하며, 구형 버전은 실제 작업에서 제거하거나 선택할 수 없도록 명확하게 관리해야 한다. 개정 이력(Revision History)을 통해 제조 담당자가 관련 공정 정보가 언제 변경되었는지 파악할 수 있어야 한다. 엔지니어링 도면, 자재 명세서, 하니스 보드, 작업 지침, 검사 문서 및 생산 시스템을 서로 동기화함으로써 제품 구성 불일치(Configuration Mismatch)를 방지할 수 있다.

작업자 교육(Operator Training)은 작업 지침과 연계되어 있지만 이를 대체하는 수단으로 간주해서는 안 된다. 교육은 압착 관련 취급, 커넥터 조립, 배선, 래핑, 검사 및 기타 제조 작업을 수행하기 위한 기술을 개발하고, 작업 지침은 실제 생산되는 특정 제품에 적용되는 공정을 정의한다. 따라서 안정적인 제조 시스템은 문서화되지 않은 경험이나 개인적인 기억에 의존하는 대신 자격을 갖춘 작업자와 관리된 문서(Controlled Documentation)를 결합해야 한다.

추적성(Traceability)을 통해 작업 지침의 실행 기록과 실제 제조된 하니스를 연결할 수 있다. 생산 요구사항에 따라 제품 일련번호 또는 로트(Lot), 작업 지침 개정판, 작업자, 작업장(Workstation), 생산 날짜, 장비, 검사 결과 및 관련 공정 상태를 기록할 수 있다. 이후 결함이 발견되면 이러한 기록을 통해 어떤 제조 정의가 적용되었는지 확인하고 동일한 조건에서 생산된 다른 하니스도 조사가 필요한지 판단할 수 있다.

작업 지침은 관리되지 않은 공정 변경을 허용하지 않으면서 지속적인 제조 개선(Continuous Manufacturing Improvement)을 지원해야 한다. 반복적인 조립 어려움, 과도한 재작업, 모호한 작업 단계, 인체공학적 문제 또는 반복 결함은 작업 지침, 치구, 제품 설계 또는 공정 자체의 개선이 필요하다는 신호일 수 있다. 제안된 변경 사항은 정해진 변경 관리 프로세스(Change-Control Process)를 통해 검토하고 승인하여 개선 내용이 작업자의 비공식적인 방법으로 남지 않고 표준화되도록 해야 한다.

로보틱스(Robotics) 및 자율이동로봇(AMR, Autonomous Mobile Robot) 하니스에서는 제한된 패키징 공간 안에 전원, 모터, 센서, 통신, 컴퓨팅, 충전 및 움직이는 모듈의 회로가 하나의 조립체로 통합될 수 있으므로 표준 작업(Standardized Work)이 특히 중요하다. 잘못된 배선이나 부품 위치는 기계적 간극, 정비성(Serviceability), 전자기적 특성 또는 내구성에 영향을 줄 수 있다. 명확한 작업 지침은 전기 아키텍처, 배선 엔지니어링, 패키징 설계 및 하니스 보드 레이아웃에서 설정된 관계가 실제 생산에서도 유지되도록 한다.

따라서 작업 지침 표준(Work Instruction Standard)은 상류의 자동 절단-탈피-압착(Automatic Cut-Strip-Crimp), 압착 품질 검증(Crimp Quality Verification), 하니스 보드 레이아웃(Harness Board Layout)을 하류의 초도품 검사(First Article Inspection)와 연결한다. 각 단계는 준비된 리드 품질, 터미널 건전성, 조립 형상, 표준화된 작업 실행 및 최종 검증이라는 서로 다른 제조 요소를 관리한다. 이들이 결합됨으로써 엔지니어링 의도를 로보틱스 및 기타 전기 시스템에 사용되는 신뢰성 높은 와이어 하니스로 반복적으로 구현할 수 있는 관리된 제조 체계(Controlled Manufacturing Chain)가 형성된다.

##  

## 10.05. First Article Inspection

![](images/image5.png){width="7.268055555555556in" height="7.268055555555556in"}

First Article Inspection is a structured verification activity used to confirm that the first representative wire harness produced from a defined manufacturing configuration satisfies the released engineering and manufacturing requirements. It provides objective evidence that materials, tooling, harness-board geometry, work instructions, assembly processes, and inspection methods collectively produce an acceptable product before routine production proceeds.

The first article should represent the intended production process rather than a specially prepared engineering sample. It should be manufactured using the released wire, terminals, connectors, seals, splices, protective materials, clips, labels, tools, fixtures, harness board, and approved work instruction. This principle is important because inspection results are meaningful only when the inspected harness reflects the same conditions expected during normal manufacturing.

First Article Inspection begins with configuration verification. The harness part number, drawing revision, bill of material, work instruction revision, harness-board revision, applicable process specifications, and inspection criteria should correspond to the same released product definition. A dimensional or functional inspection cannot establish manufacturing conformity when the product has been built using mismatched revisions or obsolete documentation.

Material verification confirms that the components incorporated into the harness correspond to the released bill of material. Wire type and gauge, insulation characteristics, terminals, connectors, cavity seals, splice components, sleeves, conduit, tape, grommets, clips, labels, and other specified materials should be checked as applicable. Material identification and lot information may also be recorded when traceability requirements apply to critical components or production batches.

Prepared lead quality provides an important upstream input to the first article. Wire length, strip length, terminal selection, conductor crimp, insulation crimp, and other characteristics generated during automatic cut-strip-crimp processing should already satisfy their applicable process requirements. First Article Inspection verifies that these prepared components remain correct when integrated into the complete harness rather than treating final assembly as a substitute for proper control of earlier manufacturing processes.

Crimp-related verification may include external terminal condition, conductor position, insulation position, bellmouth formation, crimp dimensions, pull-test evidence, or cross-sectional inspection according to the applicable quality plan. Cross-section analysis is particularly useful when validating a new terminal-wire-tooling combination or confirming a significant process change. The objective is to demonstrate that terminal connections provide the intended mechanical and electrical structure before production quantities increase.

Harness geometry is evaluated against the released dimensional definition and the physical relationships established by the harness board. Critical dimensions can include distances between connectors, branch points, splices, clips, grommets, and other installation interfaces. Branch lengths and breakout directions should also correspond to the intended configuration. Dimensional verification should concentrate on characteristics that influence installation, packaging, mating, serviceability, or mechanical loading.

Connector inspection verifies both component identity and assembly condition. Correct connector type, orientation, cavity assignment, terminal insertion, seal installation, and secondary locking features should be checked where applicable. Particular attention is required when connectors contain repeated cavity patterns, similar wire colors, or visually similar terminal systems because an apparently complete connector can still contain hidden circuit-placement or locking errors.

Splices and branch structures should be examined for correct location, circuit composition, insulation, protection, and integration into the surrounding harness. Their position relative to connectors, branch points, and flex regions can affect both packaging and durability. Where a splice becomes hidden by tape, sleeve, or conduit, the inspection process should include verification before covering so that internal assembly conditions do not become inaccessible during final inspection.

Protective components are inspected for correct type, location, coverage, and installation condition. Tape wrapping, braid sleeves, corrugated conduit, heat-shrink material, grommets, abrasion protection, and similar features should begin and terminate at the intended positions. Incorrect protection boundaries can expose wires to abrasion, heat, vibration, contamination, or excessive bending even when the electrical connectivity of the harness is otherwise correct.

Clips, clamps, retainers, and mounting features should be verified because they determine how the harness interfaces mechanically with the final product. Their quantity, location, orientation, and attachment condition influence routing accuracy and load transfer after installation. A missing or incorrectly positioned clip can cause interference, excessive movement, connector loading, or abrasion even though the harness passes electrical continuity testing.

Visual inspection evaluates workmanship characteristics that may not be adequately represented by dimensional measurements alone. Inspectors can examine damaged insulation, exposed conductor, distorted terminals, loose protection, sharp bends, twisted branches, incorrect labels, contamination, or other abnormal conditions. Visual acceptance criteria should be defined sufficiently clearly that inspection does not depend solely on individual preference or undocumented workmanship expectations.

Electrical testing verifies that the assembled harness implements the intended circuit connectivity. Continuity testing can confirm that each circuit connects the correct endpoints, while short-circuit or miswire detection can identify unintended connections between circuits. Depending on the product and applicable requirements, additional tests may evaluate insulation resistance or other electrical characteristics. Electrical testing complements physical inspection because correct appearance does not guarantee correct circuit assignment.

The work instruction itself becomes part of First Article Inspection because the objective is to validate the manufacturing process as well as the resulting product. Inspectors should confirm that the released sequence, specified tools, fixture arrangement, controlled parameters, intermediate checkpoints, and acceptance requirements are practical and sufficient. Difficult or ambiguous operations discovered during first-article production may indicate that manufacturing documentation requires correction before routine production.

Inspection results should distinguish objective measurements from acceptance decisions. Measured dimensions, test results, component verification, observations, and nonconformities should be recorded against their applicable requirements. A characteristic should not be accepted simply because the deviation appears small or because the harness can still be installed. Deviations from released requirements should follow the established engineering or quality disposition process rather than informal production judgment.

Nonconformities identified during First Article Inspection provide valuable information about the manufacturing system. A dimensional error may originate from wire preparation, board layout, fixture position, or assembly technique, while an incorrect connector circuit may indicate documentation, labeling, or process-sequencing problems. Root-cause investigation should therefore consider the complete manufacturing chain rather than correcting only the visible defect on the inspected harness.

Corrective action should address the source of the problem and then verify that the modified process produces conforming results. Depending on the issue, this may require changes to tooling, harness-board fixtures, work instructions, material controls, inspection criteria, operator training, or engineering documentation. The affected characteristics should be reinspected after correction so that production release is supported by evidence rather than by assumption that the corrective action was effective.

Traceability provides the historical record of the first article and its manufacturing conditions. Records may include product identification, revision status, wire and terminal lots, equipment and applicator identification, harness-board identification, operator information, inspection equipment, measured results, electrical test records, nonconformities, corrective actions, approvals, and production date. These records provide a baseline for later investigation and comparison with subsequent production.

First Article Inspection may also be required again when significant changes invalidate the assumptions established by the original inspection. Changes to product design, wire or terminal configuration, tooling, manufacturing location, harness board, critical process parameters, or other controlled production conditions can require partial or complete revalidation according to the applicable quality system. The scope should correspond to the characteristics potentially affected by the change.

For robotics and AMR harnesses, first-article verification is particularly valuable because a single harness may integrate battery power, motor control, sensors, communication networks, computing equipment, charging interfaces, and moving modules. Dimensional, electrical, and workmanship errors can therefore affect multiple subsystems. Verification before repetitive production reduces the probability that a systematic manufacturing error will be reproduced across multiple robots or assemblies.

First Article Inspection completes the manufacturing chain established within the manufacturing and process chapter: automatic cut-strip-crimp creates controlled terminated leads, crimp cross-section analysis verifies terminal integrity, harness-board layout establishes assembly geometry, and standardized work instructions define repeatable execution. First Article Inspection then verifies that these controls operate together successfully, providing the evidence required to release a reliable wire harness into normal production.

초도품 검사(First Article Inspection)는 정의된 제조 구성(Manufacturing Configuration)에 따라 처음 생산된 대표 와이어 하니스(Wire Harness)가 승인된 엔지니어링 및 제조 요구사항을 만족하는지 확인하기 위한 체계적인 검증 활동이다. 재료, 금형(Tooling), 하니스 보드 형상(Harness-Board Geometry), 작업 지침(Work Instruction), 조립 공정 및 검사 방법이 함께 작동하여 정상적인 제품을 생산한다는 객관적인 근거를 제공하며, 이를 확인한 후 정상 양산(Routine Production)을 진행한다.

초도품(First Article)은 특별히 준비된 엔지니어링 시제품이 아니라 실제 적용할 생산 공정을 대표해야 한다. 승인된 와이어, 터미널(Terminal), 커넥터(Connector), 실(Seal), 스플라이스(Splice), 보호재, 클립(Clip), 라벨(Label), 공구, 치구(Fixture), 하니스 보드 및 승인된 작업 지침을 사용하여 제조해야 한다. 검사 대상 하니스가 실제 양산에서 예상되는 조건과 동일한 경우에만 검사 결과가 제조 공정을 대표하는 의미 있는 결과가 된다.

초도품 검사는 구성 검증(Configuration Verification)에서 시작한다. 하니스 부품 번호, 도면 개정판(Drawing Revision), 자재 명세서(Bill of Material), 작업 지침 개정판, 하니스 보드 개정판, 적용 공정 사양(Process Specification) 및 검사 기준이 동일하게 승인된 제품 정의와 일치해야 한다. 서로 다른 개정판이나 폐기된 문서를 이용하여 제품을 제조했다면 치수 검사나 기능 검사가 정상이어도 제조 적합성(Manufacturing Conformity)을 입증할 수 없다.

재료 검증(Material Verification)은 하니스에 사용된 부품이 승인된 자재 명세서와 일치하는지를 확인한다. 와이어 종류와 규격, 절연 특성, 터미널, 커넥터, 캐비티 실(Cavity Seal), 스플라이스 부품, 슬리브(Sleeve), 주름관(Conduit), 테이프, 그로밋(Grommet), 클립, 라벨 및 기타 지정된 재료를 필요에 따라 확인해야 한다. 중요 부품 또는 생산 배치에 추적성 요구사항이 적용되는 경우에는 재료 식별 정보와 로트(Lot) 정보도 기록할 수 있다.

준비된 리드 품질(Prepared Lead Quality)은 초도품 검사에 중요한 상류 공정 입력을 제공한다. 자동 절단-탈피-압착(Automatic Cut-Strip-Crimp) 공정에서 생성된 와이어 길이, 탈피 길이(Strip Length), 터미널 선택, 도체 압착(Conductor Crimp), 절연 압착(Insulation Crimp) 및 기타 특성은 이미 해당 공정 요구사항을 만족해야 한다. 초도품 검사는 최종 조립을 선행 제조 공정 관리의 대체 수단으로 사용하는 것이 아니라, 이러한 준비 부품이 전체 하니스에 통합된 이후에도 올바른 상태를 유지하는지를 확인한다.

압착 관련 검증(Crimp-Related Verification)에는 적용되는 품질 계획에 따라 터미널 외관 상태, 도체 위치, 절연체 위치, 벨마우스(Bellmouth) 형성, 압착 치수, 인장 시험(Pull Test) 결과 또는 단면 검사(Cross-Section Inspection)가 포함될 수 있다. 단면 분석은 새로운 터미널-와이어-금형 조합을 검증하거나 중요한 공정 변경을 확인할 때 특히 유용하다. 목적은 생산 수량을 증가시키기 전에 터미널 연결부가 의도된 기계적·전기적 구조를 제공하는지 입증하는 것이다.

하니스 형상(Harness Geometry)은 승인된 치수 정의와 하니스 보드에서 설정된 물리적 관계를 기준으로 평가한다. 중요 치수에는 커넥터, 분기점(Branch Point), 스플라이스, 클립, 그로밋 및 기타 설치 인터페이스 사이의 거리가 포함될 수 있다. 분기 길이와 분기 방향(Breakout Direction)도 의도된 구성과 일치해야 한다. 치수 검증은 설치, 패키징(Packaging), 체결, 정비성(Serviceability) 또는 기계적 하중에 영향을 주는 특성을 중심으로 수행해야 한다.

커넥터 검사(Connector Inspection)는 부품 식별 정보와 조립 상태를 모두 검증한다. 올바른 커넥터 종류, 방향, 캐비티 할당(Cavity Assignment), 터미널 삽입, 실 설치 및 2차 잠금 기능(Secondary Locking Feature)을 필요한 경우 확인해야 한다. 반복되는 캐비티 패턴, 유사한 와이어 색상 또는 외관이 비슷한 터미널 시스템이 포함된 커넥터는 외관상 완성되어 보여도 내부에 회로 배치 오류나 잠금 불량이 존재할 수 있으므로 특별한 주의가 필요하다.

스플라이스 및 분기 구조(Branch Structure)는 정확한 위치, 회로 구성, 절연, 보호 상태 및 주변 하니스와의 통합 상태를 검사해야 한다. 커넥터, 분기점 및 반복 굽힘 영역(Flex Region)에 대한 상대적인 위치는 패키징과 내구성 모두에 영향을 줄 수 있다. 스플라이스가 테이프, 슬리브 또는 주름관으로 가려지는 경우에는 최종 검사에서 내부 조립 상태를 확인할 수 없으므로 보호재를 적용하기 전에 검증하는 검사 과정이 포함되어야 한다.

보호 부품(Protective Component)은 올바른 종류, 위치, 적용 범위 및 설치 상태를 검사한다. 테이프 래핑(Tape Wrapping), 브레이드 슬리브(Braid Sleeve), 주름관(Corrugated Conduit), 열수축재(Heat-Shrink Material), 그로밋, 마모 방지재(Abrasion Protection) 및 유사한 보호 요소가 의도된 위치에서 시작하고 종료되는지 확인해야 한다. 보호 경계가 잘못되면 하니스의 전기적 연결이 정상이어도 와이어가 마모, 열, 진동, 오염 또는 과도한 굽힘에 노출될 수 있다.

클립, 클램프(Clamp), 리테이너(Retainer) 및 장착 요소는 하니스가 최종 제품과 기계적으로 어떻게 결합되는지를 결정하므로 반드시 검증해야 한다. 이들의 수량, 위치, 방향 및 장착 상태는 설치 후 배선 정확성과 하중 전달에 영향을 준다. 클립이 누락되거나 잘못된 위치에 장착되면 하니스가 전기적 연속성 시험을 통과하더라도 간섭, 과도한 움직임, 커넥터 하중 또는 마모 문제가 발생할 수 있다.

육안 검사(Visual Inspection)는 치수 측정만으로 충분히 평가하기 어려운 작업 품질(Workmanship) 특성을 확인한다. 검사자는 손상된 절연체, 노출된 도체, 변형된 터미널, 느슨한 보호재, 급격한 굽힘, 비틀린 분기, 잘못된 라벨, 오염 또는 기타 비정상적인 상태를 확인할 수 있다. 육안 합격 기준(Visual Acceptance Criteria)은 검사자의 개인적인 선호나 문서화되지 않은 작업 품질 기준에 의존하지 않도록 충분히 명확하게 정의해야 한다.

전기 시험(Electrical Testing)은 조립된 하니스가 의도된 회로 연결성을 구현하고 있는지 검증한다. 연속성 시험(Continuity Testing)을 통해 각 회로가 올바른 양단을 연결하는지 확인할 수 있으며, 단락 또는 오배선 검출(Short-Circuit or Miswire Detection)을 통해 회로 사이의 의도하지 않은 연결을 식별할 수 있다. 제품과 적용 요구사항에 따라 절연 저항(Insulation Resistance) 등의 추가적인 전기 특성을 평가할 수도 있다. 올바른 외관만으로 정확한 회로 구성을 보장할 수 없기 때문에 전기 시험은 물리적 검사를 보완한다.

초도품 검사의 목적은 최종 제품뿐만 아니라 제조 공정 자체를 검증하는 것이므로 작업 지침도 검사 대상의 일부가 된다. 검사자는 승인된 작업 순서, 지정 공구, 치구 배치, 관리 파라미터(Controlled Parameter), 중간 검사 지점 및 합격 요구사항이 실제 생산에서 적용 가능하고 충분한지를 확인해야 한다. 초도품 생산 과정에서 어렵거나 모호한 작업이 발견되면 정상 양산을 시작하기 전에 제조 문서를 수정해야 할 필요성이 있음을 의미할 수 있다.

검사 결과에서는 객관적인 측정 결과(Objective Measurement)와 합격 판정(Acceptance Decision)을 구분해야 한다. 측정 치수, 시험 결과, 부품 검증 결과, 관찰 사항 및 부적합(Nonconformity)을 각각 적용되는 요구사항과 비교하여 기록해야 한다. 편차가 작아 보이거나 실제로 하니스를 설치할 수 있다는 이유만으로 해당 특성을 임의로 합격 처리해서는 안 된다. 승인된 요구사항에서 벗어난 사항은 생산 현장의 비공식적인 판단이 아니라 정해진 엔지니어링 또는 품질 판정 프로세스(Quality Disposition Process)를 따라야 한다.

초도품 검사에서 발견되는 부적합은 제조 시스템에 대한 중요한 정보를 제공한다. 치수 오류는 와이어 준비, 보드 레이아웃, 치구 위치 또는 조립 방법에서 발생할 수 있으며, 잘못된 커넥터 회로는 문서, 라벨링, 공정 순서의 문제를 나타낼 수 있다. 따라서 근본 원인 분석(Root-Cause Investigation)은 검사된 하니스에서 눈에 보이는 결함만 수정하는 것이 아니라 전체 제조 체계(Manufacturing Chain)를 대상으로 수행해야 한다.

시정 조치(Corrective Action)는 문제의 근본 원인을 해결하고 수정된 공정이 적합한 결과를 생산하는지 다시 검증해야 한다. 문제의 특성에 따라 금형, 하니스 보드 치구, 작업 지침, 재료 관리, 검사 기준, 작업자 교육 또는 엔지니어링 문서의 변경이 필요할 수 있다. 수정 이후 영향을 받은 특성을 다시 검사하여 시정 조치가 효과적일 것이라는 가정이 아니라 실제 검증 결과를 근거로 생산 승인을 수행해야 한다.

추적성(Traceability)은 초도품과 해당 제품이 제조된 조건에 대한 이력 기록을 제공한다. 기록에는 제품 식별 정보, 개정 상태, 와이어 및 터미널 로트, 장비와 어플리케이터(Applicator) 식별 정보, 하니스 보드 식별 정보, 작업자 정보, 검사 장비, 측정 결과, 전기 시험 기록, 부적합, 시정 조치, 승인 정보 및 생산 날짜 등이 포함될 수 있다. 이러한 기록은 이후 발생하는 문제 조사와 후속 생산품 비교를 위한 기준선(Baseline)을 제공한다.

기존 초도품 검사에서 검증한 전제조건을 무효화할 정도의 중요한 변경이 발생하면 초도품 검사를 다시 수행해야 할 수 있다. 제품 설계, 와이어 또는 터미널 구성, 금형, 제조 장소, 하니스 보드, 중요 공정 파라미터 또는 기타 관리되는 생산 조건이 변경되면 해당 품질 시스템에 따라 부분 또는 전체 재검증(Revalidation)이 필요할 수 있다. 재검증 범위는 변경으로 영향을 받을 가능성이 있는 특성에 맞추어 결정해야 한다.

로보틱스(Robotics) 및 자율이동로봇(AMR, Autonomous Mobile Robot) 하니스에서는 하나의 하니스가 배터리 전원, 모터 제어, 센서, 통신 네트워크, 컴퓨팅 장비, 충전 인터페이스 및 움직이는 모듈을 통합할 수 있기 때문에 초도품 검증이 특히 중요하다. 치수, 전기 및 작업 품질 오류가 여러 서브시스템(Subsystem)에 동시에 영향을 줄 수 있으므로 반복 생산 전에 검증을 수행하면 체계적인 제조 오류가 여러 로봇이나 조립체에 반복적으로 적용될 가능성을 감소시킬 수 있다.

초도품 검사(First Article Inspection)는 제조 및 공정(Manufacturing and Process) 장에서 구축된 제조 체계를 완성한다. 자동 절단-탈피-압착(Automatic Cut-Strip-Crimp)은 관리된 터미널 체결 리드(Terminated Lead)를 생산하고, 압착 단면 분석(Crimp Cross-Section Analysis)은 터미널 건전성을 검증하며, 하니스 보드 레이아웃(Harness Board Layout)은 조립 형상을 설정하고, 표준화된 작업 지침(Standardized Work Instruction)은 반복 가능한 작업 실행을 정의한다. 마지막으로 초도품 검사는 이러한 관리 요소가 하나의 시스템으로 정상적으로 작동하는지 검증하여 신뢰성 높은 와이어 하니스를 정상 양산으로 승인하기 위한 객관적인 근거를 제공한다.
