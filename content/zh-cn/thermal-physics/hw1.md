---
title: "Problem Set 1"
subtitle: ""
date: 2023-03-29T20:00:00+08:00
draft: false
author: "Mebius"
authorLink: ""
---

Chapter1: 22, 25, 27, 29, 33, 42, 46, 47 

Chapter2: 1, 4, 7, 10

## 需要记忆
大气压： 1atm = 1.013E5 Pa
绝对零度：0K = -273.15$^{\circ}$C
常见原子：CNOH的摩尔质量
气体摩尔质量：氧气（32g/mol），氮气（28g/mol），氦气（4g/mol），空气（29g/mol）
理想气体状态方程：

$$ pV=nRT \quad or \quad p\mu=\rho RT $$

## 作业答案
### 2-1
（1）认为房间中的空气满足理想气体状态方程，房间的体积 $V=100m^3$则数目 N 为
$$
N=nN_{A}=N_{A} \frac{pV}{RT}=2.69\times 10^{27}
$$
（2）量级正确且估算合理即可。采取一种简单的模型，认为粒子只能朝向“上下左右前后”六个方向运动，且速度为定值 $\bar{v}$， 则有
$$
\Gamma=\frac{1}{6} \frac{N}{V} \bar{v} = 2 \times 10^{27} m^{-2}
$$
严格计算需要使用麦克斯韦速率分布，请参考教材小孔泄流的部分，在这里仅给出结果
$$
\Gamma=\int_{0}^{+\infty} f(v_{x})v_{x} \, dv_{x} =\frac{1}{4}n \bar{v}
$$
其中 **n 为粒子数密度 n=N/V**，$f(v_{x})$ 为x方向的麦克斯韦速度分布率， $\bar{v}$ 为粒子平均速率。
（3）带公式即可，其中n为粒子数密度n=N/V，与第一问中的摩尔数不同
$$
Z=\sqrt{ 2 }n\pi d^2 \bar{v}=7.3 \times 10^9 Hz
$$
（4）平均自由程为
$$
\lambda=\frac{\bar{v}}{Z}=6\times 10^{-8}m
$$
### 2-4
由几何关系（参考教材图2.11），可得碰撞截面为
$$
\sigma=\pi \left(\frac{ d_{1}+d_{2}}{2}\right)^2=\frac{\pi}{4}d_{1}^2
$$
其中 $d_{1},d_{2}$ 分别为气体、电子的直径，由题意我们忽略电子的贡献。
由于我们认为气体静止，则他们的相对速度主要由电子提供，故无需乘 $\sqrt{ 2 }$ ，故有
$$
\lambda=\frac{1}{n\sigma}=\frac{4}{n\pi d_{1}^2}
$$
### 2-7
对于自由通过的电子，他们的数量正比于电子流强度，我们可以将这个过程视为泊松分布（参考教材例2.2），则有
$$
I(l)=I(0)\exp\left( -\frac{l}{\lambda} \right)
$$
其中 $I(l)$ 代表 $l$ 处的电子流强度，带入数据
$$
I(0)=100\mu A, \quad I(10cm)=37\mu A
$$
得到
$$
\lambda=10cm
$$
回顾2-4结论
$$
\lambda=\frac{4}{n\pi d_{1}^2} \propto \frac{1}{n} = \frac{k_{B}T}{pV} \propto \frac{1}{p}
$$
所以在气压减半且其他条件不变时，平均自由程加倍。
$$
I(20cm)=I(0)\exp\left( -\frac{l_{0}}{2\lambda} \right) = 100\exp\left( -\frac{10}{20} \right)\mu A= 60.6\mu A
$$
### 2-10
（1）套用分子动理论的结论即可，其“平均自由程”
$$
\lambda=\frac{1}{\sqrt{ 2 }n\pi d^2}=0.78m
$$
（2）两次碰撞间平均时间间隔为
$$
\tau=\frac{\lambda}{\bar{v}}=0.71s
$$
（3）在1s内平均碰撞次数为
$$
N=\frac{1s}{\tau}=1.4
$$

