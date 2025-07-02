# 背景介绍
贸易数字化也称无纸贸易，是当前数字经济国际合作的主要共识领域。2024年6-7月，70多个WTO成员国达成一致的WTO《电子商务协定》稳定文本，所凝聚的主要共识就是贸易数字化。联合国国际贸易法委员会（UNCITRAL）自2017年以来，也不断推动《电子可转让记录示范法》、《仓单示范法》、《可转让货物单证公约》等国际规则文件，推动国际贸易数字化合作。
2022年成立的北京贸易科技联盟，在北京市商务局、北京海关、朝阳区政府等政府部门的指导下，共同推动建立可信贸易协作网络（“信贸链”），打造开放、中立的贸易数字化网络。联盟秘书长单位——慧贸天下（北京）科技公司牵头开发了“信贸链”技术协议和相关的“慧贸OS”操作系统，同时，在北京市“两区”办和新加坡资讯通信媒体发展局（IMDA）的大力支持与推动下，“信贸链”兼容了IMDA开发的TradeTrust框架，以电子提单为突破口，实现了中国-新加坡首个全环节、分布式（互操作）贸易数字化实单试点（中粮-一丰试点）的落地。
下一步，为加快贸易数字化国际合作，慧贸天下在北京贸易科技联盟成员的大力支持下，决定向全球发布已遵循或兼容了UN/EDIFACT、TradeTrust、URDTT和KTDDE、ANSI、RosettaNet、IATA等国内和国际上诸多贸易数字化技术标准的“信贸链协议”（即全球贸易互操作协议），并发布“慧贸OS”产业操作系统的开源版、打造开源社区，推动各国贸易数字化系统的互联互通，不断提升跨国网络数据安全互信，共建全球可信贸易协作网络。
# 项目介绍
“信贸链协议” ，即全球贸易互操作性协议，是一套实现贸易参与方之间数字化系统高效互联互通和全环节贸易可信协作的通用技术规范。该协议分为五层，包括数字身份握手层、跨链流转与同步层、数据交换与存证层、数据标准转换层、交易过程管理层，其设计严格遵循并兼容包括UN/EDIFACT、TradeTrust、URDTT、KTDDE、ANSI X12、RosettaNet、IATA Cargo-XML等在内的多项国际及区域性贸易数字化技术标准。该协议基于区块链技术、人工智能技术底座所开发，旨在为构建数字化交易生态提供一套通用技术语言。
本项目是对信贸链协议以及信贸链协议实现的代码进行开源，以便让贸易参与各方可以,利用慧贸OS接入“信贸链”，用户可轻松与上下游伙伴进行无缝协作，完成从营销、物流、通关到结算等贸易全环节的数智化。
![image](https://github.com/user-attachments/assets/8f110b84-d634-4a40-a02e-585592bbf096)

# 主要模块说明
+ AEOTrade-Architecture：总体架构说明的目录
+ AEOTrade-ChainProtocol：信贸链协议白皮书，建议大家在使用该项目前可以优先阅读一下信贸链协议，便于大家对项目有一个宏观的认识，本开源项目主要也是基于信贸链协议的思想进行实现的，后续也会在协议的基础上进行后续迭代，希望通过信贸链协议能够让贸易参与各方能够在一个通用的技术规范下进行互联互通。https://github.com/aeotrade/AEOTrade-ChainProtocol
+ AEOTrade-Server：慧贸OS的主要后端程序，包括慧贸OS工作台、数字身份、协助合约编排等功能实现，并可以通过慧贸OS进行需求、产品发布，并可以通过慧贸OS的AI能力进行智能匹配。https://github.com/aeotrade/AEOTrade-Server
+ AEOTrade-Web: 慧贸OS的前端程序，包括慧贸OS工作台、数字身份、协助合约编排等功能实现。https://github.com/aeotrade/AEOTrade-Web
+ AEOTrade-Connection-System:连接器是慧贸OS的一个重要概念，连接器解决了企业内外部各个应用系统对接问题，你只需要将你的连接器上线就可以像搭积木一样，快速实现业务自动化处理和执行。https://github.com/aeotrade/AEOTrade-Connection-System
+ django-aeotrade-connector: 慧贸OS连接器开发框架，为了降低大家对连接器的开发难度，大家可以在框架的基础上快速开发，然后形成自己的连接器。https://github.com/aeotrade/django-aeotrade-connector
+ AEOTrade-Contract: 慧贸OS合约系统, 作为慧贸OS业务流程编排的后端支撑。https://github.com/aeotrade/AEOTrade-Contract
+ AEOTrade-Exchange:慧贸OS交换系统, 作为慧贸OS中各业务系统间信息传递，文件传递交换的后端支撑。https://github.com/aeotrade/AEOTrade-Exchange
+ AEOTrade-SmartContract: 基于信贸链协议的智能合约实现，目前代码中的合约主要是基于长安链进行的测试, 通过智能合约可进行交易过程存证和分布式数据存储。https://github.com/aeotrade/AEOTrade-SmartContract
+ AEOTrade-Deploy: 项目的部署方式说明，大家可以通过该项目完成慧贸OS开源版本的环境搭建与部署。https://github.com/aeotrade/AEOTrade-Deploy
# 下一步计划
联合权威机构，成立全球贸易科技联盟，融合国际高标准经贸规则和标准，建设“信贸链”开源社区，不断推进产业操作系统的迭代与升级，促进更多业务场景应用“信贸链”，推动“信贸链”成为全球数字贸易的通用基础设施。
# 开源协议说明
This software is licensed under the GNU Lesser General Public License (LGPL) version 3.0 or later. However, it is not permitted to use this software for commercial purposes without explicit permission from the copyright holder.
If the above restrictions are violated, all commercial profits generated during unauthorized commercial use shall belong to the copyright holder. 
The copyright holder reserves the right to pursue legal liability against infringers through legal means, including but not limited to demanding the cessation of infringement and compensation for losses suffered as a result of infringement.
本软件根据GNU较宽松通用公共许可证（LGPL）3.0或更高版本获得许可。但是，未经版权所有者明确许可，不得将本软件用于商业目的。
若违反上述限制，在未经授权的商业化使用过程中所产生的一切商业收益，均归版权所有者。
版权所有者保留通过法律途径追究侵权者法律责任的权利，包括但不限于要求停止侵权行为、赔偿因侵权行为所遭受的损失等。
