# Siegel: On Riemann’s Nachlass for Analytic Number Theory

# 说明

这篇论文即是1932年Siegel重新发现了Riemann $\zeta$函数零点计算公式的论文。一个大数学家研究另外一个大数学家的工作，进行原创性的评论与整理，在21世纪还是比较少见的，因为现在的信息交流实在太方便，而受过专业训练的PhD比20世纪多了很多，评价体系实在太卷，所以这种考古工作很少见了，如果有最新论文的Seminar，那可能也是闭门的讨论，一般读者很难见到，也不一定能看懂他们的加工创造过程。非数学的内容到此为止。

根据英文译本转译，英译本链接见：https://arxiv.org/abs/1810.05198。

英文译本作者为：Eric Barkan, David Sklar

原作者：Carl Ludwig Siegel

# 英译本摘要与评论

## 摘要

1859年，黎曼（Riemann，1826–1866）发表了他唯一的数论论文。在这篇八页的论文中，他得到了一个用于计算小于或等于实数 $x$ 的素数个数的公式，并揭示了素数分布与现称为黎曼 Zeta 函数的解析函数的零点之间的深刻联系。20世纪30年代初，20世纪伟大的数学家和学者卡尔·路德维希·西格尔（Carl Ludwig Siegel，1896–1981）在黎曼非常潦草的笔记中发现了两个相关的、源自1859年的未发表结果。

在他1932年的论文《关于黎曼解析数论的遗稿》（*Über Riemanns Nachlaß zur analytischen Zahlentheorie* / *On Riemann’s Nachlass for Analytic Number Theory*）中，西格尔展示了这些未发表的结果，并给出了他在黎曼笔记中发现的推导过程。第一个是一个渐近展开式，现在被称为黎曼-西格尔公式（Riemann-Siegel formula），用于高效计算黎曼 Zeta 函数的值。第二个是 Zeta 函数的一种新的积分表示。在黎曼之后的七十年里，这些结果一直未被重新发现。因此，西格尔1932年的这篇论文的重要性不仅在于它对数学史的贡献，还在于它对当时研究的贡献。

为了深入了解西格尔是如何从黎曼残缺不全且杂乱无章的个人文件中发现并破译这些珍宝的，我们决定研究这篇1932年的论文。我们还想知道这篇论文中有多少内容是黎曼原创的，以及西格尔是否需要填补空白。虽然每当讨论黎曼-西格尔公式时都会引用西格尔的这篇论文，但我们无法找到英译本。尽管我们的德语知识有限，我们还是依据西格尔全集第一卷中的内容完成了这篇论文的翻译。

## 评论（英文译者的评论）

1. 我们译文中的页码和公式编号均来自西格尔全集中的论文版本：*Gesammelte Abhandlungen*, Vol. 1, Springer-Verlag, Berlin (1966), pp. 275–310。

2. 我们的翻译仍在进行中。欢迎对翻译以及我们可能引入的数学错误进行指正和评论。


# 原文


在1859年致魏尔斯特拉斯（Weierstrass）的一封信中，黎曼（Riemann）提到了 $\zeta$ 函数的一个新展开式，然而他尚未将其简化到足以包含在他已发表的关于素数理论的论文中的程度。既然黎曼信中的这一点已由 H. Weber 在他 1876 年编辑的黎曼全集中发表，人们可以推测，对位于哥廷根大学图书馆的黎曼遗稿（Nachlass）进行详细审查，或许能让解析数论中隐藏的重要公式重见天日。

事实上，图书管理员迪斯特尔先生（Herr Distel）早在几十年前就在黎曼的文件中发现了这个关于 $\zeta$ 函数的表示法。它涉及一个渐近展开式，给出了函数 $\zeta(s)$ 在临界线 $\sigma = \frac{1}{2}$ 上，更一般地，在每个带状区域 $\sigma_1 \le \sigma \le \sigma_2$ 内，当 $s$ 的模无限增大时的行为。与此同时，该展开式的主项在 1920 年被哈代（Hardy）和李特尔伍德（Littlewood）独立于黎曼重新发现，作为他们“近似函数方程”的推论；他们使用了与黎曼相同的证明方法，即通过鞍点法近似计算积分。然而，在黎曼那里，还有一个获取渐近级数额外项的过程，该过程基于积分

$$ \Phi(\tau, u) = \int \frac{e^{\pi i \tau x^2 + 2\pi i u x}}{e^{2\pi i x} - 1} dx, $$

的优美性质，顺便提一下，这也引导克罗内克（Kronecker）以及最近莫德尔（Mordell）对高斯和的互反公式做出了极其优雅的推导。1926 年，贝塞尔-哈根（Bessel-Hagen）在对黎曼论文的新一轮审查中注意到了另一个先前未知的用定积分表示 Zeta 函数的方法；在此过程中，黎曼也受到了 $\Phi(\tau, u)$ 性质的引导。

$\zeta(s)$ 的这两种表示法可以列入黎曼数论遗稿中最重要的结果之列，毕竟在他已发表的论文中找不到它们。关于所谓的“黎曼猜想”的证明思路，甚至关于 Zeta 函数在临界线上存在无穷多个零点的证明思路，并未包含在黎曼的论文中。关于在区间 $0 < t < T$ 内渐近地有 $\frac{T}{2\pi} \log \frac{T}{2\pi} - \frac{T}{2\pi}$ 个 $\zeta(\frac{1}{2} + ti)$ 的实零点这一猜想，黎曼可能受到了渐近级数的启发式考量的引导；但直到今天，人们仍不清楚如何证明或证伪这一断言。借助渐近级数，黎曼还计算了 $\zeta(\frac{1}{2} + ti)$ 的一些实零点，以此获得更好的近似。

在黎曼关于 Zeta 函数理论的笔记中，没有直接可发表的材料；有时会在同一页上发现互不相关的公式；通常只写下方程的一边；即使在关键点上，也缺乏余项估计和收敛性研究。这些原因使得有必要对黎曼的残篇进行自由改编，正如在下文中所做的那样。

关于黎曼通过“高度概括”的思想发现其数学成果，而不需要形式化分析工具的传说，大概不像在克莱因（Klein）的时代那样广为流传了。黎曼的分析技巧究竟有多强，通过他对 $\zeta(s)$ 渐近级数的推导和处理表现得尤为明显。

## $\S$ 1. 一个定积分的计算

设 $u$ 为复变量。构造积分

$$ (1) \quad \Phi(u) = \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} dx, $$

积分路径从 $\infty$ 到 $\infty$，从右下到左上，沿着一条平行于第四和第二象限角平分线的直线进行，该直线在 0 和 1 两点之间穿过实轴。在公式 (1) 中，该积分路径用置于积分号下方的符号 $0 \nwarrow 1$ 表示。

函数 $\Phi(u)$ 是整函数。继黎曼之后，可以用一种简单的方式将其表示为指数函数的形式。为了证明这一点，利用柯西定理（Cauchy's Theorem）获得 $\Phi(u)$ 的两个差分方程：

一方面，我们有
$$
\begin{aligned}
\Phi(u+1) - \Phi(u) &= \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2} (e^{2\pi i (u+1)x} - e^{2\pi i u x})}{e^{\pi i x} - e^{-\pi i x}} dx = \int_{0 \nwarrow 1} e^{-\pi i x^2} e^{2\pi i (u + \frac{1}{2}) x} dx \\
&= e^{\pi i (u+\frac{1}{2})^2} \int_{0 \nwarrow 1} e^{-\pi i (x - u - \frac{1}{2})^2} dx = e^{\pi i (u+\frac{1}{2})^2} \int_{0 \nwarrow 1} e^{-\pi i x^2} dx,
\end{aligned}
$$
因此
$$ (2) \quad \Phi(u) = \Phi(u+1) - e^{\pi i (u+\frac{1}{2})^2} \int_{0 \nwarrow 1} e^{-\pi i x^2} dx. $$

另一方面，当积分路径用符号 $-1 \nwarrow 0$ 表示时（该路径由前面使用的路径平移向量 $-1$ 得到），我们有

$$ (3) \quad 1 = \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} dx - \int_{-1 \nwarrow 0} \frac{e^{-\pi i x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} dx, $$

因为被积函数在极点 $x=0$ 处的留数为 $\frac{1}{2\pi i}$；又因为

$$ \int_{-1 \nwarrow 0} \frac{e^{-\pi i x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} dx = \int_{0 \nwarrow 1} \frac{e^{-\pi i (x-1)^2 + 2\pi i u (x-1)}}{e^{\pi i (x-1)} - e^{-\pi i (x-1)}} dx = e^{-2\pi i u} \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2 + 2\pi i (u+1) x}}{e^{\pi i x} - e^{-\pi i x}} dx $$

方程 (3) 给出公式

$$ (4) \quad \Phi(u) = e^{-2\pi i u} \Phi(u+1) + 1. $$

由 (2) 和 (4)，首先对于 $u=0$ 得到著名的方程
$$ \int_{0 \nwarrow 1} e^{-\pi i x^2} dx = e^{\frac{3\pi i}{4}} $$
然后通过消去 $\Phi(u+1)$ 得到期望的结果
$$ (5) \quad \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} dx = \frac{1}{1 - e^{-2\pi i u}} - \frac{e^{\pi i u^2}}{e^{\pi i u} - e^{-\pi i u}}. $$

---

* 译者注：关于这个奇怪的记号，Gemni是这么说的：


![](https://files.mdnice.com/user/6944/a69510ba-4367-401a-896f-3be787467c80.png)



1. 积分路径的几何含义
这里的积分变量 $x$ 不再局限于实数轴，而是一个复变量（通常记为 $z$）。
路径方向：所谓“第四和第二象限角平分线”，在复平面上就是直线 $y = -x$（也就是倾斜角为 $135^\circ$ 或 $\frac{3\pi}{4}$ 的直线）。
路径位置：“平行于该线，且在 0 和 1 之间穿过实轴”。这意味着积分路径是一条直线 $L$，方程可以写为 $Im(z) = -Re(z) + c$，其中 $c$ 是一个使直线与实轴交点位于 $(0,1)$ 之间的常数。
走向：“从右下到左上”。这意味着积分是从复平面的第四象限（$\infty \cdot e^{-i\pi/4}$ 方向）走向第二象限（$\infty \cdot e^{3\pi i/4}$ 方向）。
2. 计算这个积分（化归为高斯积分）
这个积分的值 $\int e^{-\pi i x^2} dx = e^{\frac{3\pi i}{4}}$ 可以通过柯西积分定理（Cauchy's Integral Theorem）和平移路径来计算。
步骤如下：
平移路径：
由于被积函数 $f(z) = e^{-\pi i z^2}$ 是一个整函数（在全平面解析，没有奇点），且在无穷远处沿着该方向衰减得很快。根据柯西定理，我们可以将积分路径从“穿过 0 和 1 之间”平移到直接穿过原点，而不改变积分的值。
新的路径就是直线：$z = t \cdot e^{i \frac{3\pi}{4}}$，其中 $t$ 是实数，从 $-\infty$ 变到 $+\infty$。
变量代换：
在这个穿过原点的路径上，我们可以写出 $z$ 和 $dz$：
$$ z = t e^{i \frac{3\pi}{4}} $$
$$ dz = e^{i \frac{3\pi}{4}} dt $$
现在代入被积函数 $e^{-\pi i z^2}$：
$$ z^2 = (t e^{i \frac{3\pi}{4}})^2 = t^2 e^{i \frac{3\pi}{2}} = t^2 (-i) = -i t^2 $$
$$ -\pi i z^2 = -\pi i (-i t^2) = -\pi t^2 $$
你会发现，经过这个巧妙的路径旋转，指数部分原本的虚数 $-\pi i z^2$ 变成了实数 $-\pi t^2$。
计算定积分：
现在积分变成了标准的高斯积分形式：
$$ \int_{-\infty}^{\infty} e^{-\pi t^2} \cdot (e^{i \frac{3\pi}{4}} dt) $$
把常数提到积分号外面：
$$ = e^{i \frac{3\pi}{4}} \int_{-\infty}^{\infty} e^{-\pi t^2} dt $$
我们利用熟知的高斯积分公式 $\int_{-\infty}^{\infty} e^{-a t^2} dt = \sqrt{\frac{\pi}{a}}$。在这里 $a = \pi$，所以：
$$ \int_{-\infty}^{\infty} e^{-\pi t^2} dt = \sqrt{\frac{\pi}{\pi}} = 1 $$
最终结果：
$$ = e^{i \frac{3\pi}{4}} \cdot 1 = e^{\frac{3\pi i}{4}} $$


---注释与正文的分割线----

对 $u$ 及其微分 $n$ 次，得到一般公式
$$ (6) \quad \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} x^n dx = (2\pi i)^{-n} D^n \frac{e^{\pi i u} - e^{\pi i u^2}}{e^{\pi i u} - e^{-\pi i u}} \quad (n = 0, 1, 2, \dots). $$

