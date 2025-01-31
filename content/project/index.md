---
title : "社区项目"
date : "2020-05-29T13:47:08+02:00"
---

> 本页面所有项目参与开源软件供应链点亮计划暑期 2021 项目活动，如您参与，请先仔细阅读[学生指南](https://summer.iscas.ac.cn/help/student/)。

## 基于eBPF的网络性能监控与异常检测

- 项目ID： 210520870
- 难 度：高
- 支持语言： 中文

- 项目描述：

  随着网络规模的不断扩大，网络性能异常的问题越来越突出，网络性能的监控与异常检测尤为重要。网络故障或网络入侵等通常会引起网络性能异常，网络异常检测是维护网络正常运行、确保网络安全的一个重要手段。异常检测首先建立系统、网络和程序的正常模式，在后续检测过程，把偏离该模式的行为判定为网络异常事件或行为。传统的网络性能一般通过网络测量、 SNMP 或系统日志的方式计算得到，本课题要求基于eBPF技术进行获取网络性能数据。首先，分析Linux内核源代码，找出网络性能指标的监控点，使用eBPF技术提取内核网络性能数据，并进行可视化展示。其次，选择合适的算法检测网络性能的异常状况。异常检测可以分为固定阈值检测或自适应检测。目前采用的异常检测方法和基于固定阈值过滤的策略，其基本思想是对每种性能值设定一个阈值，性能数据超过阈值便被认定为异常事件。自适应异常检测算法，通常可以分为 3 种类型：基于统计特征的算法 ，基于机器学习的算法和基于数据挖掘的算法。最后，对接到社区项目LMP中，并能够成功运行。

- 项目社区导师：陈莉君
- 导师联系方式：<cljcore@126.com>

## Linux内核下系统内存及进程内存相关信息提取及预测

- 项目ID： 210520871
- 难 度：高
- 支持语言： 中文

- 项目描述

  首先：本题需要提取下列4个指标： 全系统的内存水位变化 按内存段提取进程的内存用量 按进程提取页换入信息 按进程提取巨页缺页错误相关信息 其次：要求从Linux内核中实时提取到相关数据后，经过处理，可以在网页前端展示系统当前的内存情况，并且需要将该功能实现为社区项目LMP的插件，并成功对接到LMP中 最后：需要选择一个合适的预测算法，根据当前内存指标情况，给出下个阶段可能的指标大小，其中指标数据需要存放在LMP的数据存储模块中，并且需要将该模型对接到社区项目LMP中，并能够成功运行。

- 项目社区导师：陈莉君
- 导师联系方式：<cljcore@126.com>

## LMP下数据处理的支持

- 项目ID： 210520872
- 难 度：低
- 支持语言： 中文

- 项目描述：

  LMP是一个基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。LMP项目正在规划数据处理功能，即数据采集模块提取到性能数据后，会将数据保存到数据存储模块，但是这些数据是原始数据，并不能直接交给机器学习模型处理，本题目需要实现数据存储模块中数据的预处理功能，例如数据清洗、数据转换、数据标准化等，并且需要采用不同方式来实现以上功能，所有功能需要对接到LMP项目中，并且可以正常使用。

- 项目社区导师：陈莉君
- 导师联系方式：<cljcore@126.com>

## HTTP、DNS网络态势预测

- 项目ID： 210520877
- 难 度：低
- 支持语言： 中文

- 项目描述
  LMP是一个基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。eBPF技术的出现使得我们可以更为精确地提取网络指标，因此本题目要求使用eBPF技术实现HTTP、DNS的性能监控，不限于传统的网络指标，需要探索Linux内核中可以利用的HTTP、DNS数据，要求至少从以下6个处理维度中选取4个维度对HTTP、DNS性能进行刻画展示：1、HTTP请求；2、HTTP响应；3、HTTP延时；4、DNS请求5、DNS响应6、DNS延时，从而达到探索Linux内核的目的。所有指标需要以插件形式成功对接到LMP项目之中。

- 项目社区导师：刘钊远
- 导师联系方式：<lzy781@126.com>

## LMP下数据存储模块的优化
- 项目ID： 210520878
- 难 度：低
- 支持语言： 中文

- 项目描述：
  LMP是一个基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。目前LMP项目中，插件提取的性能数据全部存储于influxdb中，本题目要求将目前项目中的数据存储模块中数据库换为ES数据库，并可正常支持项目目前的所有功能，并需要提供详细的文档说明。

- 项目社区导师：刘钊远
- 导师联系方式：<lzy781@126.com>

## LMP下应用程序进程线程的动态捕获
- 项目ID： 210520879
- 难 度：低
- 支持语言： 中文
- 项目描述

  LMP是一个基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。本题目要求利用eBPF技术实现应用程序进程线程的动态捕获，通过在内核中找到进程/线程的入口函数和出口函数，动态捕获应用程序在运行过程中产生的进程或者线程，并且需要成功对接到LMP项目中，且捕获到的PID等信息可以为其余插件服务。

- 项目社区导师：刘钊远
- 导师联系方式：<lzy781@126.com>

## 通过预选重要内核参数实现更快的IO性能调优
- 项目ID： 210520873

- 难 度：高

- 支持语言： 中文

- 项目描述：

  IO子系统拥有许多能够显著影响Linux系统行为的内核参数，调整这些参数可以显著提高性能。由于IO系统可调节参数较多，自动调优框架会花费大量时间探索庞大的配置空间，并且需要随着工作负载的变化而重复这一过程。 研究表明，有些参数相比其他参数对性能的影响更大，因此关注数量较少的更重要的参数可以加快自动调整系统的速度，因为需要探索的参数空间较小。 本题目要求设计并实现一个框架，首先能够对IO子系统全部可调节参数形成的参数空间进行合理降维，依据降维后的参数空间作为当前系统配置，运行工作负载并记录该点的性能指标（例如吞吐量、延时），输出配置空间中的点和对应的性能指标形成数据集。 然后提出重要性指标，通过机器学习方法预选出重要参数并进行重要性排序，能够使用前端页面展示当前IO子系统的Top5重要参数。 最后，选手可自行选择离线训练或者在线训练的方式预选重要参数，离线训练时间应尽可能短，预选参数达到的性能尽可能高，参数空间覆盖面应尽可能广。

- 项目社区导师：许振文

- 导师联系方式：<helight@qq.com>

## Linux内核TCP性能分析工具
- 项目ID： 210520874

- 难 度：低

- 支持语言： 中文

- 项目描述：

  LMP（Linux microscope）是Linux内核之旅社区开发的一款基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。TCP虽然作为可靠的传输层网络协议，但在最初设计的时候并没有把所有的应用场景考虑到，大型网络相关项目开发时往往会考虑优化TCP协议性能，这就需要提供TCP协议性能分析工具提供运维测试，eBPF技术的出现使得我们从内核角度去看待网络性能，因此本题目要求使用eBPF技术实现TCP层的性能监控，不限于传统的网络指标，需要探索Linux内核中TCP层有哪些可以利用的数据，要求至少从Linux内核中以下5个处理维度中选取4个维度对TCP性能进行刻画展示：1、数据包连接、传输情况；2、丢包或重传；3、拥塞控制；4、Conncet(三次握手)连接延迟、5、HTTP处理，并且需要采用BCC方式开发，并成功对接到社区LMP项目中。

- 项目社区导师：许振文

- 导师联系方式：<helight@qq.com>

## LMP（Linux microscope）项目插件添加
- 项目ID： 210520875

- 难 度：低

- 支持语言： 中文

- 项目描述：

  LMP（Linux microscope）是Linux内核之旅社区开发的一款基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，与常规Linux系统性能数据展示工具不同，该项目是一种内核态监控方案，目前在ubuntu18.04上测试通过，内核版本4.15.0。LMP数据提取模块支持多种插件类型，包括BCC插件、CBPF插件、SHELL插件等。目前项目主体架构开发已经完成，但bcc插件数量较少，使得LMP无法发挥出其真正能力，故需要向LMP中添加插件，丰富插件库，更好的支撑项目发展。在BCC现有工具中，对接包括scheduler、Virtual Memory、Sockets、TCP/UDP、VFS、File Systems、Volume Manager、Block Device等子系统的性能监测工具到LMP系统之中。

- 项目社区导师：许振文

- 导师联系方式：<helight@qq.com>

## LMP项目前端网页优化

- 项目ID： 210520867

- 难 度：低

- 支持语言： 中文

- 项目描述：

  LMP是一个基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。LMP项目目前需要优化前端页面，本题目要求采用vue框架，配合后端逻辑实现前端指标展示、指标选取、指标状态展示和性能数据可视化展示功能，要求功能完备，页面美观。

- 项目社区导师：陈继峰

- 导师联系方式：<chenlinuxer@163.com>
  
## 基于eBPF的DDos攻击检测
- 项目ID： 210520868

- 难 度：高

- 支持语言： 中文

- 项目描述：

  网络安全问题一直是人们最关注的问题之一。ddos攻击仍是最常见、最常用的的一种攻击手段。 由于其使用简单、攻击效果明显能够快速的消耗系统资源，使得正常的服务请求不能够正常访问。因此，如果能够追踪不同的ddos攻击方式在linux系统攻击的过程。提取ddos在攻击过程中表现出的不同的一些行为特征和指标数据，进行检测分析，对系统防御具有重要的意义。eBPF技术在系统追踪、观测、性能调优、安全和网络领域发挥着重要的角色。eBPF技术的出现对ddos攻击的过程进行跟踪观测成为了可能。因此本题目要求通过eBPF技术提取ddos攻击在linux系统的指标数据。设计出相应的检测算法，算法要能够进行ddos攻击的溯源，找到攻击的源头。最后，可以使用xdp技术对攻击的源头进行防御，数据提取功能和检测算法需要对接到LMP项目中。

- 项目社区导师：陈继峰

- 导师联系方式：<chenlinuxer@163.com>

## LMP项目下插件API的优化

- 项目ID： 210520869

- 难 度：低

- 支持语言： 中文

- 项目描述：

  LMP是一个基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。目前LMP项目中支持接入BCC类型的插件，每一个插件需要调用项目提供的API接口才能将性能数据写入到influxdb数据库。本题目要求优化API接口和插件管理，设计出一套较为完善和稳定的API接口，并优化所有的插件管理，例如目录管理等。

- 项目社区导师：陈继峰

- 导师联系方式：<chenlinuxer@163.com>

## NUMA节点的CPU UNCORE共享资源的争用感知与评估

- 项目ID： 210520848

- 难 度：高

- 支持语言： 中文

- 项目描述：

  NUMA架构是目前商用服务器使用的一种主流架构，其分布式内存设计提高了多处理器系统的可扩展性。但是，NUMA下各种共享资源的争用却影响着应用程序的性能。共享资源竞争主要发生在节点内处理器的UNCORE部分，其包含了三种主要的竞争资源：LLC（ Last Level Cache）、 QPI链路和内存控制器（IMC），这三种访存性能事件可以反映节点的访存压力情况。因此，感知NUMA内节点的访存压力情况，对于指导多线程应用程序的优化具有重要作用。本题目首先要求自己设计并实现一种框架，在内核态下从Intel处理器的PMU中读取UNCORE的三种访存性能事件类型（LLC、QPI、IMC）的计数值，并在用户态进行展示。三种类型下具体的访存性能事件的选取由自己选定，所选取的性能事件需要能反映出当前节点的访存压力情况。其次，用户态程序需要依据性能事件计数值评估每个节点的访存压力，并依据压力由高到低将节点进行排序。最后，要求所实现框架能够成功运行。

- 项目社区导师：赵晨雨

- 导师联系方式：<lonemorelightp@163.com>

## LMP项目下插件和数据提取功能的优化
- 项目ID： 210520864

- 难 度：低

- 支持语言： 中文

- 项目描述：

LMP是一个基于BCC(BPF Compiler Collection)的Linux系统性能数据实时展示的web工具，是Linux内核之旅社区项目。目前LMP项目中，插件在执行过程中会直接将性能数据存放到数据存储模块中，因为eBPF的特性，在磁盘IO等场景会出现数据提取和存储死循环的问题，现需要将数据提取和数据存储隔离为两个服务，该功能方案较多，需要提出不同的方案并比较优劣，选取最佳方案实现，在此过程中可以优化LMP插件API。

- 项目社区导师：赵晨雨

- 导师联系方式：<lonemorelightp@163.com>

## Linux内核下CPU cache统计及预测
- 项目ID： 210520865

- 难 度：高

- 支持语言： 中文

- 项目描述：

  缓存的引入，平衡了CPU和内存的处理速度。但随即带来的缓存争用，无疑影响了CPU以及其上运行进程的性能。因此，了解缓存的分布情况，对缓解缓存争用，从而实现CPU利用率最大化和负载均衡等目标，都有着巨大的指导意义。本题首先要求从Linux内核中实时提取到CPU cache相关数据后，经过处理，可以在网页前端展示系统当前的缓存分布情况，并且需要将该功能实现为社区项目LMP的插件，并成功对接到LMP中；其次需要选择一个合适的预测算法，根据当前缓存分布情况，给出下个阶段可能的缓存分布，其中性能数据需要存放在LMP的数据存储模块中，并且需要将该模型对接到社区项目LMP中，并能够成功运行。

- 项目社区导师：赵晨雨

- 导师联系方式：<lonemorelightp@163.com>