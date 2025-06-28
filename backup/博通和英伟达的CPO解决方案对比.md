### 关键要点

- 研究表明，博通和英伟达的CPO解决方案在目标和应用上高度一致，均用于提升数据中心性能。
- 证据显示，英伟达的带宽和功耗效率可能更高，但博通的解决方案已量产，技术更成熟。
- 两者在调制器技术和市场定位上存在显著差异，存在一定争议，取决于具体需求。
![image.png](https://raw.githubusercontent.com/lxc-one/img4app/main/img/20250628102155024.png)


![image.png](https://raw.githubusercontent.com/lxc-one/img4app/main/img/20250628102226986.png)


### 概述

博通和英伟达的Co-Packaged Optics（CPO，协同封装光学）解决方案旨在通过将光模块与芯片集成，提升数据中心和AI计算的带宽和能效。以下是两者的主要异同点，适合普通用户理解。

### 相同点

- 目标一致：两者都聚焦于解决数据中心的高带宽和低功耗需求，特别适用于AI和高性能计算。
- 能效提升：两者均声称显著降低功耗，博通减少3倍，英伟达声称高效3.5倍。
- 可靠性提高：两者都强调CPO技术提升网络可靠性，减少组件故障。

### 不同点

- 技术成熟度：博通的解决方案已量产，提供51.2Tb/s带宽，计划2025年升级至102.4Tbps。英伟达的解决方案尚未全面上市，Quantum-X预计今年晚些时候推出，带宽高达115.2Tbps，Spectrum-X在2026年推出，可达409.6Tbps。
- 带宽容量：英伟达的带宽明显更高，适合大规模AI集群；博通当前带宽较低，但更适合现有数据中心。
- 技术差异：博通使用Mach-Zehnder调制器，成熟但功耗较高；英伟达用Micro-Ring Resonator调制器，功耗低但需额外热管理。
- 市场定位：英伟达更聚焦未来百万GPU级别的扩展，博通更适合当前需求，提供更高集成密度。

更多细节请见下文调查报告。

  

### 调查报告：博通与英伟达CPO解决方案的全面比较

博通（Broadcom）和英伟达（NVIDIA）作为半导体行业的领导者，在Co-Packaged Optics（CPO）领域均有显著布局。CPO技术通过将光模块与芯片封装在一起，旨在解决数据中心和AI计算中的带宽瓶颈和功耗挑战。以下是基于2025年6月27日最新数据的详细分析，涵盖两者的技术实现、应用场景和市场定位。

### 技术实现的异同

相同点

- 核心目标：两者均致力于通过CPO技术提升数据传输速度和降低能耗，特别针对数据中心和AI集群的高带宽需求。
- 功耗效率：两者都声称其CPO解决方案相较传统插拔式光模块（pluggables）显著降低功耗。博通表示其解决方案每800Gb/s端口功耗为5.5W，较插拔式光模块减少3倍（约15W）；英伟达声称其解决方案比传统网络高效3.5倍，提供3.5倍的能效提升。
- 可靠性提升：两者均强调CPO减少组件数量，从而提高网络可靠性。英伟达具体提到其解决方案的网络容错性提高10倍，信号可靠性提升63倍。

不同点

- 技术成熟度与上市时间：博通的Bailly CPO交换机（基于Tomahawk-5 ASIC）已于2025年初投入量产，提供51.2Tb/s带宽（64 x 800Gbps或128 x 400Gbps），并计划在2025年下半年推出102.4Tbps的下一代解决方案。相比之下，英伟达的Quantum-X（InfiniBand）预计今年晚些时候上市，提供115.2Tbps（144 x 800Gb/s或576 x 200Gbps），而Spectrum-X（Ethernet）则定于2026年推出，带宽可达409.6Tbps（512 x 800Gbps）。
- 带宽容量：英伟达的解决方案在带宽上明显领先，Quantum-X提供115.2Tbps，Spectrum-X最高可达409.6Tbps，适合未来百万GPU级别的AI工厂。而博通当前提供51.2Tb/s，计划升级至102.4Tbps，更多满足当前800G Ethernet时代的需求。
- 调制器技术：博通使用Mach-Zehnder Modulator（MZM），功耗范围为5-10pJ/bit，占地面积较大，但温度耐受性更好，便于与现有基础设施集成。英伟达采用Micro-Ring Resonator Modulator（MRM），功耗更低（1-2pJ/bit），支持波分复用（WDM），但对温度敏感，需要额外的加热电路。
- 集成方式：博通的解决方案将8个6.4Tbps硅光子引擎直接集成到封装中，提供更高的“海滩密度”（beachfront density），光纤耦合为边缘耦合，当前每个引擎16对光纤，可能扩展至64对。英伟达使用可拆卸的光学服务组件（OSA），每4.8Tbps包含3个1.6Tbps引擎，光纤耦合同样为边缘耦合，Quantum-X提供324个光连接（144对光纤用于144 x 200Gbps），提升可服务性和灵活性。
- 波分复用（WDM）：博通使用粗波分复用（Coarse WDM），每个光纤支持400G（4λ x 100G），但800Gbps端口配置尚未明确。英伟达不使用WDM，依赖更高的光纤数量，例如Quantum-X使用144对光纤支持144 x 200Gbps。
- 冷却需求：博通的当前解决方案可能初始为空气冷却，但高密度配置可能需要液冷。英伟达明确使用液冷，尤其在GTC 2025演示中展示了其解决方案的液冷需求。

### 应用场景与市场定位

相同点

- 应用领域：两者均服务于数据中心网络，特别适用于AI训练、推理和高性能计算（HPC）场景，满足大规模数据传输需求。
- 合作伙伴生态：两者均与光模块制造商和系统集成商合作，推动CPO技术的落地。博通与Micas Networks合作，英伟达则与TSMC、Corning、Foxconn等11家合作伙伴合作。

不同点

- 市场定位：博通的CPO解决方案更聚焦于当前数据中心需求，提供更高的集成密度，适合现有800G Ethernet时代（100G SerDes），其51.2Tbps解决方案已对齐当前网络需求，2025年计划推出100Tbps。英伟达则更注重大规模AI集群的未来需求，带宽从100Tbps跃升至400Tbps（200G SerDes），支持连接超过10,000个GPU，适合百万GPU级别的AI工厂。
- 扩展性：英伟达的解决方案通过多光子开关芯片实现更高基数（radix）交换，模块化设计（如可拆卸OSA）提升扩展性和可服务性。博通的单封装设计更紧凑，但扩展性相对较弱。

### 详细数据对比

以下表格总结了两者的关键技术参数：

|           |                                                          |                                                                                 |
| --------- | -------------------------------------------------------- | ------------------------------------------------------------------------------- |
| **品牌**    | **博通（Broadcom）**                                         | **英伟达（NVIDIA）**                                                                 |
| **产品**    | Bailly CPO交换机（Tomahawk-5 ASIC）                           | Quantum-X（InfiniBand）和Spectrum-X（Ethernet）光子交换机                                 |
| **带宽**    | 51.2Tb/s（64 x 800Gbps或128 x 400Gbps），计划2025年下半年102.4Tbps | Quantum-X：115.2Tbps（144 x 800Gbps或576 x 200Gbps）；Spectrum-X：102.4Tbps或409.6Tbps |
| **光学引擎**  | 8个6.4Tbps硅光子引擎，直接集成                                      | 多个1.6Tbps引擎，每4.8Tbps包含3个引擎，可拆卸模块                                                |
| **光纤耦合**  | 边缘耦合，400G-FR4（4λ x 100G），每个引擎16对光纤，可能扩展至64对              | 边缘耦合，Quantum-X：324个光连接（144对光纤用于144 x 200Gbps）                                   |
| **激光器集成** | 外部，16个可插拔激光器模块（每个6.4Tbps引擎2个）                            | 外部，Quantum-X：18个激光器模块（每个供应8个引擎），单位带宽激光器数量更少                                     |
| **调制器**   | Mach-Zehnder Modulator（MZM），5-10pJ/bit，温度耐受性更好           | Micro-Ring Resonator Modulator（MRM），1-2pJ/bit，支持WDM，温度敏感                        |
| **WDM**   | 使用粗波分复用（Coarse WDM），每个光纤400G（4λ x 100G）                  | 不使用WDM，依赖光纤数量（例如，144对光纤用于144 x 200Gbps）                                         |
| **功耗效率**  | 每800Gb/s端口5.5W，6-7pJ/bit，较插拔式光模块减少3倍                     | 比插拔式光模块高效3.5倍，使用MRM和更少激光器，需液冷                                                   |
| **冷却**    | 可能初始为空气冷却，高密度可能需液冷                                       | 明确使用液冷                                                                          |
| **可靠性**   | 高可靠性，减少组件导致的链路抖动                                         | 网络容错性提高10倍，信号可靠性提高63倍                                                           |
| **部署速度**  | 未明确                                                      | 部署速度提高1.3倍                                                                      |
| **合作伙伴**  | Micas Networks                                           | TSMC、Corning、Foxconn等11家合作伙伴                                                    |
| **市场定位**  | 当前数据中心需求，海滩密度高                                           | 大规模AI集群，支持百万GPU级别扩展                                                             |

### 争议与未来趋势

CPO技术的推广面临一定争议，例如与传统插拔式光模块的竞争。一些分析（如Yole Group报告，[Co-Packaged Optics for Datacenter 2023](https://www.yolegroup.com/product/report/co-packaged-optics-for-datacenter-2023/)）指出，插拔式光模块在未来两代交换系统内仍具优势，CPO的全面部署可能需要更长时间。博通和英伟达的解决方案在调制器选择上也存在技术路线之争，MZM更成熟但功耗高，MRM更高效但热管理复杂。

未来趋势显示，英伟达的带宽和扩展性更适合AI工厂的长期需求，而博通的解决方案可能在短期内更具实用性。两者均需克服液冷成本和生态系统兼容性挑战。

### 结论

综上所述，博通和英伟达的CPO解决方案在目标和能效提升上高度一致，但技术路径和市场定位存在显著差异。博通更适合当前数据中心需求，已量产且技术成熟；英伟达则更聚焦未来AI集群的扩展，带宽和功耗效率更高，但上市时间较晚。用户选择应根据具体需求（如即时部署或长期扩展）权衡。

  

### 关键引文

- [Broadcom CPO最高功耗效率和带宽密度](https://www.broadcom.com/info/optics/cpo)
- [新标准推动协同封装光学](https://semiengineering.com/new-standards-push-co-packaged-optics/)
- [博通协同封装光学产品](https://www.broadcom.com/products/fiber-optic-modules-components/co-packaged-optics)
- [如何通过CPO扩展光学互连](https://www.broadcom.com/blog/how-to-scale-the-optical-interconnect-using-co-packaged-optics-cpo)
- [英伟达光学开关可能改变AI数据中心](https://spectrum.ieee.org/co-packaged-optics)
- [协同封装光学深入探讨](https://blog.apnic.net/2025/05/07/co-packaged-optics-a-deep-dive/)
- [英伟达光学收入超10亿美元](https://semianalysis.com/2023/08/23/nvidias-optical-ascent-1b-revenue/)
- [英伟达硅光子网络交换机](https://www.nvidia.com/en-us/networking/products/silicon-photonics/)
- [Yole Group半导体行业趋势](https://www.yolegroup.com/product/report/co-packaged-optics-for-datacenter-2023/)
- [博通英伟达受益于CPO技术](https://www.msn.com/en-us/money/technologyinvesting/broadcom-nvidia-among-those-set-to-benefit-from-co-packaged-optics-technology-j-p-morgan/ar-AA1GYAQZ)