为了接下来的讨论，方便将 (5) 写成另一种形式。将 $u$ 写成 $2u + \frac{1}{2}$ 并将 (5) 乘以 $e^{-2\pi i (u + \frac{1}{4})^2}$；这给出了黎曼发现的方程
$$ \int_{0 \nwarrow 1} \frac{e^{\pi i \{ x^2 - 2(u + \frac{1}{2} - x)^2 + \frac{1}{8} \}}}{e^{2\pi i x} - 1} dx = \frac{\cos(2\pi u^2 + \frac{3\pi}{8})}{\cos 2\pi u}, $$
该方程将继续发挥重要作用。
积分 $\Phi(u)$ 是积分
$$ (7) \quad \Phi(\tau, u) = \int_{0 \nwarrow 1} \frac{e^{\pi i \tau x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} dx, $$
的一个特例，对于它，两个差分方程也就足够了。莫德尔（Mordell）对此进行了进一步研究。对于 $\tau$ 的每个负有理数值，都有一个类似于 (5) 的公式；由此，通过对 $u$ 的特殊化，可以获得高斯和的互反律。在他的讲座中，黎曼将$\theta$函数的变换理论建立在 $\Phi(\tau, u)$ 的性质之上。

## $\S$ 2. Zeta 函数的渐近公式

如果复变量 $s = \sigma + ti$ 的实部 $\sigma$ 大于 1 且 $m$ 是一个自然数，那么
$$ \zeta(s) = \sum_{n=1}^{m} n^{-s} + \frac{1}{\Gamma(s)} \int_{0}^{\infty} \frac{x^{s-1} e^{-m x}}{e^x - 1} dx, $$
或者当 $C_1$ 是环绕负虚轴正向行进的回路时，
$$ (8) \quad \zeta(s) = \sum_{n=1}^{m} n^{-s} + \frac{(2\pi)^s e^{\frac{\pi i s}{2}}}{\Gamma(s) (e^{2\pi i s} - 1)} \int_{C_1} \frac{x^{s-1} e^{-2\pi i m x}}{e^{2\pi i x} - 1} dx. $$

这个公式甚至对 $\sigma$ 的任意值都有效。现在让 $\sigma$ 限制在一个固定的区间 $\sigma_1 \le \sigma \le \sigma_2$ 内，并设 $t > 0$。为了用鞍点法计算 (8) 中出现的积分在 $t \to \infty$ 时的渐近值，必须取通过 $D \log (x^{s-1} e^{-2\pi i m x})$ 的零点的积分路径。对于这个零点，从方程
$$ \frac{s-1}{x} - 2\pi i m = 0 $$
得到值
$$ (9) \quad \xi = \frac{s-1}{2\pi i m} = \frac{t}{2\pi m} + \frac{1-\sigma}{2\pi m} i. $$
在以 $\xi$ 为中心、半径为 $|\xi|$ 的圆盘内，以下展开式是有效的
$$
\begin{aligned}
x^{s-1} e^{-2\pi i m x} &= \xi^{s-1} e^{-2\pi i m \xi} e^{(s-1) \{ -\frac{1}{2} (\frac{x-\xi}{\xi})^2 + \frac{1}{3} (\frac{x-\xi}{\xi})^3 - \dots \}} \\
&= \xi^{s-1} e^{-2\pi i m \xi} e^{-\frac{s-1}{2\xi^2} (x-\xi)^2} \{ c_0 + c_1 (x-\xi) + c_2 (x-\xi)^2 + \dots \};
\end{aligned}
$$
并且级数
$$ \xi^{s-1} e^{-2\pi i m \xi} \sum_{n=0}^{\infty} c_n \int_{C_1} \frac{e^{-\frac{s-1}{2\xi^2} (x-\xi)^2}}{e^{2\pi i x} - 1} (x-\xi)^n dx $$
给出了 (8) 中积分的一个可能的渐近展开。如果 $\frac{s-1}{2\xi^2}$ 取特殊值 $\pi i$，级数中出现的积分现在都可以通过 § 1 的公式 (6) 来计算。对于固定的 $s$，这是对 $m$ 的一个条件，一般来说，由于 $m$ 是整数，这个条件只能近似满足。这就是为什么黎曼用邻近值 $\eta$ 替换鞍点 $\xi$，根据方程
$$ \frac{ti}{2\eta^2} = \pi i $$
得到
$$ (10) \quad \eta = + \sqrt{\frac{t}{2\pi}} $$
然后按照 (9) 的建议，确定 $m$ 为小于 $\frac{t}{2\pi \eta}$ 的最大整数，所以
$$ (11) \quad m = [\eta]. $$

现在引入缩写
$$ (12) \quad \tau = +\sqrt{t} = \eta \sqrt{2\pi} $$
$$ \varepsilon = e^{-\frac{\pi i}{4}} = \frac{1-i}{\sqrt{2}} $$
$$ g(x) = x^{s-1} \frac{e^{-2\pi i m x}}{e^{2\pi i x} - 1} $$

暂时设 $\eta$ 不是整数。积分路径 $C_1$ 将被折线 $C_2$ 取代，该折线由从点 $\eta - \frac{\varepsilon}{2}\eta$ 出发的两条半直线组成，分别包含点 $\eta$ 和 $-(m + \frac{1}{2})$。考虑到极点 $\pm 1, \pm 2, \dots, \pm m$，由留数定理可得

$$ \int_{C_1} g(x) dx = (e^{\pi i s} - 1) \sum_{n=1}^{m} n^{s-1} + \int_{C_2} g(x) dx $$

$$ (13) \quad \zeta(s) = \sum_{n=1}^{m} n^{-s} + \frac{(2\pi)^s}{2\Gamma(s) \cos \frac{\pi s}{2}} \sum_{n=1}^{m} n^{s-1} + \frac{(2\pi)^s e^{\frac{\pi i s}{2}}}{\Gamma(s) (e^{2\pi i s} - 1)} \int_{C_2} g(x) dx. $$

在 $C_2$ 的两个直线段中位于左侧的那一段（我们将之命名为 $C_3$）上，现在有
$$ \arg x \ge \arctan \frac{1}{2\sqrt{2}-1} > (2\sqrt{2}-1)^{-1} - \frac{1}{3} (2\sqrt{2}-1)^{-3} > \frac{1}{2\sqrt{2}} + \frac{1}{8} $$
$$ \mathfrak{I}(x) \le \frac{\eta}{2\sqrt{2}} $$
因此根据 (10) 和 (11)
$$ |x^{s-1} e^{-2\pi i m x}| \le |x|^{\sigma-1} e^{-t \left( \frac{1}{2\sqrt{2}} + \frac{1}{8} \right) + \pi m \frac{\eta}{2\sqrt{2}}} \le |x|^{\sigma-1} e^{-\frac{t}{8}} $$

$$ (14) \quad \int_{C_3} g(x) dx = O \left( e^{-\frac{t}{9}} \right), $$

对于 $\sigma_1 \le \sigma \le \sigma_2$ 关于 $\sigma$ 一致成立。
在 $C_2$ 的右侧半直线上，令
$$ x = \eta + \varepsilon y \quad (y \ge -\frac{\eta}{2}); $$
那么我们有
$$ |x^{s-1} e^{-2\pi i m x}| = |x|^{\sigma-1} e^{-t \arctan \frac{y}{y + \eta\sqrt{2}} - \pi\sqrt{2} m y}. $$
即使 $y \ge +\frac{\eta}{2}$ 这也是成立的，所以对于足够大的 $t$ 有
$$
\begin{aligned}
t \arctan \frac{y}{y + \eta\sqrt{2}} - \pi\sqrt{2} m y &\le \frac{ty}{y + \eta\sqrt{2}} - \pi\sqrt{2} m y < ty \left( \frac{1}{y + \eta\sqrt{2}} - \frac{\eta - 1}{\sqrt{2} \eta^2} \right) \\
&= \frac{ty}{\eta\sqrt{2}} \left( \frac{1}{\eta} - \frac{y}{y + \eta\sqrt{2}} \right) \le \frac{t}{2\sqrt{2}} \left( \frac{1}{\eta} - \frac{1}{1 + 2\sqrt{2}} \right) < - \frac{t}{11};
\end{aligned}
$$
所以我们有估计
$$ (15) \quad \int_{\frac{\eta}{2}}^{\infty} g(x) \varepsilon dy = O \left( e^{-\frac{t}{11}} \right), $$
这特别地再次对于 $\sigma_1 \le \sigma \le \sigma_2$ 关于 $\sigma$ 一致成立。由 (14) 和 (15) 得到
$$ (16) \quad \int_{C_2} g(x) dx = \int_{\eta - \varepsilon \frac{\eta}{2}}^{\eta - \varepsilon \frac{\eta}{2}} g(x) dx + O \left( e^{-\frac{t}{11}} \right). $$
为了对 (16) 右侧的积分进行渐近展开，我们要从恒等式
$$ (17) \quad g(x) = \eta^{s-1} e^{-2\pi i m \eta} \frac{e^{-\pi i (x-\eta)^2 + 2\pi i (\eta-m) (x-\eta)}}{e^{2\pi i x} - 1} e^{(s-1) \log (1 + \frac{x-\eta}{\eta}) - 2\pi i \eta (x-\eta) + \pi i (x-\eta)^2} $$
出发。
对于 $|x-\eta| < \eta$，右侧因子的最后一项可以展开为 $x-\eta$ 的幂级数，其系数需要更详细地研究。利用 (12) 中 $\tau$ 的定义，令
$$ (18) \quad e^{(s-1) \log (1 + \frac{z}{\tau}) - i \tau z + \frac{1}{2} z^2} = \sum_{n=0}^{\infty} a_n z^n = w(z) \quad (|z| < \tau). $$
由微分方程
$$ (z+\tau) \frac{dw}{dz} + (1 - \sigma - i z^2) w = 0 $$
得出递推公式
$$ (19) \quad (n+1) \tau a_{n+1} = -(n + 1 - \sigma) a_n + i a_{n-2} \quad (n = 2, 3, \dots), $$
这也适用于 $n=0, 1$，只要设定 $a_{-2}=0, a_{-1}=0$。如果再加上方程 $a_0=1$，那么 $a_1, a_2, \dots$ 就由 (19) 确定了；特别地，$a_n$ 是 $\tau^{-1}$ 的 $n$ 次多项式，其中不包含幂 $\tau^{-k}$ 对于 $k = 0, 1, \dots n - 2[\frac{n}{3}] - 1$。因此
$$ a_n = O \left( t^{-\frac{n}{2} + [\frac{n}{3}]} \right) $$
对于 $\sigma_1 \le \sigma \le \sigma_2$ 关于 $\sigma$ 是一致成立的，但关于 $n$ 稍显不一致。
为了估计幂级数 $w(z)$ 的尾部，利用表示式
$$ (20) \quad r_n(z) = \sum_{k=n}^{\infty} a_k z^k = \frac{1}{2\pi i} \int_{C} \frac{w(u) z^n}{u^n (u-z)} du; $$
其中 $C$ 是位于收敛圆内的一条曲线，它正向环绕点 $0$ 和 $z$ 各一次。由 (18) 我们有
$$
\begin{aligned}
\log w(u) &= (\sigma - 1 + i\tau^2) \log (1 + \frac{u}{\tau}) - i\tau u + \frac{i}{2} u^2 \\
&= (\sigma - 1) \log (1 + \frac{u}{\tau}) + i u^2 \sum_{k=1}^{\infty} \frac{(-1)^{k-1}}{k+2} \left( \frac{u}{\tau} \right)^k;
\end{aligned}
$$

因此，在圆 $|u| \le \frac{3}{5}\tau$ 内有效，我们有估计
$$ (21) \quad \Re \log w(u) \le |\sigma - 1| \log \frac{5}{2} + \frac{5}{6} \frac{|u|}{\tau} |u|^2. $$
在 (20) 中，设定 $|z| \le \frac{4}{7}\tau$，并设 $C$ 为围绕 $u=0$ 半径为 $\varrho_n$ 的圆，目前，该半径仅需满足条件
$$ (22) \quad \frac{21}{20} |z| \le \varrho_n \le \frac{3}{5}\tau $$
从 (20), (21), (22) 随后得到关于 $\sigma$ 和 $n$ 一致的估计
$$ (23) \quad r_n(z) = O \left( |z|^n \varrho_n^{-n} e^{\frac{5}{6\tau} \varrho_n^3} \right). $$
关于 $\varrho$ 的函数 $\varrho^{-n} e^{\frac{5}{6\tau} \varrho^3}$ 在 $\varrho = (\frac{2n\tau}{5})^{\frac{1}{3}}$ 处取得最小值 $(\frac{5e}{2n\tau})^{\frac{n}{3}}$。由 (22)，在这种情况下选择 $\varrho_n = \varrho$ 是允许的
$$ \frac{21}{20} |z| \le \left( \frac{2n\tau}{5} \right)^{\frac{1}{3}} \le \frac{3}{5}\tau $$
因此，我们有
$$ (24) \quad r_n(z) = O \left( |z|^n \left( \frac{5e}{2n\tau} \right)^{\frac{n}{3}} \right) \quad \left( n \le \frac{27}{50} t, |z| \le \frac{20}{21} \left( \frac{2n\tau}{5} \right)^{\frac{1}{3}} \right). $$
对于 $|z| \le \frac{4}{7}\tau$，根据 (22)，选择 $\varrho_n = \frac{21}{20}|z|$ 也是允许的；这时 (23) 给出关系
$$ (25) \quad r_n(z) = O \left( \left( \frac{20}{21} \right)^n e^{\frac{5}{6\tau} (\frac{21}{20}|z|)^3} \right) = O \left( e^{\frac{14}{29} |z|^2} \right) \quad \left( |z| \le \frac{\tau}{2} \right). $$

由 (17) 和 (18) 可得
$$ (26) \quad \int_{\eta - \varepsilon \frac{\eta}{2}}^{\eta - \varepsilon \frac{\eta}{2}} g(x) dx = \eta^{s-1} e^{-2\pi i m \eta} \int_{\eta - \varepsilon \frac{\eta}{2}}^{\eta - \varepsilon \frac{\eta}{2}} \frac{e^{-\pi i (x-\eta)^2 + 2\pi i (\eta-m) (x-\eta)}}{e^{2\pi i x} - 1} w \left( \sqrt{2\pi} (x-\eta) \right) dx. $$
为了确定如果在该方程中用部分和 $\sum_{k=0}^{n-1} a_k (2\pi)^{\frac{k}{2}} (x-\eta)^k$ 替换 $w \left( \sqrt{2\pi} (x-\eta) \right)$ 所产生的误差，必须考察积分
$$ (27) \quad J_n = \int_{\eta - \varepsilon \frac{\eta}{2}}^{\eta - \varepsilon \frac{\eta}{2}} \frac{e^{-\pi i (x-\eta)^2 + 2\pi i (\eta-m) (x-\eta)}}{e^{2\pi i x} - 1} r_n \left( \sqrt{2\pi} (x-\eta) \right) dx $$

从此以后设 $n \le \frac{5}{16} t$。如果我们将积分路径中位于圆盘 $|x-m| \le \frac{1}{2\sqrt{\pi}}$ 或 $|x-m-1| \le \frac{1}{2\sqrt{\pi}}$ 内的部分分别替换为相应的圆弧，那么将被积函数的极点 $x=m, m+1$ 的邻域避开了。如在 (24) 中一样，圆弧上的积分对 $J_n$ 仅提供贡献 $O \left( (\frac{5e}{2n\tau})^{\frac{n}{3}} \right)$。在积分路径的其余部分，我们有 $-\pi i (x-\eta)^2 = -\pi |x-\eta|^2$。令
$$ \frac{20}{21} \left( \frac{2n\tau}{5} \right)^{\frac{1}{3}} = \lambda $$
并考虑 (24) 对于 $|x-\eta| \le \frac{1}{\sqrt{2\pi}}$，或者另一方面 (25) 对于 $\frac{1}{\sqrt{2\pi}} \le |x-\eta| \le \frac{\eta}{2}$；那么随后有
$$
\begin{aligned}
J_n &= O \left\{ \left( \frac{5e}{2n\tau} \right)^{\frac{n}{3}} \int_{0}^{\lambda} e^{-\frac{1}{2}v^2} v^n dv + \int_{\lambda}^{\frac{\tau}{2}} e^{-\frac{1}{58} v^2} v^n dv \right\} \\
&= O \left\{ \left( \frac{5e}{2n\tau} \right)^{\frac{n}{3}} e^{\sqrt{2\pi n}} 2^{\frac{n}{2}} \Gamma \left( \frac{n+1}{2} \right) + e^{-\frac{1}{59} \lambda^2} \right\} = O \left\{ \left( \frac{25n}{4et} \right)^{\frac{n}{6}} e^{\sqrt{2\pi n}} + e^{-\frac{1}{59} \lambda^2} \right\}.
\end{aligned}
$$
一个简单的计算表明，对于 $n \le 2 \cdot 10^{-8} t$，第二个 $O$-项被第一个超过。这产生了估计
$$ (28) \quad J_n = O \left( \left( \frac{3n}{t} \right)^{\frac{n}{6}} \right) \quad (n \le 2 \cdot 10^{-8} t) $$
关于 $\sigma$ 和 $n$ 是一致的。
从 (16), (18), (26), (27), (28) 现在可以得出
$$
\begin{aligned}
\int_{C_2} g(x) dx &= \eta^{s-1} e^{-2\pi i m \eta} \left\{ \sum_{k=0}^{n-1} a_k (2\pi)^{\frac{k}{2}} \int_{\eta - \varepsilon \frac{\eta}{2}}^{\eta - \varepsilon \frac{\eta}{2}} \frac{e^{-\pi i (x-\eta)^2 + 2\pi i (\eta-m) (x-\eta)}}{e^{2\pi i x} - 1} (x-\eta)^k dx + O \left( \left( \frac{3n}{t} \right)^{\frac{n}{6}} \right) \right\}.
\end{aligned}
$$
如果在右侧不是在 $\eta + \varepsilon \frac{\eta}{2}$ 到 $\eta - \varepsilon \frac{\eta}{2}$ 上积分，而是在整条直线 $\eta + \varepsilon \infty$ 到 $\eta - \varepsilon \infty$ 上积分，那么，因为 $n \le 2 \cdot 10^{-8} t$ [英译者注：Red Herring? / 转移注意力的东西？]，积分的值 [英译者注：$\int_{C_2} g(x) dx$] 仅改变 $O \left( e^{-\frac{1}{8} \pi \eta (\frac{\eta}{2})^k} \right)$；另一方面，根据 (24)

$$ a_k = (r_k - r_{k+1}) z^{-k} = O \left( \left( \frac{5e}{2k\tau} \right)^{\frac{k}{3}} \right) \quad (k = 1, 2, \dots, n-1), $$
所以
$$ \sum_{k=0}^{n-1} |a_k| e^{-\frac{1}{8}\pi \eta} \left( \frac{\eta}{2} \right)^k = O \left( e^{-\frac{1}{8}\pi \eta} \left( \frac{5et}{16n} \right)^{\frac{n}{3}} \right) = O \left( \left( \frac{3n}{t} \right)^{\frac{n}{6}} \right). $$
最后，将积分变量 $x$ 替换为 $x+m$，使得
$$ (29) \quad \int_{C_2} g(x) dx = (-1)^m e^{-\frac{\pi i}{8}} \eta^{s-1} e^{-\pi i \eta^2} \left\{ \sum_{k=0}^{n-1} a_k (2\pi)^{\frac{k}{2}} \int_{0 \nwarrow 1} \frac{e^{\pi i \left( x^2 - 2(x+m-\eta)^2 + \frac{1}{8} \right)}}{e^{2\pi i x} - 1} (x + m - \eta)^k dx + O \left( \left( \frac{3n}{t} \right)^{\frac{n}{6}} \right) \right\}. $$
根据 § 1 的结果，积分
$$ (30) \quad \int_{0 \nwarrow 1} \frac{e^{\pi i \left( x^2 - 2\left( x - \frac{\delta}{\sqrt{2\pi}} - \frac{1}{2} \right)^2 + \frac{1}{8} \right)}}{e^{2\pi i x} - 1} dx = F(\delta) $$
的值为
$$ F(u) = \frac{\cos(u^2 + \frac{3\pi}{8})}{\cos(\sqrt{2\pi} u)}. $$
为了也以初等的方式表示 (29) 中出现的 $k > 0$ 的右侧积分，黎曼从 (30) 构造方程
$$ F(\delta + u) e^{i u^2} = \int_{0 \nwarrow 1} \frac{e^{\pi i \left( x^2 - 2\left( x - \frac{\delta}{\sqrt{2\pi}} - \frac{1}{2} \right)^2 + \frac{1}{8} \right)}}{e^{2\pi i x} - 1} e^{2\sqrt{2\pi} i \left( x - \frac{\delta}{\sqrt{2\pi}} - \frac{1}{2} \right) u} dx, $$
从中他通过关于 $u$ 的幂级数展开，得到了公式
$$ (31) \quad \int_{0 \nwarrow 1} \frac{e^{\pi i \left( x^2 - 2\left( x - \frac{\delta}{\sqrt{2\pi}} - \frac{1}{2} \right)^2 + \frac{1}{8} \right)}}{e^{2\pi i x} - 1} \left( x - \frac{\delta}{\sqrt{2\pi}} - \frac{1}{2} \right)^k dx = 2^{-k} (2\pi)^{-\frac{k}{2}} k! \sum_{r=0}^{[\frac{k}{2}]} \frac{i^{r-k}}{r!(k-2r)!} F^{(k-2r)}(\delta) \quad (k = 0, 1, 2, \dots) $$

现在，由 (13), (29), (31) 得到展开式
$$ (32) \quad \zeta(s) = \sum_{l=1}^{m} l^{-s} + \frac{(2\pi)^s}{2\Gamma(s) \cos \frac{\pi s}{2}} \sum_{l=1}^{m} l^{s-1} + (-1)^{m-1} \frac{(2\pi)^{\frac{s+1}{2}}}{\Gamma(s)} t^{\frac{s-1}{2}} e^{\frac{\pi i s}{2} - \frac{ti}{2} - \frac{\pi i}{8}} S $$

其中
$$ (33) \quad S = \sum_{0 \le 2r \le k \le n-1} \frac{2^{-k} i^{r-k} k!}{r! (k-2r)!} a_k F^{(k-2r)}(\delta) + O \left( \left( \frac{3n}{t} \right)^{\frac{n}{6}} \right) $$
$$ n \le 2 \cdot 10^{-8} t, \quad \delta = \sqrt{t} - \left( m + \frac{1}{2} \right) \sqrt{2\pi}, \quad F(u) = \frac{\cos(u^2 + \frac{3\pi}{8})}{\cos(\sqrt{2\pi} u)} $$
并且系数 $a_k$ 由递推公式 (19) 确定。这个展开式是渐近的，并且特别地对于 $\sigma_1 \le \sigma \le \sigma_2$ 是一致的，因为 (33) 中的余项确实对于每个固定的 $n$，一致地关于 $\sigma$ 是 $t^{-\frac{n}{6}}$ 阶的。与分析中已知的渐近级数相比，(32) 本身的不同之处在于整数 $m$ 的出现，这导致展开式的各项不连续地依赖于 $t$。在证明中所做的假设 $\sqrt{\frac{t}{2\pi}}$ 不是整数，随后很容易消除，因为人们确实可以在 $\sqrt{\frac{t}{2\pi}}$ 的任何整数值处进行 (32) 中的右边界交叉。

如果我们在 (33) 中选择特殊值 $n = 2 \cdot 10^{-8} t$，误差项为 $O \left( 10^{-10^{-8} t} \right)$，因此随着 $t$ 的增加呈指数级趋于 0。对于实际目的，由于极小的指数因子 $10^{-8}$，这个误差项的估计是没有用的；更精细的估计表明，$10^{-8}$ 可以被相当大的数代替。找到作为 $n$ 的函数的误差增长的确切阶数将会很有趣；但这不是平凡的，因为它对于固定的 $t$ 并不随着 $n$ 的增加而收敛到 0。

由于 $\sigma = \frac{1}{2}$ 的情况特别重要，将 (32) 乘以函数 $e^{\vartheta i}$ 是适宜的，该函数定义为
$$ (34) \quad e^{\vartheta i} = \pi^{\frac{s}{2} - \frac{1}{4}} \sqrt{\frac{\Gamma(\frac{s}{2})}{\Gamma(\frac{1-s}{2})}} $$
我们用 $\vartheta$ 表示在从 $0$ 到 $-\infty$ 以及从 $1$ 到 $+\infty$ 切开的平面上唯一确定的分支的值，它在 $s = \frac{1}{2}$ 时消失。那么，在临界线 $\sigma = \frac{1}{2}$ 上，$\vartheta = \arg (\pi^{-\frac{s}{2}} \Gamma(\frac{s}{2}))$ 且 $e^{\vartheta i} \zeta(s)$ 是实数。接着 (32)，对于 $\sigma_1 \le \sigma \le \sigma_2$
$$ (35) \quad e^{\vartheta i} \zeta(s) = 2 \sum_{l=1}^{m} \frac{\cos(\vartheta + i(s-\frac{1}{2}) \log l)}{\sqrt{l}} + (-1)^{m-1} \left( \frac{t}{2\pi} \right)^{\frac{\sigma-1}{2}} e^{i(\frac{t}{2} \log \frac{t}{2\pi} - \frac{t}{2} - \frac{\pi}{8} - \vartheta) t} S, $$
其中 $S$ 由 (33) 定义。$S$ 的有限和中包含的每个 $a_k$ 都是 $\tau^{-1}$ 的多项式。因此从 (33) 推出，对于每个固定的 $n$ 和 $t \to \infty$，通过按 $\tau^{-1}$ 的幂重新排序，我们有关系
$$ S = \sum_{k=0}^{n-1} A_k \tau^{-k} + O(\tau^{-n}), $$
其中系数 $A_0, A_1, \dots, A_{n-1}$ 是导数 $F'(\delta), F''(\delta), \dots$ 的有限数量的齐次线性组合。借助 (33) 和 $a_k$ 的递推公式显式计算 $A_k$ 相当繁琐；黎曼通过以下技巧简化了这一点。代入
$$ F(\delta+x) e^{ix^2} = \sum_{k=0}^{\infty} b_k x^k, $$
那么
$$ (36) \quad S \sim \sum_{k=0}^{\infty} (2i)^{-k} k! a_k b_k $$
是一个完全的渐近级数，所需的量 $A_k$ 是 $\tau^{-k}$ 的系数，它通过按 $\tau^{-1}$ 的幂排列级数而产生。(36) 右侧的和不过是 $x$ 的正负幂级数中的常数项，该级数通过形式乘法产生
$$ F \left( \delta + \frac{1}{x} \right) e^{i x^{-2}} = \sum_{k=0}^{\infty} b_k x^{-k} $$
与发散幂级数
$$ (37) \quad y = \sum_{k=0}^{\infty} (2i)^{-k} k! a_k x^k. $$
由于固定的幂 $\tau^{-k}$ 仅出现在有限数量的系数 $a_0, a_1, a_2, \dots$ 中，因此以下计算 $A_k$ 的方法是合理的：通过 $e^{i x^{-2}}$ 和 $y$ 的形式乘法构造项
$$ (38) \quad z = e^{i x^{-2}} y = \sum_{n=-\infty}^{\infty} d_n x^n $$
由此，通过按 $\tau^{-1}$ 的幂排序，级数 $\sum_{k=0}^{\infty} B_k \tau^{-k}$；那么 $A_k$ 就是 $F(\delta + \frac{1}{x}) B_k$ 中的常数项。为了计算这个常数项，$B_k$ 中出现的 $x$ 的负幂是无关紧要的，所以只需确定 $B_k$ 的多项式部分。

如果，为了简便，设定
$$ (2i)^{-k} k! a_k = c_k \quad (k=0, 1, 2, \dots), $$
那么，由 (19)
$$ \tau c_{n+1} = i \frac{n+1-\sigma}{2} c_n - \frac{n(n-1)}{8} c_{n-2} \quad (n=0, 1, 2, \dots) $$
其中 $c_{-2}=0, c_{-1}=0, c_0=1$，因此幂级数 (37) 形式上满足微分方程
$$ \tau(y-1) = \frac{i}{2} x^{\sigma+1} D (x^{1-\sigma} y) - \frac{1}{8} x^3 D^2 (x^2 y). $$
对于级数 (38) 得到微分方程
$$ (39) \quad \left\{ \tau + \frac{1}{2x} + i \left( \frac{\sigma}{2} - \frac{1}{4} \right) x \right\} z + \frac{1}{8} x^3 D^2 (x^2 z) = \tau e^{i x^{-2}}. $$
如果现在，按 $\tau^{-1}$ 的幂排序，
$$ z = \sum_{n=0}^{\infty} B_n \tau^{-n}, $$
那么由 (39) 推出
$$ B_0 = e^{i x^{-2}} $$
以及递推公式
$$ B_{n+1} = \left( i \frac{1-2\sigma}{4} x - \frac{1}{2x} \right) B_n - \frac{1}{8} x^3 D^2 (x^2 B_n) \quad (n=0, 1, 2, \dots). $$
如果现在设定
$$ B_n = \sum_{k=-\infty}^{3n} a_k^{(n)} x^k \quad (n=0, 1, 2, \dots), $$
那么有
$$ a_k^{(0)} = 0 \quad (k \ne 0, -2, -4, -6, \dots) $$
$$ a_{-2k}^{(0)} = \frac{i^k}{k!} \quad (k=0, 1, 2, 3, \dots) $$
$$ (40) \quad a_k^{(n+1)} = i \frac{1-2\sigma}{4} a_{k-1}^{(n)} - \frac{1}{2} a_{k+1}^{(n)} - \frac{(k-1)(k-2)}{8} a_{k-3}^{(n)} \quad (n=0, 1, 2, \dots; k=0, \pm 1, \pm 2, \dots). $$
借助这些用于计算 $a_k^{(n)}$ 的递推公式，那么 $A_n$ 可以被显式指定，即
$$ (41) \quad A_n = \sum_{k=0}^{3n} \frac{a_k^{(n)}}{k!} F^{(k)}(\delta); $$

这得出
$$ S \sim \sum \frac{a_k^{(n)}}{k!} F^{(k)}(\delta) \tau^{-n}, $$
其中 $n$ 取值 $0, 1, 2, \dots$，而 $k$ 取值 $0, 1, 2, \dots, 3n$。
递推公式 (40) 对于 $\sigma = \frac{1}{2}$ 最为简单。对于这个特例，很容易得到
$$ B_0 = 1 + \dots $$
$$ B_1 = -\frac{1}{2^2} x^3 + \dots $$
$$ B_2 = \frac{5}{2^4} x^6 + \frac{1}{2^2} x^2 + \frac{1}{2^4 \cdot 3} + \dots $$
$$ B_3 = -\frac{5 \cdot 7}{2^6} x^9 - \frac{1}{2^5} x^5 - \frac{1}{2^6 \cdot 3} x^3 - \frac{1}{2^4} x + \dots $$
$$ B_4 = \frac{5^2 \cdot 7 \cdot 11}{2^9} x^{12} + \frac{7 \cdot 11}{2^4} x^8 + \frac{51}{2^7 \cdot 3} x^6 + \frac{19}{2^6} x^4 + \frac{1}{3 \cdot 2^7} x^2 + \frac{11 \cdot 13}{2^9 \cdot 3^2} + \dots; $$
其中省略的加项仅包含 $x$ 的负幂。因此，对于 $\sigma = \frac{1}{2}$
$$
(42) \quad \left\{
\begin{aligned}
A_0 &= F(\delta) \\
A_1 &= -\frac{1}{2^3 \cdot 3} F^{(3)}(\delta) \\
A_2 &= \frac{1}{2^7 \cdot 3^2} F^{(6)}(\delta) + \frac{1}{2^4} F^{(2)}(\delta) + \frac{1}{2^4 \cdot 3} F(\delta) \\
A_3 &= -\frac{1}{2^{10} \cdot 3^4} F^{(9)}(\delta) - \frac{1}{2^4 \cdot 3 \cdot 5} F^{(5)}(\delta) - \frac{1}{2^7 \cdot 3^2} F^{(3)}(\delta) - \frac{1}{2^4} F^{(1)}(\delta) \\
A_4 &= \frac{1}{2^{15} \cdot 3^5} F^{(12)}(\delta) + \frac{11}{2^{11} \cdot 3^2 \cdot 5} F^{(8)}(\delta) + \frac{1}{2^{11} \cdot 3^3} F^{(6)}(\delta) \\
&\quad + \frac{19}{2^9 \cdot 3} F^{(4)}(\delta) + \frac{1}{2^8 \cdot 3} F^{(2)}(\delta) + \frac{11 \cdot 13}{2^9 \cdot 3^2} F(\delta);
\end{aligned}
\right.
$$
因此，在 $\sigma = \frac{1}{2}$ 的情况下，$S$ 被确定到了 $\tau^{-5}$ 阶的误差。
如果借助斯特林级数（Stirling's series）渐近地展开右侧第二项中的量 $\vartheta$，渐近展开式 (35) 还可以进一步简化。为此，黎曼考虑公式
$$ \log \Gamma \left( \frac{1}{4} + \frac{ti}{2} \right) = \left( \frac{ti}{2} - \frac{1}{4} \right) \log \frac{ti}{2} - \frac{ti}{2} + \log \sqrt{2\pi} + \frac{1}{4} \int_{0}^{\infty} \left( \frac{4e^{3x}}{e^{4x} - 1} - \frac{1}{x} - 1 \right) \frac{e^{-2tix}}{x} dx \quad (t > 0), $$
这是由 $\log \Gamma(s)$ 著名的 Binet 积分表示通过简单的变换得到的。
由于恒等式
$$ \frac{4e^{3x}}{e^{4x} - 1} = \frac{1}{\cosh x} + \frac{1}{\sinh x} $$
通过分离实部和虚部可得
$$ \log \left| \Gamma \left( \frac{1}{4} + \frac{ti}{2} \right) \right| = -\frac{\pi}{4} t - \frac{1}{4} \log \frac{t}{2} + \log \sqrt{2\pi} + \frac{1}{4} \int_{0}^{\infty} \left( \frac{1}{\cos x} - 1 \right) \frac{e^{-2tx}}{x} dx - \frac{1}{4} \log (1 + e^{-2\pi t}) $$
$$ \arg \Gamma \left( \frac{1}{4} + \frac{ti}{2} \right) = \frac{t}{2} \log \frac{t}{2} - \frac{t}{2} - \frac{\pi}{8} + \frac{1}{4} \int_{0}^{\infty} \left( \frac{1}{\sin x} - \frac{1}{x} \right) \frac{e^{-2tx}}{x} dx + \frac{1}{2} \arctan e^{-\pi t}, $$
其中，由于在 $k\frac{\pi}{2} (k=1, 2, \dots)$ 处的极点，积分应被理解为柯西主值。如果设定
$$ \frac{1}{\cos x} = \sum_{n=0}^{\infty} \frac{E_n}{(2n)!} x^{2n} \quad (|x| < \frac{\pi}{2}) $$
$$ \frac{x}{\sin x} = \sum_{n=0}^{\infty} \frac{F_n}{(2n)!} x^{2n} \quad (|x| < \pi), $$
那么 $E_0=1, E_1=1, E_2=5, E_3=61, F_0=1, F_1=\frac{1}{3}, F_2=\frac{7}{15}, F_3=\frac{31}{21}$ 且一般地
$$ E_n - \binom{2n}{2} E_{n-1} + \binom{2n}{4} E_{n-2} - \dots + (-1)^n E_0 = 0 \quad (n=1, 2, 3, \dots) $$
$$ \binom{2n+1}{1} F_n - \binom{2n+1}{3} F_{n-1} + \binom{2n+1}{5} F_{n-2} - \dots + (-1)^n F_0 = 0 \quad (n=1, 2, 3, \dots). $$

这就以众所周知的方式提供了渐近级数
$$ (43) \quad \log \left| \Gamma \left( \frac{1}{4} + \frac{ti}{2} \right) \right| \sim -\frac{\pi}{4} t - \frac{1}{4} \log \frac{t}{2} + \log \sqrt{2\pi} + \frac{1}{8} \sum_{n=1}^{\infty} \frac{E_n}{n} (2t)^{-2n} $$
$$ \arg \Gamma \left( \frac{1}{4} + \frac{ti}{2} \right) \sim \frac{t}{2} \log \frac{t}{2} - \frac{t}{2} - \frac{\pi}{8} + \frac{1}{8} \sum_{n=1}^{\infty} \frac{F_n}{n(2n-1)} (2t)^{1-2n}. $$
在 $\sigma = \frac{1}{2}$ 上，现在有 $\vartheta = -\frac{1}{2} \log \pi + \arg \Gamma(\frac{1}{4} + \frac{ti}{2})$，因此
$$ \frac{t}{2} \log \frac{t}{2\pi} - \frac{t}{2} - \frac{\pi}{8} - \vartheta \sim -\frac{1}{8} \sum_{n=1}^{\infty} \frac{F_n}{n(2n-1)} (2t)^{1-2n} $$
$$ e^{i(\frac{t}{2} \log \frac{t}{2\pi} - \frac{t}{2} - \frac{\pi}{8} - \vartheta) t} = 1 - \frac{i}{2^4 \cdot 3} t^{-1} - \frac{1}{2^9 \cdot 3^2} t^{-2} + O(t^{-3}). $$

考虑到 (42)，我们现在有，作为 $\sigma = \frac{1}{2}$ 时 $\zeta(s)$ 渐近级数的明确形式，方程
$$ (44) \quad e^{\vartheta i} \zeta \left( \frac{1}{2} + ti \right) = 2 \sum_{n=1}^{m} \frac{\cos(\vartheta - t \log n)}{\sqrt{n}} + (-1)^{m-1} \left( \frac{t}{2\pi} \right)^{-\frac{1}{4}} R $$
其中
$$ \vartheta = -\frac{t}{2} \log \pi + \arg \Gamma \left( \frac{1}{4} + \frac{ti}{2} \right) $$
$$ m = \left[ \sqrt{\frac{t}{2\pi}} \right] $$
$$ R \sim C_0 + C_1 t^{-\frac{1}{2}} + C_2 t^{-1} + C_3 t^{-\frac{3}{2}} + C_4 t^{-2} + \dots $$
$$
(45) \quad \left\{
\begin{aligned}
C_0 &= F(\delta) \\
C_1 &= -\frac{1}{2^3 \cdot 3} F^{(3)}(\delta) \\
C_2 &= \frac{1}{2^4} F^{(2)}(\delta) + \frac{1}{2^7 \cdot 3^2} F^{(6)}(\delta) \\
C_3 &= -\frac{1}{2^4} F^{(1)}(\delta) - \frac{1}{2^4 \cdot 3 \cdot 5} F^{(5)}(\delta) - \frac{1}{2^{10} \cdot 3^4} F^{(9)}(\delta) \\
C_4 &= \frac{1}{2^5} F(\delta) + \frac{19}{2^9 \cdot 3} F^{(4)}(\delta) + \frac{11}{2^{11} \cdot 3^2 \cdot 5} F^{(8)}(\delta) + \frac{1}{2^{15} \cdot 3^5} F^{(12)}(\delta) \\
F(x) &= \frac{\cos(x^2 + \frac{3\pi}{8})}{\cos(\sqrt{2\pi} x)} \\
\delta &= \sqrt{t} - \left( m + \frac{1}{2} \right) \sqrt{2\pi},
\end{aligned}
\right.
$$

[译者注： （44）和（45）即为黎曼-西格尔公式]

基本上可以在黎曼那里找到上述内容。前文中唯一的新贡献是余项估计。
人们现在可以放弃条件 $\sigma = \frac{1}{2}$ 以及 $\sigma$ 仅限于区间 $\sigma_1 \le \sigma \le \sigma_2$ 的限制，并且仍然可以使用渐近展开式 (44)；那时人们只需将 $t$ 理解为复数 $-i(s - \frac{1}{2})$，将 $m$ 理解为整数 $[\sqrt{|\frac{t}{2\pi}|}]$，而 $\vartheta$ 的含义仍然由 (34) 定义。证明这一断言所需的扩展可以毫无困难地从前面 (44) 的推导中获得。
渐近级数 $R$ 是量 $F(\delta), F'(\delta), F''(\delta), \dots$ 的齐次线性组合；通过重排，从中产生形式为
$$ D_0^* F(\delta) + D_1^* F'(\delta) + D_2^* F''(\delta) + \dots, $$
的表达式，其中每个 $D_n^*$ 都是 $\tau^{-1}$ 的幂级数。这些幂级数是发散的；这提出了一个问题：它们是否是某些解析函数 $D_0, D_1, D_2, \dots$ 的渐近展开式，以及级数
$$ (46) \quad D_0 F(\delta) + D_1 F'(\delta) + D_2 F''(\delta) + \dots $$
是否也是 $R$ 的一个渐近展开式。这个问题黎曼也处理过；并且再次没有必要的残差估计。但是，由于级数 (46) 因其较大的残余项而没有像原始渐近展开式那样的理论和实践重要性，随后的陈述中省略了对误差的相当费力的研究；也许这个 [陈述?] 更突显了黎曼的形式力量。

公式 (30)，它也可以写成形式
$$ \int_{m \nwarrow m+1} \frac{e^{-\pi i (x-\eta)^2 + 2\pi i (x-\eta)(\eta-m)}}{e^{2\pi i x} - 1} dx = F(\delta) e^{-\frac{\pi i}{8} - \pi i (\eta-m)^2} $$
允许反演
$$ (47) \quad \frac{2}{\sqrt{2\pi}} e^{-\frac{\pi i}{8} - \pi i (\eta-m)^2} \int_{0 \nwarrow 1} F(u+\delta) e^{i u^2 - 2\sqrt{2\pi} i (x-\eta) u} du $$
$$ = \frac{e^{-\pi i (x-\eta)^2 + 2\pi i (x-\eta)(\eta-m)}}{e^{2\pi i x} - 1}, $$
如果 $m < \Re(x) < m+1$。这可以通过应用傅里叶定理或通过过渡到 (5) 中的复共轭变量得到。从 (47) 随后得到
$$ (48) \quad \frac{e^{-2\pi i m x}}{e^{2\pi i x} - 1} = (-1)^m \frac{2}{\sqrt{2\pi}} e^{-\pi i x^2 - \frac{\pi i}{8}} \int_{0 \nwarrow 1} F(u+\delta) e^{i(u | \tau - \sqrt{2\pi} x)^2} du, $$
对于 $m < \Re(x) < m+1$ 也有效。直接将级数
$$ F(\delta) + \frac{F'(\delta)}{1!} u + \frac{F''(\delta)}{2!} u^2 + \dots $$
代入其中的 $F(u+\delta)$，并利用 (16) 中出现的积分
$$ \int_{\eta - \varepsilon \frac{\eta}{2}}^{\eta - \varepsilon \frac{\eta}{2}} g(x) dx = \int_{\eta - \varepsilon \frac{\eta}{2}}^{\eta - \varepsilon \frac{\eta}{2}} x^{s-1} \frac{e^{-2\pi i m x}}{e^{2\pi i x} - 1} dx $$
来计算该级数单个成员所提供的贡献。
通过这种方式我们找到渐近展开
$$ (49) \quad \int_{C_2} g(x) dx \sim (-1)^m \frac{2}{\sqrt{2\pi}} e^{-\frac{\pi i}{8}} \sum_{n=0}^{\infty} \frac{F^{(n)}(\delta)}{n!} \int_{m \nwarrow m+1} x^{s-1} e^{-\pi i x^2} \left\{ \int_{0 \nwarrow 1} u^n e^{i(u | \tau - \sqrt{2\pi} x)^2} du \right\} dx. $$
另一方面，根据 (13) 和 (44)
$$ (50) \quad \int_{C_2} g(x) dx = (-1)^m \left( \frac{t}{2\pi} \right)^{-\frac{1}{4}} e^{\vartheta i} R (1 - e^{\pi i s}). $$
现在，因为可以很容易地看出，将 $A_n$ 表示为 $F^{(k)}(\delta)$ 的常系数齐次线性函数（如 (41) 中给出）只有一种可能方式，从 (49) 和 (50) 推出方程
$$ (51) \quad n! D_n (1 - e^{\pi i s}) = \frac{2}{\sqrt{2\pi}} \left( \frac{t}{2\pi} \right)^{\frac{1}{4}} e^{-\vartheta i - \frac{\pi i}{8}} \int_{0 \nwarrow 1} x^{s-1} e^{-\pi i x^2} \left\{ \int_{0 \nwarrow 1} u^n e^{i(u | \tau - \sqrt{2\pi} x)^2} du \right\} dx \quad (n=0, 1, 2, \dots), $$
特别地，如果我们设定
$$ \frac{1}{\sqrt{2\pi}} \left( \frac{t}{2} \right)^{\frac{1}{4}} e^{\frac{\pi i}{4}} \sqrt{\Gamma \left( \frac{1}{4} + \frac{ti}{2} \right) \Gamma \left( \frac{1}{4} - \frac{ti}{2} \right)} = e^\omega $$
那么
$$ (52) \quad \left\{
\begin{aligned}
D_0 &= e^\omega \\
D_1 &= -\tau (e^\omega - e^{-\omega}) + \frac{\tau e^{\pi i s - \omega}}{1 - e^{\pi i s}} \sim -\tau (e^\omega - e^{-\omega}).
\end{aligned}
\right. $$
对于其余的 $D_n$，可以通过分部积分从 (51) 导出一个递推；但也可以无需额外计算通过以下方式获得。接着 (36), (37), (38)
$$ S \sim d_0 F(\delta) + \frac{d_1}{1!} F'(\delta) + \frac{d_2}{2!} F''(\delta) + \dots, $$
其中，由 (38) 和 (39)，$d_n$ 满足递推
$$ \tau d_n + \frac{1}{2} d_{n+1} + \frac{(n-1)(n-2)}{8} d_{n-3} = 0 \quad (n=1, 2, 3, \dots) $$
因为
$$ e^{(\frac{t}{2} \log \frac{t}{2\pi} - \frac{t}{2} - \frac{\pi}{8} - \vartheta) i} S = R $$
我们因此有 $D_n$ 的递推公式
$$ (53) \quad D_{n+1} = -\frac{2}{n+1} \tau D_n - \frac{1}{4n(n+1)} D_{n-3} \quad (n=1, 2, 3, \dots) $$

其中 $D_{-2} = 0, D_{-1} = 0$。由此借助 (52) 可导出值
$$
\begin{aligned}
D_2 &= -\tau D_1 \sim \tau^2 (e^\omega - e^{-\omega}) \\
D_3 &= -\frac{2}{3} \tau D_2 \sim -\frac{2}{3} \tau^3 (e^\omega - e^{-\omega}) \\
D_4 &= -\frac{1}{2} \tau D_3 - \frac{1}{2^4 \cdot 3} D_0 \sim \frac{1}{3} \tau^4 (e^\omega - e^{-\omega}) - \frac{1}{2^4 \cdot 3} e^\omega.
\end{aligned}
$$
$D_0, D_1, \dots$ 本身的渐近展开可以从 (43) 中获得；根据该公式，具体地
$$ \omega \sim \frac{1}{8} \sum_{n=1}^{\infty} \frac{E_n}{n} (2t)^{-2n} = \frac{1}{2^5} t^{-2} + \frac{5}{2^8} t^{-4} + \frac{61}{2^9 \cdot 3} t^{-6} + \dots. $$
将此代入 $D_0, \dots, D_4$ 的上述结果中，可得
$$ (54) \quad \left\{
\begin{aligned}
D_0 &\sim 1 + \frac{1}{2^5} \tau^{-4} + \frac{41}{2^{11}} \tau^{-8} + \dots \\
D_1 &\sim -\frac{1}{2^4} \tau^{-3} - \frac{5}{2^7} \tau^{-7} + \dots \\
D_2 &\sim \frac{1}{2^4} \tau^{-2} + \frac{5}{2^7} \tau^{-6} + \dots \\
D_3 &\sim -\frac{1}{2^3 \cdot 3} \tau^{-1} - \frac{5}{2^6 \cdot 3} \tau^{-5} + \dots \\
D_4 &\sim \frac{19}{2^9 \cdot 3} \tau^{-4} + \dots.
\end{aligned}
\right. $$
从递推关系 (53) 可以看出，$D_n$ 的渐近级数中出现的所有幂指数都 $\equiv n \pmod 4$。相应地，$C_n$ 中出现的 $F'(\delta)$ 的所有导数的阶数形式为 $3n - 4k$，这很容易在 $C_0, C_1, C_2, C_3, C_4$ 找到的表达式中得到证实。
如果写成
$$ R \sim \sum b_{kl} F^{(3l-4k)}(\delta) \tau^{-l}, $$
其中求和指标 $k$ 遍历值 $0, \dots, [\frac{3l}{4}]$，求和指标 $l$ 遍历值 $0, 1, \dots$，那么所有 $l \le 4$ 的 $b_{kl}$ 就被确定了，同时，根据 (54)，值 $b_{00}, b_{34}, b_{68}, b_{23}, b_{57}, b_{12}, b_{46}, b_{01}, b_{35}, b_{24}$ 是已知的；人们立刻可以看出，(45) 和 (54) 中同时出现的 $b_{00}, b_{34}, b_{23}, b_{12}, b_{01}, b_{24}$ 的值是一致的。
为了数值计算 $b_{kl}$，以及为了渐近级数的实际应用，按 $\tau^{-1}$ 的递增幂排序是首选。通过 (53) 确定 $D_n$ 实际上比前面处理的确定 $C_n$ 更费力；此外，连续的 $D_n$ 并没有单调递减的量级，而是 $D_{3n-2}, D_{3n-1}, D_{3n}$ 具有精确的阶数 $\tau^{-(n+2)}, \tau^{-(n+1)}, \tau^{-n}$，因此为了获得例如达到前一个误差 $O(\tau^{-5})$ 的精度，必须计算直到 $D_{12}$ 的 $D_5$。
过渡到 $D_n$ 是利用公式 (48) 完成的。如果人们试图从 (48) 获得 $\zeta(s)$ 的精确表达式而不仅仅是渐近级数，那么人们就会得出下一节将讨论的方法。

## $\S$ 3. Zeta 函数的积分表示

$\zeta(s)$ 渐近级数系数的显式确定是基于 § 1 的公式 (5)。借助该公式，黎曼推导出了 $\zeta(s)$ 的另一个相当有趣的表达式，该表达式在 1926 年之前似乎未被其他数学家注意到。
现在，设 $\sigma < 0$，并设 $u^{-s}$ 在从 $0$ 到 $-\infty$ 切开的 $u$ 平面上取主值。将 (5) 乘以 $u^{-s}$ 并沿着第一象限的角平分线从 $u=0$ 到 $e^{\frac{\pi i}{4}} \infty$ 进行积分。现在，如果设定缩写 $e^{\frac{\pi i}{4}} = \varepsilon$，
$$
\begin{aligned}
\int_{0}^{\varepsilon \infty} \frac{u^{-s}}{1 - e^{-2\pi i u}} du &= - \int_{0}^{\varepsilon \infty} u^{-s} \sum_{n=1}^{\infty} e^{2\pi i n u} du = - \sum_{n=1}^{\infty} \int_{0}^{\varepsilon \infty} u^{-s} e^{2\pi i n u} du \\
&= -\Gamma(1-s) \sum_{n=1}^{\infty} (2\pi n e^{-\frac{\pi i}{2}})^{s-1} \\
&= -(2\pi)^{s-1} e^{\frac{\pi i}{2}(1-s)} \Gamma(1-s) \zeta(1-s)
\end{aligned}
$$
并且
$$
\begin{aligned}
\int_{0}^{\varepsilon \infty} u^{-s} \left( \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2 + 2\pi i u x}}{e^{\pi i x} - e^{-\pi i x}} dx \right) du &= \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2}}{e^{\pi i x} - e^{-\pi i x}} \left( \int_{0}^{\varepsilon \infty} u^{-s} e^{2\pi i u x} du \right) dx \\
&= (2\pi)^{s-1} e^{\frac{\pi i}{2}(1-s)} \Gamma(1-s) \int_{0 \nwarrow 1} \frac{e^{-\pi i x^2} x^{s-1}}{e^{\pi i x} - e^{-\pi i x}} dx,
\end{aligned}
$$
所以由 (5)
$$ (55) \quad (2\pi)^{s-1} e^{\frac{\pi i}{2}(1-s)} \Gamma(1-s) \left\{ \zeta(1-s) + \int_{0 \nwarrow 1} \frac{x^{s-1} e^{-\pi i x^2}}{e^{\pi i x} - e^{-\pi i x}} dx \right\} + \int_{0}^{\varepsilon \infty} \frac{u^{-s} e^{\pi i u^2}}{e^{\pi i u} - e^{-\pi i u}} du = 0. $$
这里的第二个积分可以写成形式
$$ \frac{1}{e^{\pi i s} - 1} \int_{0 \swarrow 1} \frac{u^{-s} e^{\pi i u^2}}{e^{\pi i u} - e^{-\pi i u}} du $$
其中符号 $0 \swarrow 1$ 表示通过实轴反射从第一个积分产生的积分路径。将 (55) 乘以因子
$$ 2^{1-s} \pi^{-\frac{1-s}{2}} e^{\frac{\pi i}{2}(s-1)} \frac{\Gamma(\frac{1-s}{2})}{\Gamma(1-s)} $$
并考虑到关系
$$ \frac{2^{-s} \pi^{\frac{1-s}{2}} \Gamma(\frac{1-s}{2})}{\sin \frac{\pi s}{2} \Gamma(1-s)} = \pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right), $$
得到在整个 $s$ 平面上有效的公式
$$ (56) \quad \pi^{-\frac{1-s}{2}} \Gamma \left( \frac{1-s}{2} \right) \zeta(1-s) = \pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right) \int_{0 \swarrow 1} \frac{x^{-s} e^{\pi i x^2}}{e^{\pi i x} - e^{-\pi i x}} dx + \pi^{-\frac{1-s}{2}} \Gamma \left( \frac{1-s}{2} \right) \int_{0 \nwarrow 1} \frac{x^{s-1} e^{-\pi i x^2}}{e^{\pi i x} - e^{-\pi i x}} dx. $$