### 1-22
对于潜水艇中气箱，初态和末态有
$$
pV=nRT ,~ ~ ~p'V'=nRT' 
$$
其中$p=120kg/cm^2,~V=20L,~T=293K,~T'=278K$, 对于排水后的压强应有受力平衡
$$
p'=p_{0} + p_{水压}\approx 4kg/cm^2
$$
所以排除的体积为
$$
\Delta V=V'-V= 549L
$$
### 1-25
实际上，实验表明在气体压强趋于零时，理想气体状态方程对所有气体适用（教材Page35）。写出理想气体状态方程
$$
p\mu=\rho RT
$$
故有
$$
\mu = R T \lim_{ p \to 0 } \frac{\rho}{p}= 59g/mol
$$
其中的极限可以用在 $\frac{\rho}{p}-p$ 图中拟合的直线截距代替（请学会使用卡西欧拟合直线）。
### 1-27
混合气体的压强可以用各个组分的压强之和计算
$$
p=p_{o_{2}} + p_{N_{2}} + p_{Ar} = \frac{RT}{V}(n_{O_{2}}+n_{N_{2}}+n_{Ar})=2.58\times 10^
{-2} Pa
$$
其中 n 代表摩尔数，我们可以通过原子数 N 或者气体质量 m 和气体摩尔数 $\mu$ 计算
$$
n_{i}=\frac{N_{i}}{N_{A}}=\frac{m_{i}}{\mu_{i}}
$$
### 1-29
氧气：混合后气体并没有发生反应，容器的体积和温度不变，所以氧气的分压不变。
氮气：混合后发生等温变化，分压变化为
$$
p'_{N_{2}}=p_{N_{2}}\frac{V}{V'}=2.5atm
$$
综上，混合后各个气体压强 $p_{i}$ 和总压强 p 有
$$
p_{O_{2}}'=1atm~, \quad p_{N_{2}}'=2.5atm~,\quad 
p'=p_{O_{2}}' + p_{N_{2}}' = 3.5atm
$$
### 1-33
由于烘烤前压强相对烘烤后极小，由于没有给出更多有关抽真空时的温度信息，我们不妨认为烘烤后容器中的气体分子都是由器壁提供的。则有
$$
N=\nu N_{A}=\frac{pV}{RT}N_{A}=1.89\times 10^{18}
$$
### 1-42
（1）对初态有 $RT_{1}=p_{1}\nu_{1}=p_{1}^2/k$ ，故有
$$
k=\frac{p_{1}^2}{RT_{1}}
$$
（2）易知 $RT=p\nu=k\nu^2$
$$
T_{2}=4T_{1}=800K
$$
### 1-46
（1）理想气体
$$
p_{1}=\frac{nRT}{V}=7.271\times 10^6Pa
$$
若用范德瓦尔斯则有
$$
p_{2}=\frac{nRT}{V-\nu b}-\frac{a}{V^2}=5.86\times 10^6 Pa
$$
（2）范德瓦尔斯计算的更小，这是因为在这个密度上分子间作用力为引力，且有分子本身占据一部分体积（这部分非常小，在这种情况下不占主导）。差值百分比为
$$
\eta=\frac{p_{1}-p_{2}}{p_{1}}=19\%
$$
（3）与第一问相似，答案为
$$
p_{1}=7.272\times 10^6 Pa,~\quad p_{2}=7.122\times 10^{6}Pa,~\quad \eta=2\%
$$
这是因为当体积增大时，分子间距变大，相互之间作用力趋于零，且占据的体积也可以忽略不计。所以气体性质更接近理想气体。

### 1-47
套用体膨胀系数和等温压缩系数的公式即可，对体中气体有
$$
\nu = \frac{RT}{p}(1+pB(T))
$$
其中体膨胀系数有

$$ \alpha=\frac{1}{V}\left( \frac{ \partial V }{ \partial T } \right)_{p}
= \frac{1}{p\nu} \left( R(1+Bp) + RTp\frac{dB}{dT}\right) 
= \frac{1}{T} + \frac{p}{1+Bp}\frac{dB}{dT} $$
等温压缩系数有
$$
\beta=-\frac{1}{V}\left( \frac{ \partial V }{ \partial p }  \right)_{T}
= \frac{1}{p(1+Bp)}
$$