黎曼并不是将所有东西都写成这种对称形式；但这里选择的版本似乎对应用很方便。现在人们已经使 $\zeta(s)$ 的函数方程显而易见了；因为对于 $\sigma = \frac{1}{2}$，右侧的两项是复共轭的，所以 $\pi^{-\frac{s}{2}} \Gamma(\frac{s}{2}) \zeta(s)$ 在那里是实数，并且由于该函数对于 $\sigma > 1$ 是实数，所以根据对称原理，函数方程
$$ (57) \quad \pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right) \zeta(s) = \pi^{-\frac{1-s}{2}} \Gamma \left( \frac{1-s}{2} \right) \zeta(1-s) $$
适用于 $\sigma = \frac{1}{2}$ 并因此普遍适用于任何 $s$。
如果进一步设定
$$ (58) \quad \mathfrak{f}(s) = \int_{0 \swarrow 1} \frac{x^{-s} e^{\pi i x^2}}{e^{\pi i x} - e^{-\pi i x}} dx $$
$$ (59) \quad \varphi(s) = 2 \pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right) \mathfrak{f}(s) $$
那么由 (56) 和 (57)
$$ (60) \quad \pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right) \zeta(s) = \Re(\varphi(s)) \quad (\sigma = \frac{1}{2}); $$

这样一来，对临界线上 $\zeta(s)$ 的研究就简化为对 $\varphi(s)$ 实部的研究。

## $\S$ 4. 两个黎曼公式对 Zeta 函数理论的意义

根据方程 (32)，$\zeta(s)$ 渐近级数的主项是表达式
$$ \sum_{l=1}^{m} l^{-s} + \frac{(2\pi)^s}{\pi} \sin \frac{\pi s}{2} \Gamma(1-s) \sum_{l=1}^{m} l^{s-1} \quad \left( m = \left[ \sqrt{\frac{t}{2\pi}} \right] \right), $$
这也被哈代（Hardy）和李特尔伍德（Littlewood）发现了，但他们没有给出黎曼对 $S$ 的展开式，而只是给出了其绝对值的一个上界。他们还发现了主项的一种更一般的形式，即
$$ (61) \quad \sum_{l \le x} l^{-s} + \frac{(2\pi)^s}{\pi} \sin \frac{\pi s}{2} \Gamma(1-s) \sum_{l \le y} l^{s-1} $$
其中 $xy = \frac{t}{2\pi}$。这并非黎曼之前给出的；但可以想象，沿着黎曼的思路，人们可以毫无困难地得出表达式 (61) 的完整渐近展开式，该表达式对于由 (7) 定义的函数 $\Phi(\tau, u)$ 所起的作用，正如黎曼的特殊函数 $\Phi(-1, u)$ 所起的作用一样。

对于哈代和李特尔伍德已经利用他们的公式所做的应用，特别是用于估计位于区间 $0 < t < T$ 内 $\zeta(\frac{1}{2} + ti)$ 的零点数目 $N_0(T)$，黎曼公式给出了更精确的值，这似乎并不是一个更好的结果。然而，在上述提到的地方，黎曼声称 $N_0(T)$ 渐近等于 $\frac{T}{2\pi} \log \frac{T}{2\pi} - \frac{T}{2\pi}$，并因此渐近等于 $\zeta(s)$ 位于带状区域 $0 < t < T$ 内的所有零点的数目 $N(T)$，并且这可以借助他的新展开式来证明；但从他的遗稿中并不清楚他是否设计了这个证明。在 $\sigma = \frac{1}{2}$ 上有效的表示式
$$ (62) \quad e^{\vartheta i} \zeta \left( \frac{1}{2} + ti \right) = 2 \sum_{n=1}^{m} \frac{\cos(\vartheta - t \log n)}{\sqrt{n}} + O(t^{-\frac{1}{4}}) $$
$$ \vartheta = \frac{t}{2} \log \frac{t}{2\pi} - \frac{t}{2} + O(1) $$
中，右侧三角和的第一项，即 $\cos \vartheta$，实际上在区间 $0 < t < T$ 内渐近地有 $\frac{T}{2\pi} \log \frac{T}{2\pi} - \frac{T}{2\pi}$ 个零点；并且系数 $\frac{1}{\sqrt{1}}, \frac{1}{\sqrt{2}}, \frac{1}{\sqrt{3}}, \dots$ 单调递减。也许黎曼相信这一观察结果可以用于证明他的断言。

很明显，可以使用精确的黎曼公式来估计均值
$$ \frac{1}{T} \int_{0}^{T} \left| \zeta \left( \frac{1}{2} + ti \right) \right|^{2n} dt \quad (n = 3, 4, \dots); $$
这些均值是众所周知的，并且与所谓的林德洛夫猜想（Lindelöf conjecture）密切相关。但在这里，人们遇到了由于自然数因子分解导致的算术性质的相当大的困难。

对于建立 Zeta 函数的数值表，特别是为了进一步计算零点，渐近展开式有巨大的益处。然而，如果人们必须将其用于实际应用目的，就必须开发出比 § 2 中推导出的更仔细的余项估计。黎曼利用他的公式进行了相当广泛的计算，以确定 $\zeta(\frac{1}{2} + ti)$ 的正零点。对于最小的正零点，他发现值 $a_1 = 14.1386$；格拉姆（Gram）计算出的值为 $14.1347$，差异不到千分之三。利用 $\zeta(s)$ 的乘积表示也可以得出 $a_1$ 的下界，产生易于证明的方程
$$ \sum_{n=1}^{\infty} \left( a_n^2 + \frac{1}{4} \right)^{-1} = 1 + \frac{1}{2} \gamma - \frac{1}{2} \log \pi - \log 2, $$
其中 $\gamma$ 是欧拉常数，且 $a_n$ 遍历 $\zeta(\frac{1}{2} + ai) = 0$ 位于右半平面的所有解 $a$。由此黎曼断言
$$ \sum_{n=1}^{\infty} \left( a_n^2 + \frac{1}{4} \right)^{-1} = 0.02309 \ 57089 \ 66121 \ 03381. $$
对于 $a_3$，他找到了值 25.31；而格拉姆给出的值为 25.01。
第二个黎曼公式，即 $\zeta(s)$ 的积分表示，或许对理论更具意义。人们将试图从 (60) 中获得一些关于临界线上 $\zeta(s)$ 零点分布的信息。让 $t$ 在区间 $t_1 < t < t_2$ 内增加。在此过程中，$\arg \varphi(\frac{1}{2} + ti)$ 增加了 $\Delta$，当通过一个位于 $\sigma = \frac{1}{2}$ 的 $\varphi(s)$ 的可能零点时，该变化量等于 $\pi$ 乘以该零点的重数，所以由 (60)，$\zeta(\frac{1}{2} + ti)$ 在 $t_1 < t < t_2$ 内的零点数大于 $\frac{|\Delta|}{\pi} - 1$。但是现在，我们有
$$ (63) \quad \arg \left\{ \pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right) \right\} = \vartheta = \frac{t}{2} \log \frac{t}{2\pi} - \frac{t}{2} + O(1), $$
因此根据 (59)，$\zeta(\frac{1}{2} + ti)$ 位于区间 $0 < t < T$ 的零点数渐近地至少等于 $\frac{T}{2\pi} \log T$，即渐近等于 $\zeta(s)$ 位于带状区域 $0 < t < T$ 内的零点数，如果由 (58) 定义的函数 $\mathfrak{f}(\frac{1}{2} + ti)$ 的辐角随 $t \to \infty$ 的减少速度慢于 $-t \log t$。对于每个半带 $\sigma_1 \le \sigma \le \sigma_2, t > 0$，人们可以用 § 2 的方法将 $\mathfrak{f}(s)$ 展开为渐近级数；但是人们再次获得作为主项的 $[\sqrt{\frac{t}{2\pi}}]$ 个加项的和，即 $\sum_{n=1}^{m} n^{-s}$；而研究这个和的辐角是一个与研究 (62) 中出现的和的零点完全相同难度的难题，因此通过引入 $\mathfrak{f}(s)$ 我们显然没有获得任何东西。
如果现在考虑边为 $\sigma = \frac{1}{2}, \sigma = 2, t = 0, t = T$ 的矩形，其上边不包含 $\mathfrak{f}(s)$ 的零点，那么 $\frac{1}{2\pi} \arg \mathfrak{f}(s)$ 沿矩形正向环绕的变化量等于矩形内 $\mathfrak{f}(s)$ 的零点数。在下边，$\arg \mathfrak{f}(s)$ 变化 $O(1)$，在服从渐近级数的右边，也只变化 $O(1)$。此外，可以用 Zeta 函数理论中的常用方法证明，上边的变化至多为 $O(\log T)$。因此，除去量级为 $\log T$ 的误差外，$\arg \mathfrak{f}(\frac{1}{2} + ti)$ 在区间 $0 < t < T$ 内的变化量等于 $-2\pi$ 乘以矩形内 $\mathfrak{f}(s)$ 的零点数。由此，问题简化为研究整超越函数 $\mathfrak{f}(s)$ 的零点。

黎曼试图获得关于 $\mathfrak{f}(s)$ 零点的陈述，为此他从 (58) 构造关系
$$ |\mathfrak{f}(\sigma+ti)|^2 = \int_{0 \swarrow 1} \int_{0 \swarrow 1} \frac{x^{-\sigma-ti} y^{-\sigma+ti} e^{\pi i (x^2-y^2)}}{(e^{\pi i x} - e^{-\pi i x})(e^{\pi i y} - e^{-\pi i y})} dx dy $$
并通过引入新变量、积分区域变形和使用留数定理将复双重积分转化为另一种形式；然而，这并没有导致有用的结果。
到目前为止，关于 $\mathfrak{f}(s)$ 零点的位置知之甚少。在黎曼那里我们找不到关于这个主题的进一步评论；因此，在这篇历史数学论文的背景下，以下关于 $\mathfrak{f}(s)$ 理论的评论必须保持简短。它们提供了不等式
$$ N_0(T) > \frac{3}{8\pi} e^{-\frac{3}{2}} T + o(T) $$
的证明。
对于 $\mathfrak{f}(s)$，可以用 § 2 的方法找到一个渐近级数；对于当前的目的，考虑该级数的主项就足够了。首先将证明，在 $t > 0, -\sigma \ge t^{\frac{3}{7}}$ 的区域，以下公式适用
$$ (64) \quad \mathfrak{f}(s) \sim e^{\pi i (\frac{s}{2} - \frac{7}{8})} \pi^{\frac{s-1}{2}} \sin \frac{\pi s}{2} \Gamma \left( \frac{1-s}{2} \right) \frac{\sin \pi \eta}{\cos 2\pi \eta} \quad (|s| \to \infty) $$
其中使用缩写
$$ \eta = \sqrt{\frac{s-1}{2\pi i}} \quad (0 < \arg \eta < \frac{\pi}{4}). $$
现在，由 (56)
$$ (65) \quad \mathfrak{f}(s) = \pi^{s-\frac{1}{2}} \frac{\Gamma(\frac{1-s}{2})}{\Gamma(\frac{s}{2})} \left\{ \zeta(1-s) - \int_{0 \nwarrow 1} \frac{x^{s-1} e^{-\pi i x^2}}{e^{\pi i x} - e^{-\pi i x}} dx \right\}. $$
函数 $x^{s-1} e^{-\pi i x^2}$ 的鞍点位于 $x = \eta$。设定
$$ \Re(\eta) = \eta_1, \quad \Im(\eta) = \eta_2 $$
$$ m = [\eta_1 + \eta_2] $$
$$ z = x - \eta $$
$$ w(z) = e^{2\pi i \eta^2 \{ \log(1+\frac{z}{\eta}) - \frac{z}{\eta} + \frac{1}{2}(\frac{z}{\eta})^2 \}} - 1. $$

对于每个自然数 $k$，由柯西定理可得
$$ (66) \quad \int_{0 \nwarrow 1} \frac{x^{s-1} e^{-\pi i x^2}}{e^{\pi i x} - e^{-\pi i x}} dx = \sum_{n=1}^{k} n^{s-1} + \eta^{s-1} e^{-\pi i \eta^2} \left\{ \int_{k \swarrow k \parallel 1} \frac{e^{-2\pi i (z-\eta)^2}}{e^{\pi i z} - e^{-\pi i z}} dx + \int_{k \swarrow k \parallel 1} \frac{e^{-2\pi i (z-\eta)^2}}{e^{\pi i z} - e^{-\pi i z}} w(z) dx \right\}. $$
人们现在很容易想完全照搬 § 2 的方法，因此选择 $k=m$；但那样一来，只能在较小的矩形区域 $t > 0, -\sigma \ge t^{\frac{1}{2}}$ 内直接获得 (64)，而扩展到附加区域 $t^{\frac{1}{2}} > -\sigma \ge t^{\frac{3}{7}}$ 则需要消除某些额外项。这就是为什么我们最初让 $k$ 任意选择。
(66) 右侧的第一个积分可以根据 § 1 中黎曼的方法计算；得到
$$ (67) \quad \int_{k \swarrow k \parallel 1} \frac{e^{-2\pi i (z-\eta)^2}}{e^{\pi i z} - e^{-\pi i z}} dx = \frac{\sqrt{2} e^{\frac{3\pi i}{8}} \sin \pi \eta + (-1)^{k-1} e^{2\pi i \eta - 2\pi i (\eta-k)^2}}{2 \cos 2\pi \eta}. $$

在第二个积分中，我们将积分路径引导穿过鞍点 $x = \eta$，并使其平行于第二和第四象限的角平分线行进。因此它在点 $\eta_1 + \eta_2$ 处穿过实轴。然而，为了避开极点 $x=m$ 和 $x=m+1$ 的邻域，人们仍然可以用位于圆 $|x-m|=\frac{1}{2}$ 和 $|x-m-1|=\frac{1}{2}$ 内部的积分路径部分替换为这些圆的圆弧。如果做出假设
$$ k = m + r \ge m, $$
那么
$$ (68) \quad \int_{k \swarrow k \parallel 1} \frac{e^{-2\pi i (x-\eta)^2}}{e^{\pi i x} - e^{-\pi i x}} w(z) dx = \sum_{l=1}^{r} (-1)^{m+l-1} e^{-2\pi i (m+l-\eta)^2} w(m+l-\eta) + \int_{m \swarrow m \parallel 1} \frac{e^{-2\pi i (x-\eta)^2}}{e^{\pi i x} - e^{-\pi i x}} w(z) dx. $$
对于 $w(z)$ 需要两个估计。第一个涉及圆 $|z| \le \frac{1}{2}|\eta|$；具体来说，即
$$ \left| \log \left( 1 + \frac{z}{\eta} \right) - \frac{z}{\eta} + \frac{1}{2} \left( \frac{z}{\eta} \right)^2 \right| = \left| \sum_{n=3}^{\infty} \frac{(-1)^{n-1}}{n} \left( \frac{z}{\eta} \right)^n \right| \le \frac{1}{3} \left| \frac{z}{\eta} \right|^3 \frac{1}{1 - \left| \frac{z}{\eta} \right|} \le \frac{2}{3} \left| \frac{z}{\eta} \right|^3 $$
因此
$$ (69) \quad |w(z)| \le e^{\frac{4\pi}{3} \left| \frac{z^3}{\eta} \right|} - 1 \quad (|z| \le \frac{1}{2}|\eta|). $$
第二个涉及位于该圆外的积分路径部分。如果现在设定 $\Re(z e^{\frac{\pi i}{4}}) = u, \Im(z e^{\frac{\pi i}{4}}) = v$，那么在积分路径上 $-\frac{1}{2} \le v \le +\frac{1}{2}$，并且在 $|\eta| > 1$ 的情况下，在圆 $|z| = \frac{1}{2}|\eta|$ 之外适用不等式
$$ \left| \frac{v}{u} \right| < (|\eta|^2 - 1)^{-\frac{1}{2}}, $$
所以
$$ \arg \left( 1 + \frac{iv}{u} \right) \to 0 \quad (|s| \to \infty) $$
且
$$ \frac{\pi}{4} - \varepsilon < \left| \arg \frac{z}{\eta} \right| < \frac{3\pi}{4} + \varepsilon, $$
其中 $\varepsilon \to 0$ 当 $|s| \to \infty$。但是此时
$$ \left| 2\pi i \eta^2 \left\{ \log \left( 1 + \frac{z}{\eta} \right) - \frac{z}{\eta} + \frac{1}{2} \left( \frac{z}{\eta} \right)^2 \right\} \right| = 2\pi |\eta|^2 \cdot \left| \int_{0}^{z} \frac{x^2}{1+x} dx \right| $$
$$ \le 2\pi |\eta|^2 \int_{0}^{|z|} \frac{x^2}{\sin (\frac{\pi}{4} - \varepsilon)} dx = \frac{\pi |z|^2}{\sin (\frac{\pi}{4} - \varepsilon)} \le \frac{3}{2} \pi |z|^2 $$
且
$$ |w(z)| < e^{\frac{3}{2} \pi |z|^2}. $$
此外，在积分路径上
$$ |e^{-2\pi i z^2}| = |e^{-2\pi (u^2 - v^2)}| \le e^{\pi - 2\pi |z|^2}; $$
且因此
$$ |e^{-2\pi i z^2} w(z)| \le \left\{
\begin{aligned}
&e^{\pi - \frac{\pi}{2} |z|^2} \quad &(|z| > \frac{1}{2}|\eta|) \\
&e^{\pi - 2\pi |z|^2} \left( e^{\frac{4\pi}{3} \left| \frac{z^3}{\eta} \right|} - 1 \right) \quad &(|z| \le \frac{1}{2}|\eta|).
\end{aligned}
\right. $$
这就得出
$$ \int_{m \swarrow m \parallel 1} \frac{e^{-2\pi i (z-\eta)^2}}{e^{\pi i x} - e^{-\pi i x}} w(z) dx = O \left( e^{-\pi \eta_2} \eta^{-1} \right) $$
并结合 (65), (66), (67), (68)
$$ (70) \quad \mathfrak{f}(s) = \pi^{s-\frac{1}{2}} \frac{\Gamma \left( \frac{1-s}{2} \right)}{\Gamma \left( \frac{s}{2} \right)} \eta^{s-1} e^{-\pi i \eta^2} \left\{ e^{\pi i \eta^2} \sum_{n=m+r+1}^{\infty} \left( \frac{n}{\eta} \right)^{s-1} - \frac{\sqrt{2} e^{\frac{3\pi i}{8}} \sin \pi \eta + (-1)^{m+r-1} e^{2\pi i \eta - 2\pi i (\eta - m - r)^2}}{2 \cos 2\pi \eta} + \sum_{l=1}^{r} (-1)^{m+l} e^{-2\pi i (m+l-\eta)^2} w(m+l-\eta) + O(e^{-\pi \eta_2} \eta^{-1}) \right\}. $$
现在必须证明，对于 $r$ 的适当选择以及 $|s| \to \infty$ 在区域 $t > 0, -\sigma \ge t^{\frac{3}{7}}$ 内，项
$$ -\frac{\sqrt{2} e^{\frac{3\pi i}{8}} \sin \pi \eta}{2 \cos 2\pi \eta} $$
比花括号中的其他项具有更高的阶数。首先，
$$ (71) \quad \left| e^{\pi i \eta^2} \sum_{n=m+r+1}^{\infty} \left( \frac{n}{\eta} \right)^{s-1} \right| < e^{-2\pi \eta_1 \eta_2} |\eta|^{1-s} \left\{ \frac{(m+r+1)^\sigma}{-\sigma} + (m+r+1)^{\sigma-1} \right\} < e^{-2\pi \eta_1 \eta_2 + t \arg \eta} \left( \frac{m+r+1}{|\eta|} \right)^{\sigma-1} \left( \frac{m+r+1}{-\sigma} + 1 \right); $$
因为
$$ (72) \quad -2\pi \eta_1 \eta_2 + t \arg \eta < -2\pi \eta_1 \eta_2 + t \frac{\eta_2}{\eta_1} = -2\pi \frac{\eta_2^3}{\eta_1} < 0 $$
且
$$ \left( \frac{m+1}{|\eta|} \right)^{\sigma-1} < \left( \frac{\eta_1^2 + \eta_2^2 + 2\eta_1 \eta_2}{\eta_1^2 + \eta_2^2} \right)^{\frac{\sigma-1}{2}} < e^{\frac{\sigma-1}{2} \frac{2\eta_1 \eta_2}{\eta_1^2 + \eta_2^2}} < e^{\frac{\eta_2}{\eta_1} \frac{\sigma-1}{2}} = e^{-\pi \eta_2^2} $$
因此
$$ (73) \quad \left| e^{\pi i \eta^2} \sum_{n=m+1}^{\infty} \left( \frac{n}{\eta} \right)^{s-1} \right| = O \left( e^{-\pi \eta_2^2} \left( 1 + \frac{\eta_1}{-\sigma} \right) \right); $$
并且还有
$$ (74) \quad \left| (-1)^{m-1} e^{2\pi i \eta - 2\pi i (\eta-m)^2} \right| = e^{-2\pi \eta_2 - 4\pi (m-\eta_1) \eta_2} < e^{-4\pi (\eta_2 - \frac{1}{2}) \eta_2}. $$
现在，对于子区域 $t > 0, -\sigma \ge t^{\frac{5}{8}}$ 不等式
$$ \eta_2 = \frac{1-\sigma}{4\pi \eta_1} > \frac{1-\sigma}{2} \{ 2\pi (t + 1 - \sigma) \}^{-\frac{1}{2}} > \frac{1}{2} t^{\frac{5}{8}} \{ 2\pi (t + t^{\frac{5}{8}}) \}^{-\frac{1}{2}} $$
得到满足，且右侧随 $t$ 趋于无穷，所以考虑到 (73) 和 (74) 可得，(70) 中花括号内的表达式在上述子区域对于 $r=0$ 取值
$$ (75) \quad \frac{\sqrt{2} e^{\frac{3\pi i}{8}} \sin \pi \eta}{2 \cos 2\pi \eta} (1 + o(1)) \quad (|s| \to \infty) $$
在现在要处理的子区域 $t > 0, t^{\frac{5}{8}} > -\sigma \ge t^{\frac{3}{7}}$ 中，选择
$$ r = [|\sigma|^{\frac{1}{5}}]. $$
那么对于足够大的 $t$
$$ \left( \frac{m+r+1}{|\eta|} \right)^{\sigma-1} < \left( \frac{|\eta|+r}{|\eta|} \right)^{\sigma-1} < e^{\frac{\sigma-1}{2} \cdot \frac{r}{2\eta_1}} = e^{-\pi r \eta_2}, $$
因此，由 (71) 和 (72)
$$ (76) \quad e^{\pi i \eta^2} \sum_{n=m+r+1}^{\infty} \left( \frac{n}{\eta} \right)^{s-1} = O \left( e^{-\pi r \eta_2} \left( 1 + \left| \frac{\eta}{\sigma} \right| \right) \right) = O \left( e^{-\frac{1}{2} t^{\frac{1}{10}}} \right). $$
此外，对于 $l=1, \dots, r$
$$ (77) \quad |m+l-\eta|^2 \le (r+\eta_2)^2 + \eta_2^2 = O(|\sigma|^{\frac{2}{5}}) = O(t^{\frac{1}{4}}), $$
所以因此对于足够大的 $t$，$m+l-\eta$ 位于圆 $|z| \le \frac{1}{2}|\eta|$ 内，且 (69) 对于 $z = m+l-\eta$ 适用；因为由 (77) 推出
$$ (78) \quad w(m+l-\eta) = O \left( |\sigma|^{\frac{3}{5}} |\eta|^{-1} \right). $$
最后，对于 $l=1, \dots, r$
$$ (79) \quad \left| e^{-2\pi i (m+l-\eta)^2} \right| < e^{-4\pi (\eta_2+l-1)\eta_2} \le e^{-4\pi r \eta_2^2} $$
且对于足够大的 $t$
$$ (80) \quad \left| e^{-2\pi i \eta - 2\pi i (m+l-\eta)^2} \right| < e^{-3\pi r \eta_2} = O(e^{-t^{\frac{1}{10}}}), $$
因此，根据 (78) 和 (79)
$$ (81) \quad \sum_{l=1}^{r} (-1)^{m+l} e^{-2\pi i (m+l-\eta)^2} w(m+l-\eta) = r O \left( e^{-4\pi \eta_2^2} |\sigma|^{\frac{3}{5}} |\eta|^{-1} \right) = O \left( e^{-4\pi \eta_2^2} |\sigma|^{\frac{4}{5}} |\eta|^{-1} \right). $$
现在考虑不等式
$$ |\sin \pi \eta| \ge \sinh \pi \eta_2 > \pi \eta_2 > \frac{|\sigma|}{4|\eta|} $$
$$ |\cos 2\pi \eta| \le \cosh 2\pi \eta_2 < 2e^{2\pi \eta_2}, $$

估计 (76), (80), (81) 表明，即使在区域 $t > 0, t^{\frac{5}{8}} > -\sigma \ge t^{\frac{3}{7}}$ 内，(70) 花括号中的值也由表达式 (75) 给出。
(64) 中的断言随后通过应用斯特林公式得出。
顺便提一下，甚至对于更大的区域 $t > 0, -\sigma \ge t^\varepsilon$（其中 $\varepsilon$ 是任何固定的正数）也可以证明 (64)；但对于接下来的内容，这就足够了，即每个 $\varepsilon$ 的值小于 $\frac{1}{2}$，例如 $\varepsilon = \frac{3}{7}$。

除了公式 (64) 之外，仍然需要对于固定的 $\sigma$ 和 $t \to \infty$ 对 $\mathfrak{f}(s)$ 的阶数进行粗略估计。这可以从 $\mathfrak{f}(s)$ 在区域 $t > 0, -\sigma \le t^{\frac{3}{7}}$ 的渐近展开中获得。观察 (64) 的证明表明，人们对方程 (70) 应用条件 $-\sigma \ge t^{\frac{3}{7}}$ 仅在于其较弱的形式 $\sigma < \sigma_0$，其中 $\sigma_0$ 是任何实数。因此，类似于 (70) 且 $r=0$，这在四分之一平面 $\sigma < \sigma_0, t > 0$ 内是有效的：
$$ (82) \quad \mathfrak{f}(s) = \pi^{s-\frac{1}{2}} \frac{\Gamma \left( \frac{1-s}{2} \right)}{\Gamma \left( \frac{s}{2} \right)} \left( \zeta(1-s) - \sum_{n=1}^{m} n^{s-1} - \eta^{s-1} e^{-\pi i \eta^2} \left\{ \frac{\sqrt{2} e^{\frac{3\pi i}{8}} \sin \pi \eta + (-1)^{m-1} e^{2\pi i \eta - 2\pi i (\eta-m)^2}}{2 \cos 2\pi \eta} + O(\eta^{-1}) \right\} \right) $$
其中 $\eta = \sqrt{\frac{s-1}{2\pi i}}, |\arg \eta| < \frac{\pi}{4}, m = [\Re \eta + \Im \eta]$。渐近级数的其他项可以通过 § 2 的方法获得，但对于当前的目的并不需要。

$\mathfrak{f}(s)$ 的第二个渐近展开，它对于四分之一平面 $\sigma > \sigma_0, t > 0$ 更可取，是通过应用鞍点法得到的，不是对 (65) 提供的 $\mathfrak{f}(s)$ 的表示，而是对 (58) 的表示。计算无需完整重复，因为 (58) 中的积分是通过过渡到复共轭变量并用 $1-\sigma$ 替换 $\sigma$ 从 (65) 中的积分产生的。因此，
$$ (83) \quad \mathfrak{f}(s) = \sum_{n=1}^{m_1} n^{s-1} + \eta_1^{s-1} e^{\pi i \eta_1^2} \left\{ \frac{\sqrt{2} e^{-\frac{3\pi i}{8}} \sin \pi \eta_1 + (-1)^{m_1-1} e^{-2\pi i \eta_1 - 2\pi i (\eta_1-m_1)^2}}{2 \cos 2\pi \eta_1} + O(\eta_1^{-1}) \right\} $$
其中 $\eta_1 = \sqrt{\frac{s}{2\pi i}}, |\arg \eta_1| < \frac{\pi}{4}, m_1 = [\Re \eta_1 - \Im \eta_1]$ 在四分之一平面 $\sigma > \sigma_0, t > 0$ 内。通过比较 (82) 和 (83)，得出了 $\zeta(s)$ 在每个半带 $\sigma_1 < \sigma < \sigma_2, t > 0$ 内的渐近级数；这个推导相对于 § 2 中必要的估计可能稍微简单一些，但级数的单个项在这里最初以更复杂的形式出现。

从 (83) 可以得出
$$ (84) \quad \left\{
\begin{aligned}
&\mathfrak{f}(s) = \sum_{n=1}^{m_1} n^{-s} + O \left( \left( \frac{|s|}{2\pi e} \right)^{-\frac{\sigma}{2}} \right) \quad &(\sigma \ge 0, t > 0) \\
&\mathfrak{f}(s) = O(t^{\frac{1}{4}}) \quad &(\sigma \ge \frac{1}{2}) \\
&|\mathfrak{f}(s) - 1| < \frac{3}{4} \quad &(\sigma \ge 2, t > t_0).
\end{aligned}
\right. $$
并从 (82) 得出
$$ (85) \quad \left\{
\begin{aligned}
&\mathfrak{f}(s) = \pi^{s-\frac{1}{2}} \frac{\Gamma(\frac{1-s}{2})}{\Gamma(\frac{s}{2})} \left( \zeta(1-s) - \sum_{n=1}^{m} n^{s-1} + O(1) \right) \quad &(\sigma \le 1, t > 0) \\
&\mathfrak{f}(s) = \pi^{s-\frac{1}{2}} \frac{\Gamma(\frac{1-s}{2})}{\Gamma(\frac{s}{2})} O \left( \left( \frac{t}{2\pi} \right)^{\frac{\sigma}{2}} |\sigma|^{-1} \right) \quad &(0 < -\sigma \le t^{\frac{3}{7}}, t > 0) \\
&\mathfrak{f}(s) = \pi^{s-\frac{1}{2}} \frac{\Gamma(\frac{1-s}{2})}{\Gamma(\frac{s}{2})} O(\log t) \quad &(0 < -\sigma \le t^{\frac{3}{7}}, t > 0).
\end{aligned}
\right. $$
在接下来的内容中，方便的是，代替 $\mathfrak{f}(s)$ 引入函数
$$ g(s) = \pi^{-\frac{s+1}{2}} e^{-\frac{\pi i s}{2}} \Gamma \left( \frac{s+1}{2} \right) \mathfrak{f}(s) $$
由 (64) 我们有，对于 $t > 0, -\sigma \ge t^{\frac{3}{7}}$ 且 $\eta = \sqrt{\frac{s-1}{2\pi i}}$
$$ (86) \quad g(s) \sim e^{-\frac{7\pi i}{8}} \tan \frac{\pi s}{2} \frac{\sin \pi \eta}{\cos 2\pi \eta} \quad (|s| \to \infty). $$

现在应该可以估计 $|g(s)|^2$ 在每条半线 $\sigma = \sigma_0 < \frac{1}{2}, t \ge 0$ 上的平均值，具体来说，即表达式
$$ T^{-1} \int_{0}^{T} |g(\sigma+ti)|^2 dt \quad (\sigma < \frac{1}{2}). $$
人们可以借助渐近展开 (82) 来实现这一点；然而，最优雅的方式是使用 (58) 进行推导；由此，具体对于 $\varepsilon > 0$
$$ \int_{0}^{\infty} |\mathfrak{f}(\sigma+ti)|^2 e^{-\varepsilon t} dt $$
$$ = \int_{0}^{\infty} e^{-\varepsilon t} \left\{ \int_{0 \swarrow 1} \int_{0 \swarrow 1} \frac{x^{-\sigma-ti} y^{-\sigma+ti} e^{\pi i (x^2-y^2)}}{(e^{\pi i x} - e^{-\pi i x})(e^{\pi i y} - e^{-\pi i y})} dx dy \right\} dt, $$
在这里，可以通过变形积分路径、交换积分顺序以及应用留数定理来变换右侧。计算得出的陈述
$$ \int_{0}^{\infty} |\mathfrak{f}(\sigma+ti)|^2 e^{-\varepsilon t} dt \sim \frac{1}{2\varepsilon} (2\pi \varepsilon)^{\sigma - \frac{1}{2}} \Gamma \left( \frac{1}{2} - \sigma \right), $$
对于 $\sigma < \frac{1}{2}$ 和 $\varepsilon \to \infty$ 有效，由此进一步得出
$$ \int_{1}^{\infty} |\mathfrak{f}(\sigma+ti)|^2 \left( \frac{t}{2\pi} \right)^\sigma e^{-\varepsilon t} dt \sim \frac{(2\varepsilon)^{-\frac{3}{2}}}{1-2\sigma}. $$
所以对于每个固定的 $\sigma < \frac{1}{2}$
$$ \int_{1}^{T} |\mathfrak{f}(\sigma+ti)|^2 \left( \frac{t}{2\pi} \right)^\sigma dt \sim \frac{1}{3\sqrt{2\pi}} \frac{T^{\frac{3}{2}}}{\frac{1}{2} - \sigma}. $$
但从斯特林公式得出附加陈述
$$ (87) \quad |g(s)| \sim \sqrt{2\pi}^{-\frac{1}{2}} \left( \frac{t}{2} \right)^{\frac{\sigma}{2}} |\mathfrak{f}(s)|, $$
并以此赢得所需的公式
$$ T^{-1} \int_{1}^{T} |g(\sigma+ti)|^2 dt \sim \frac{1}{3} \sqrt{\frac{2}{\pi}} \frac{T^{\frac{1}{2}}}{\frac{1}{2} - \sigma} $$
对于固定的 $\sigma < \frac{1}{2}$。由此进一步得出
$$ (88) \quad \int_{0}^{T} \log |g(\sigma+ti)| dt < \frac{T}{2} \log \frac{\sqrt{2} T^{\frac{1}{2}}}{3\sqrt{\pi} (\frac{1}{2} - \sigma)} + o(T) \quad (\sigma < \frac{1}{2}, T \to \infty). $$
对于 $\sigma = \frac{1}{2}$，结果是 $\int_{0}^{T} \log |g(\sigma+ti)| dt$ 的一个下界。实际上，根据 (60)，在临界线上
$$ \left| \pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right) \zeta(s) \right| \le \left| 2\pi^{-\frac{s}{2}} \Gamma \left( \frac{s}{2} \right) \mathfrak{f}(s) \right|, $$
因此，由 (87)
$$ |g(s)| \ge (8\pi)^{-\frac{1}{4}} t^{\frac{1}{4}} |\zeta(s)| (1+o(1)) \quad (\sigma = \frac{1}{2}) $$
$$ (89) \quad \int_{0}^{T} \log \left| g \left( \frac{1}{2} + ti \right) \right| dt > \frac{T}{4} \log T - (\log 8\pi + 1) \frac{T}{4} + \int_{0}^{T} \log \left| \zeta \left( \frac{1}{2} + ti \right) \right| dt + o(T). $$
最后，对于 $\sigma \ge 2$，由 (87) 和 (84)
$$ (90) \quad \int_{0}^{T} \log |g(\sigma+ti)| dt = \sigma \left( \frac{T}{2} \log \frac{T}{2\pi} - \frac{T}{2} \right) + \frac{T}{2} \log 2 + o(T). $$

现在设 $t_0 > 0, T > t_0$，且直线 $t = t_0, t = T$ 不含函数 $g(s)$ 的零点。此外，设 $\sigma_0 > -T^{\frac{3}{7}} = \sigma_1$。考虑边为 $\sigma = \sigma_0, t = T, \sigma = \sigma_1, t = t_0$ 的矩形。在左侧 $\sigma = \sigma_1, t = t_0 \le t \le T$ 上有，对于足够大的 $T$，根据 (64) 没有 $g(s)$ 的零点。将位于矩形内的 $g(s)$ 的零点通过平行于实轴构造的割线连接到右侧 $\sigma = \sigma_0$。在切割后的矩形中，$\log g(s)$ 是单值的；它成为一个分支，通过要求 $0 \le \arg g(\sigma_1+Ti) < 2\pi$ 是固定的。众所周知，适用
$$ (91) \quad 2\pi \sum_{\alpha < \sigma_0} (\sigma_0 - \alpha) = \int_{t_0}^{T} \log |g(\sigma_0+ti)| dt - \int_{\sigma_1}^{\sigma_0} \arg g(\sigma+Ti) d\sigma - \int_{t_0}^{T} \log |g(\sigma_1+ti)| dt + \int_{\sigma_1}^{\sigma_0} \arg g(\sigma+t_0 i) d\sigma, $$
其中 $\alpha$ 遍历位于正方形内的 $g(s)$ 的所有根的实部。第一个积分可以针对 $\sigma_0 < \frac{1}{2}$ 向上精确估计，针对 $\sigma_0 = \frac{1}{2}$ 向下精确估计，针对 $\sigma_0 \ge 2$。第三和第四个积分贡献，正如可以毫无困难地通过 (86) 看出的那样，仅是一个阶数为 $T^{\frac{13}{14}}$ 的量。最后，第二个积分可以用通常的方式利用 (84) 和 (85) 估计为 $O(T^{\frac{6}{7}} \log T)$。相应地，由 (88)

$$ (92) \quad \sum_{\alpha < \sigma} (\sigma - \alpha) < \frac{T}{8\pi} \log T - \frac{T}{4\pi} \log \left\{ 3\sqrt{\frac{\pi}{2}} \left( \frac{1}{2} - \sigma \right) \right\} + o(T) \quad (\sigma < \frac{1}{2}), $$
由 (89)
$$ (93) \quad \sum_{\alpha < \frac{1}{2}} \left( \frac{1}{2} - \alpha \right) < \frac{T}{8\pi} \log T - (1 + \log 8\pi) \frac{T}{8\pi} + \frac{1}{2\pi} \int_{0}^{T} \log \left| \zeta \left( \frac{1}{2} + ti \right) \right| dt + o(T) $$
以及由 (90)
$$ (94) \quad \sum_{\alpha} (\sigma - \alpha) = \sigma \left( \frac{T}{4\pi} \log \frac{T}{2\pi} - \frac{T}{4\pi} \right) - \frac{T}{4\pi} \log 2 + o(T) \quad (\sigma \ge 2); $$
在最后一个方程中让 $\alpha$ 遍历位于带状区域 $0 < t < T$ 内 $g(s)$ 的所有零点的实部。如果它们的数目指定为 $N_1(T)$，那么由 (94)
$$ (95) \quad N_1(T) = \frac{T}{4\pi} \log \frac{T}{2\pi} - \frac{T}{4\pi} + o(T). $$
在上半平面，$g(s)$ 的零点与 $\mathfrak{f}(s)$ 的零点一致。在 $N_1(T)$ 个零点中有多达 $o(T)$ 个位于 $\sigma = \frac{1}{2}$ 右侧的条件下，那么区间 $0 < t < T$ 内 $\arg \mathfrak{f}(\frac{1}{2} + ti)$ 的变化量将等于 $-(\frac{T}{2} \log \frac{T}{2\pi} - \frac{T}{2}) + o(T)$，并且人们得不到关于 $\zeta(\frac{1}{2} + ti)$ 零点的陈述。然而，首先从 (94) 进一步得出
$$ \sum_{\alpha} \alpha = -\frac{T}{4\pi} \log 2 + o(T); $$
因此肯定有无限多个 $\mathfrak{f}(s)$ 的零点甚至位于 $\sigma = 0$ 的左侧；并且这是从 (92) 和 (93) 中获得的，独立于 (94)，通过减去位于区域 $\sigma < \frac{1}{2}, 0 < t < T$ 内 $\mathfrak{f}(s)$ 的零点数目的下界。我们将这个数目记为 $N_2(T)$，那么对于每个 $\sigma < \frac{1}{2}$ 随后有
$$ \left( \frac{1}{2} - \sigma \right) N_2(T) > \frac{T}{4\pi} \log \left\{ \frac{3}{4} e^{-\frac{1}{2}} \left( \frac{1}{2} - \sigma \right) \right\} + \frac{1}{2\pi} \int_{0}^{T} \log \left| \zeta \left( \frac{1}{2} + ti \right) \right| dt + o(T). $$
这个估计对于
$$ \sigma = \frac{1}{2} - \frac{4}{3} e^{\frac{1}{2}} $$
是最有利的，结果是
$$ N_2(T) > \frac{3}{16\pi} e^{-\frac{3}{2}} T + \frac{3}{8\pi} e^{-\frac{3}{2}} \int_{0}^{T} \log \left| \zeta \left( \frac{1}{2} + ti \right) \right| dt + o(T). $$
现在众所周知，使用 (91) 形式的方法，用 $\zeta(s)$ 代替 $g(s)$，
$$ \frac{1}{2\pi} \int_{0}^{T} \log \left| \zeta \left( \frac{1}{2} + ti \right) \right| dt = \sum_{\alpha_\zeta > \frac{1}{2}} \left( \alpha_\zeta - \frac{1}{2} \right) + O(\log T), $$
其中 $\alpha_\zeta$ 遍历位于临界线右侧带状区域 $0 < t < T$ 内 Zeta 函数零点的实部。由此得出
$$ (96) \quad N_2(T) > \frac{3}{16\pi} e^{-\frac{3}{2}} T + \frac{3}{4} e^{-\frac{3}{2}} \sum_{\alpha_\zeta > \frac{1}{2}} \left( \alpha_\zeta - \frac{1}{2} \right) + o(\log T). $$
在 $\sigma = \frac{1}{2}$ 的右侧，带状区域 $0 < t < T$ 内至多有 $N_1(T) - N_2(T)$ 个 $\mathfrak{f}(s)$ 的零点，所以 $\arg \mathfrak{f}(\frac{1}{2} + ti)$ 在区间 $0 < t < T$ 内减少至多 $2\pi (N_1(T) - N_2(T)) + O(\log T)$。因此，$\arg \varphi(\frac{1}{2} + ti)$ 在这个区间内至少增加
$$ \vartheta(T) - 2\pi N_1(T) + 2\pi N_2(T) + O(\log T), $$
并且这个量由 (63), (95), (96) 至少等于 $2\pi N_2(T) + o(T)$。因此 $N_0(T)$，即区间 $0 < t < T$ 内 $\zeta(\frac{1}{2} + ti)$ 的零点数，满足不等式
$$ (97) \quad N_0(T) > \frac{3}{8\pi} e^{-\frac{3}{2}} T + \frac{3}{2} e^{-\frac{3}{2}} \sum_{\alpha_\zeta > \frac{1}{2}} \left( \alpha_\zeta - \frac{1}{2} \right) + o(T). $$
位于临界线上的 $\zeta(s)$ 零点的密度，即比率 $N_0(T) : T$ 当 $T \to \infty$ 时的下界，是正的且至少等于 $\frac{3}{8\pi} e^{-\frac{3}{2}}$，因此大于 $\frac{1}{38}$。除了这个数值之外，该陈述并非新发现，而是早在 1920 年就由哈代和李特尔伍德以一种更简单得多的方式证明了。尽管如此，这个次要结果或许表明这里讨论的 $\mathfrak{f}(s)$ 的性质具有某种独立的价值。
关于公式 (97) 可以做一个补充说明。黎曼猜想的不真实性可以在某种意义上通过总和 $\sum (\alpha_\zeta - \frac{1}{2})$ 来衡量。虽然人们通过李特尔伍德知道，这个总和不超过 $O(T \log \log T)$，但没有已知的更好估计。如果黎曼猜想是错误的，这个总和可能比 $T$ 增长得更快；那么，然而，由 (97)，数 $N_0(T)$ 将比 $T$ 增长得更快，并且黎曼猜想不可能“太错”。设 $\psi(t)$ 代表 $t$ 的任何正函数，它趋向于无穷大比 $\log t$ 慢，那么由 (97) 仍然得出，在狭窄区域 $0 \le \sigma - \frac{1}{2} \le \frac{\psi(t)}{\log t}, 2 \le t \le T$ 内，至少有 $\frac{3}{4\pi} e^{-\frac{3}{2}} T \psi(T) (1+o(1))$ 个 $\zeta(s)$ 的零点。这是一个新结果，甚至对于 $\psi(t)$ 增长比 $\log \log t$ 慢的情况也有效。所以，例如，在区域 $0 \le \sigma - \frac{1}{2} \le \frac{19}{\log t}, 2 \le t \le T$ 内有超过 $T + o(T)$ 个零点。
关于人们是否可以改进 (96) 中给出的 $N_2(T)$ 的下界的问题仍然悬而未决。为了证明黎曼关于 $N_0(T)$ 渐近等于 $\frac{T}{2\pi} \log \frac{T}{2\pi} - \frac{T}{2\pi}$ 的断言，只需展示关于 $N_2(T)$ 的相应陈述即可。如果不采用本质上新的思想，用以前 Zeta 函数理论中使用的分析方法似乎很难实现这一点；这对于任何证明黎曼猜想的尝试尤其如此。