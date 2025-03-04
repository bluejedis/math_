<span style="color: silver;">

# <span style="color: silver;"><span style="color: RoyalBlue;">函数</span>的图像

<ul>

* 用 ~ 指代 "函数"

## <span style="color: silver;">直角坐标系图像

<ul>

### <span style="color: silver;">常见图像

<ul>

#### <span style="color: silver;">基本初等~ 与初等~

<ul>

基本初等~ 包括：常数~ 、幂~ 、指数~ 、对数~ 、三角~ 、反三角~ 。

##### <span style="color: silver;">常数~

<ul>

$y=A$，$A$ 为常数，图像平行于 $x$ 轴。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.3yelaxpv6u.png)
*图像描述：一条平行于 x 轴的直线，位于 y=A 的位置，交 y 轴于 (0, A)。*

</ul>

##### <span style="color: silver;">幂~

<ul>

$y=x^{\mu}$，$\mu$ 为实数，当 $x>0$ 时，$y=x^{\mu}$ 都有定义：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.1hscw0jjoe.png)
*图像描述：展示不同 $\mu$ 值的幂~ 图像，例如 $\mu=-1$ (双曲线)，$\mu=1/2$ (平方根曲线)，$\mu=1$ (直线)，$\mu=2$ (抛物线)，经过点 (1,1)。*

对于幂~ 可以根据不同幂下相同单调性来研究最值：

1. $\sqrt{u}$，$\sqrt[3]{u}$ 可以使用 $u$ 来研究。
2. $\vert u \vert$ 可以使用 $u^2$ 来研究。
3. $\dfrac{1}{u}, u>0$ 可以使用 $u$ 来研究，但是最值相反。
4. $u_1 u_2 \dots u_n$ 可以使用 $\sum_{i=1}^{n} \ln u_i$ 来研究。

</ul>

##### <span style="color: silver;">指数~

<ul>

$y=a^x (a>0, a\neq 1)$：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9rjjk8ei1b.png)
*图像描述：展示 $0<a<1$ (下降曲线) 和 $a>1$ (上升曲线) 的指数~ ，过点 (0,1)。*

指数~ 具有如下性质：

1. 特殊~ 值：$a^0=1$。
2. 定义域：$(-\infty, +\infty)$，值域：$(0, +\infty)$。
3. 单调性：$a>1$ 时，$y=a^x$ 单调增；$0<a<1$ 时，$y=a^x$ 单调减。
4. 常用指数~ ：$y=e^x$。
5. <span style="color: Gold;">极</span>限：$\lim_{x\to -\infty} e^x = 0$，$\lim_{x\to +\infty} e^x = +\infty$。

</ul>

##### <span style="color: silver;">对数~

<ul>

$y=\log_a x (a>0, a\neq 1)$ 为 $y=a^x$ 的反~ ：

常用公式：$x=e^{\ln x}$，$u^v = e^{\ln u^v} = e^{v \ln u} (x>0, u>0)$。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.1lbytqdmgu.png)
*图像描述：展示 $0<a<1$ (下降曲线) 和 $a>1$ (上升曲线) 的对数~ ，过点 (1,0)。*

对数~ 具有如下性质：

1. 特殊~ 值：$\log_a 1 = 0$，$\log_a a = 1$，$\ln 1 = 0$，$\ln e = 1$。
2. 定义域：$(0, +\infty)$，值域：$(-\infty, +\infty)$。
3. 单调性：$a>1$ 时，$y=\log_a x$ 单调增；$0<a<1$ 时，$y=\log_a x$ 单调减。
4. 常用对数~ ：$y=\ln x$，$e=2.71828\dots$。
5. <span style="color: Gold;">极</span>限：$\lim_{x\to 0^+} \log_a x = -\infty$，$\lim_{x\to +\infty} \log_a x = +\infty$。

</ul>

##### <span style="color: silver;">三角~

<ul>

**正弦~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.esnl4pc1b.png)
*图像描述：周期性波浪曲线，周期为 $2\pi$，振幅为 1，经过原点，最大值 1，最小值 -1。*

**余弦~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.7i0j0qvejc.png)
*图像描述：周期性波浪曲线，周期为 $2\pi$，振幅为 1，起点为 (0,1)，最大值 1，最小值 -1。*

弦~ 有如下特征：

1. **特殊~ 值**：  
   $\sin 0=0$，$\sin \dfrac{\pi}{6} = \dfrac{1}{2}$，$\sin \dfrac{\pi}{4} = \dfrac{\sqrt{2}}{2}$，$\sin \dfrac{\pi}{3} = \dfrac{\sqrt{3}}{2}$，$\sin \dfrac{\pi}{2} = 1$，  
   $\sin \pi = 0$，$\sin \dfrac{3\pi}{2} = -1$，$\sin 2\pi = 0$，  
   $\cos 0 = 1$，$\cos \dfrac{\pi}{6} = \dfrac{\sqrt{3}}{2}$，$\cos \dfrac{\pi}{4} = \dfrac{\sqrt{2}}{2}$，$\cos \dfrac{\pi}{3} = \dfrac{1}{2}$，$\cos \dfrac{\pi}{2} = 0$，  
   $\cos \pi = -1$，$\cos \dfrac{3\pi}{2} = 0$，$\cos 2\pi = 1$。
2. **定义域**：$(-\infty, +\infty)$，**值域**：$[-1, +1]$。
3. **奇偶性**：$y=\sin x$ 为奇~ ，$y=\cos x$ 为偶~ 。
4. **周期性**：最小正周期为 $2\pi$。
5. **有界性**：$\vert \sin x \vert \leqslant 1$，$\vert \cos x \vert \leqslant 1$。

**正切~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.5j4caeq9uo.png)
*图像描述：周期性曲线，周期为 $\pi$，在 $x = \pm \dfrac{\pi}{2}$ 等处有垂直渐近线。*

**余切~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9nzxminmhs.png)
*图像描述：周期性曲线，周期为 $\pi$，在 $x = 0, \pm \pi$ 等处有垂直渐近线。*

切~ 有如下特征：

1. **特殊~ 值**：  
   $\tan 0 = 0$，$\tan \dfrac{\pi}{6} = \dfrac{\sqrt{3}}{3}$，$\tan \dfrac{\pi}{4} = 1$，$\tan \dfrac{\pi}{3} = \sqrt{3}$，$\lim_{x\to \dfrac{\pi}{2}} \tan x = \infty$，  
   $\tan \pi = 0$，$\lim_{x\to \dfrac{3\pi}{2}} \tan x = \infty$，$\tan 2\pi = 0$，  
   $\lim_{x\to 0} \cot x = \infty$，$\cot \dfrac{\pi}{6} = \sqrt{3}$，$\cot \dfrac{\pi}{4} = 1$，$\cot \dfrac{\pi}{3} = \dfrac{\sqrt{3}}{3}$，$\cot \dfrac{\pi}{2} = 0$，  
   $\lim_{x\to \pi} \cot x = \infty$，$\cot \dfrac{3\pi}{2} = 0$，$\lim_{x\to 2\pi} \cot x = \infty$。
2. **定义域**：$\tan x: x \neq k\pi + \dfrac{\pi}{2} (k \in \mathbb{Z})$，$\cot x: x \neq k\pi (k \in \mathbb{Z})$，**值域**：$(-\infty, +\infty)$。
3. **奇偶性**：定义域内均为奇~ 。
4. **周期性**：最小正周期为 $\pi$。

$\sec x = \dfrac{1}{\cos x}$，$\csc x = \dfrac{1}{\sin x}$：

**正割~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.5c14ez4n0p.png)
*图像描述：周期性曲线，周期为 $2\pi$，在 $x = \pm \dfrac{\pi}{2}$ 等处有垂直渐近线，值域为 $(-\infty, -1] \cup [1, +\infty)$。*

**余割~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.8l08bmsd2p.png)
*图像描述：周期性曲线，周期为 $2\pi$，在 $x = 0, \pm \pi$ 等处有垂直渐近线，值域为 $(-\infty, -1] \cup [1, +\infty)$。*

割~ 有如下特征：

1. **定义域**：$\sec x: x \neq k\pi + \dfrac{\pi}{2} (k \in \mathbb{Z})$，$\csc x: x \neq k\pi (k \in \mathbb{Z})$，**值域**：$(-\infty, -1] \cup [1, +\infty)$。
2. **奇偶性**：$y=\sec x$ 为偶~ ，$y=\csc x$ 为奇~ 。
3. **周期性**：最小正周期为 $2\pi$。

</ul>

##### <span style="color: silver;">反三角~

<ul>

类似是三角~ 的反~ ，但是由于是个多值~ 所以不是严格的~ 。所以为了限制反三角~ 为单值~ ，将反三角~ 的值限定在一个区间内，将其作为反三角~ 的主值。

**反正弦~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.5c14ez5dfd.png)
*图像描述：曲线从 (-1, $-\dfrac{\pi}{2}$) 到 (1, $\dfrac{\pi}{2}$)，过原点，单调递增。*

**反余弦~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.1zieklp1ft.png)
*图像描述：曲线从 (-1, $\pi$) 到 (1, 0)，过 (0, $\dfrac{\pi}{2}$)，单调递减。*

反弦~ 有如下特征：

1. **特殊~ 值**：  
   $\arcsin 0 = 0$，$\arcsin \dfrac{1}{2} = \dfrac{\pi}{6}$，$\arcsin \dfrac{\sqrt{2}}{2} = \dfrac{\pi}{4}$，$\arcsin \dfrac{\sqrt{3}}{2} = \dfrac{\pi}{3}$，$\arcsin 1 = \dfrac{\pi}{2}$，  
   $\arccos 1 = 0$，$\arccos \dfrac{\sqrt{3}}{2} = \dfrac{\pi}{6}$，$\arccos \dfrac{\sqrt{2}}{2} = \dfrac{\pi}{4}$，$\arccos \dfrac{1}{2} = \dfrac{\pi}{3}$，$\arccos 0 = \dfrac{\pi}{2}$。
2. **定义域**：$(-1, +1)$，**值域**：$\arcsin x: [-\dfrac{\pi}{2}, +\dfrac{\pi}{2}]$，$\arccos x: [0, \pi]$。
3. **单调性**：$y=\arcsin x$ 单调增，$y=\arccos x$ 单调减。
4. **奇偶性**：$y=\arcsin x$ 为奇~ 。
5. **有界性**：$\vert \arcsin x \vert \leqslant \dfrac{\pi}{2}$，$0 \leqslant \arccos x \leqslant \pi$。
6. **性质**：$\arcsin x + \arccos x = \dfrac{\pi}{2} (-1 \leqslant x \leqslant 1)$。

**对反弦~ 性质进行证明：**

令 $f(x) = \arcsin x + \arccos x$，对其求导得：  
$f'(x) = \dfrac{1}{\sqrt{1-x^2}} - \dfrac{1}{1-x^2} = 0$，所以 $f(x)$ 是个常数~ 。  
又 $f(0) = \dfrac{\pi}{2}$，所以该~ 恒等于 $\dfrac{\pi}{2}$。

**反正切~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.8dx0g777r5.png)
*图像描述：曲线从 $(-\infty, -\dfrac{\pi}{2})$ 到 $(+\infty, \dfrac{\pi}{2})$，过原点，单调递增，有水平渐近线 $y = \pm \dfrac{\pi}{2}$。*

**反余切~ ：**

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.1lbytqh5xd.png)
*图像描述：曲线从 $(-\infty, \pi)$ 到 $(+\infty, 0)$，过 $(0, \dfrac{\pi}{2})$，单调递减。*

反切~ 有如下特征：

1. **特殊~ 值**：  
   $\arctan 0 = 0$，$\arctan \dfrac{\pi}{6} = \dfrac{\sqrt{3}}{3}$，$\arctan 1 = \dfrac{\pi}{4}$，$\arctan \sqrt{3} = \dfrac{\pi}{3}$，  
   $\textrm{arccot}\,0 = \dfrac{\pi}{2}$，$\textrm{arccot}\,\sqrt{3} = \dfrac{\pi}{6}$，$\textrm{arccot}\,1 = \dfrac{\pi}{4}$，$\textrm{arccot}\,\dfrac{\sqrt{3}}{3} = \dfrac{\pi}{3}$。
2. **定义域**：$(-\infty, +\infty)$，**值域**：$\arctan x: [-\dfrac{\pi}{2}, +\dfrac{\pi}{2}]$，$\textrm{arccot}\,x: [0, \pi]$。
3. **单调性**：$y=\arctan x$ 单调增，$y=\textrm{arccot}\,x$ 单调减。
4. **奇偶性**：$y=\arctan x$ 为奇~ 。
5. **有界性**：$\vert \arctan x \vert \leqslant \dfrac{\pi}{2}$，$0 \leqslant \textrm{arccot}\,x \leqslant \pi$。
6. **性质**：  
   $\arctan x + \textrm{arccot}\,x = \dfrac{\pi}{2} (-\infty < x < +\infty)$；  
   $\arctan x = \textrm{arccot}\,\dfrac{1}{x} = \dfrac{\pi}{2} - \arctan x$。

</ul>

##### <span style="color: silver;">初等~

<ul>

由基本初等~ 经过有限次四则运算与复合步骤且可以被一个式子所表示。

幂指~ $u(x)^{v(x)} = e^{v(x) \ln u(x)}$ 也是初等~ 。

</ul>

</ul>

#### <span style="color: silver;">分段~

<ul>

$x$ 的不同范围对应不同的法则，经典形式如下：

$$
f(x) = \begin{cases}
\psi_1(x), & x > x_0 \\
a, & x = x_0 \\
\psi_2(x), & x < x_0
\end{cases}
\text{或}
f(x) = \begin{cases}
\psi(x), & x \neq x_0 \\
a, & x = x_0
\end{cases}
$$

##### <span style="color: silver;">绝对值~

<ul>

$$
y = |x| = \begin{cases}
x, & x \geqslant 0 \\
-x, & x < 0
\end{cases}
$$

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.6bh7s59rx5.png)
*图像描述：V 形曲线，以原点为顶点，右半部分为 $y=x$，左半部分为 $y=-x$。*

</ul>

##### <span style="color: silver;">符号~

<ul>

$$
y = \textrm{sgn}\,x = \begin{cases}
1, & x > 0 \\
0, & x = 0 \\
-1, & x < 0
\end{cases}
$$

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9nzxmiqlcy.png)
*图像描述：分段水平线，$x>0$ 时 $y=1$，$x=0$ 时 $y=0$（空心点），$x<0$ 时 $y=-1$。*

</ul>

##### <span style="color: silver;">取整~

<ul>

$x$ 为实数，不超过 $x$ 的最大整数称为其整数部分 $[x]$，其定义域为 $\mathbb{R}$，值域为 $\mathbb{Z}$。

1. $x - 1 < [x] \leqslant x$。
2. $\lim_{x \to 0^+} [x] = 0$。
3. $\lim_{x \to 0^-} [x] = -1$。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.32i3vhmsgy.png)
*图像描述：阶梯状曲线，每个整数区间内为水平线，例如 $[-1, 0)$ 为 $y=-1$，$[0, 1)$ 为 $y=0$。*

</ul>

</ul>

</ul>

### <span style="color: silver;">图像变换

<ul>

#### <span style="color: silver;">平移变换

<ul>

##### <span style="color: silver;">左右平移

<ul>

$f(x)$ 沿 $x$ 轴左移 $x_0$ 个单位长度得到 $f(x + x_0)$，向右移动 $x_0$ 个单位则得到 $f(x - x_0)$：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.3k85k2oc3v.png)
*图像描述：展示~ $-x^2+1$，$-(x-2)^2+1$（右移 2 单位），$-(x+2)^2+1$（左移 2 单位）的抛物线。*

</ul>

##### <span style="color: silver;">上下平移

<ul>

$f(x)$ 沿 $y$ 轴上移 $y_0$ 个单位长度得到 $f(x) + y_0$，向下移动 $y_0$ 个单位则得到 $f(x - y_0)$：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.4n7uuykd5n.png)
*图像描述：展示~ $-x^2+1$，$-x^2+3$（上移 2 单位），$-x^2-1$（下移 2 单位）的抛物线。*

</ul>

</ul>

#### <span style="color: silver;">对称变换

<ul>

##### <span style="color: silver;">上下对称

<ul>

将 $f(x)$ 关于 $x$ 轴对称得到 $-f(x)$：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.4g4mziyehn.png)
*图像描述：展示~ $-x^2+1$ 和其关于 $x$ 轴对称的 $x^2-1$ 的抛物线。*

</ul>

##### <span style="color: silver;">左右对称

<ul>

将 $f(x)$ 关于 $y$ 轴对称得到 $f(-x)$：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.6pnnj0jep0.png)
*图像描述：展示~ $\ln x$ 和其关于 $y$ 轴对称的 $\ln (-x)$ 的曲线。*

</ul>

##### <span style="color: silver;">原点对称

<ul>

将 $f(x)$ 关于 $x$ 轴和 $y$ 轴（即原点）对称得到 $-f(-x)$：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.1lbytqjn30.png)
*图像描述：展示~ $\ln x$ 和其关于原点对称的 $-\ln (-x)$ 的曲线。*

</ul>

##### <span style="color: silver;">反~ 对称

<ul>

将 $f(x)$ 关于 $y=x$ 对称得到 $f^{-1}(x)$：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.3d4xon35i3.png)
*图像描述：展示~ $\ln x$ 和其反~ $e^x$，以及对称轴 $y=x$ 的曲线。*

</ul>

##### <span style="color: silver;">~ 绝对值

<ul>

保留 $f(x)$ ~ 值在 $[0, \infty]$ 的部分，并对 $[-\infty, 0]$ 部分进行上下对称：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.8oju9cpeod.png)
*图像描述：展示~ $|x^2-1|$，保留 $x^2-1$ 的正部，将负部翻转为正，形成 V 形连接。*

</ul>

##### <span style="color: silver;">自变量绝对值

<ul>

先只保留 $f(x)$ 定义域在 $[0, \infty]$ 的部分，然后在 $[-\infty, 0]$ 部分使用 $[0, \infty]$ 的部分进行左右对称：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.1lbytqk584.png)
*图像描述：展示~ $-|x|^3 + 1$，右半部分为 $-x^3 + 1$，左半部分为其关于 $y$ 轴对称的镜像。*

</ul>

</ul>

#### <span style="color: silver;">伸缩变换

<ul>

##### <span style="color: silver;">水平伸缩

<ul>

纵坐标不变，当 $k>1$ 时，$y=f(kx)$ 是 $y=f(x)$ 缩短 $k$ 倍得到；当 $0<k<1$ 时，$y=f(kx)$ 是 $y=f(x)$ 伸长 $k$ 倍得到：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.92qa07y331.png)
*图像描述：展示 $\sin(x)$，$\sin(2x)$（缩短 2 倍），$\sin(\dfrac{x}{2})$（伸长 2 倍）的正弦曲线。*

</ul>

##### <span style="color: silver;">垂直伸缩

<ul>

横坐标不变，$y=k f(x)$ 的对应纵坐标为 $y=f(x)$ 对应纵坐标的 $k$ 倍：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.491f43dlpi.png)
*图像描述：展示 $\sin(x)$ 和 $\dfrac{\sin(x)}{2}$（纵向压缩 2 倍）的正弦曲线。*

</ul>

</ul>

</ul>

</ul>

</ul>

## <span style="color: silver;"><span style="color: Gold;">极</span>坐标系图像

<ul>

### <span style="color: silver;"><span style="color: Gold;">极</span>坐标系

<ul>

#### <span style="color: silver;"><span style="color: Gold;">极</span>坐标定义

<ul>

- **<span style="color: Gold;">极</span>点**：平面内的一个定点 $O$。
- **<span style="color: Gold;">极</span>轴**：自 <span style="color: Gold;">极</span>点引出的射线 $Ox$。
- **<span style="color: Gold;">极</span>坐标系**：选定长度单位、角度单位与正方向（通常为逆时针）建立的坐标系。
- **<span style="color: Gold;">极</span>径**：设 $M$ 为平面一点， <span style="color: Gold;">极</span>点 $O$ 与 $M$ 的距离 $|OM|$，记为 $\rho$。
- **<span style="color: Gold;">极</span>角**：以 <span style="color: Gold;">极</span>轴 $Ox$ 为始边，射线 $OM$ 为终边的角 $\angle xOM$ 为 $M$ 的 <span style="color: Gold;">极</span>角，记为 $\theta$。
- **<span style="color: Gold;">极</span>坐标**：有序数对 $\rho$、$\theta$ 为 $M$ 的 <span style="color: Gold;">极</span>坐标，记为 $M(\rho, \theta)$。

</ul>

#### <span style="color: silver;"><span style="color: Gold;">极</span>坐标系转换

<ul>

设 $M$ 为平面一点，直角坐标为 $(x, y)$， <span style="color: Gold;">极</span>坐标为 $(\rho, \theta)$，其关系是：

$$
\begin{cases}
x = \rho \cos \theta \\
y = \rho \sin \theta
\end{cases}
\text{，}
\begin{cases}
\rho^2 = x^2 + y^2 \\
\tan \theta = \dfrac{y}{x} (x \neq 0)
\end{cases}
$$

</ul>

#### <span style="color: silver;">常用 <span style="color: Gold;">极</span>坐标方程

<ul>

**直线的 <span style="color: Gold;">极</span>坐标方程：**

- 从 <span style="color: Gold;">极</span>点 $O$ 发出的一条射线：$\tan \theta = k$（由于 $k$ 符号未知，不能直接转为反三角~ ）。
- 过点 $(a, 0)$ 且垂直于 <span style="color: Gold;">极</span>轴的直线：$\rho = a \sec \theta = \dfrac{a}{\cos \theta}$。
- 过点 $\left(a, \dfrac{\pi}{2}\right)$ 且平行于 <span style="color: Gold;">极</span>轴的直线：$\rho = a \csc \theta = \dfrac{a}{\sin \theta}$。

**圆的 <span style="color: Gold;">极</span>坐标方程：**

- 圆心为 <span style="color: Gold;">极</span>点，半径为 $r$ 的圆：$\rho = r$。
- 圆心 $O'(r, 0)$，半径为 $r$ 的圆：$\rho = 2r \cos \theta$。
- 圆心 $O'\left(r, \dfrac{\pi}{2}\right)$，半径为 $r$ 的圆：$\rho = 2r \sin \theta$。

**抛物线的 <span style="color: Gold;">极</span>坐标方程：**

- $y = ax^2$：$\rho = \dfrac{1}{a} \tan \theta \sec \theta$。
- $y^2 = ax$：$\rho = a \cot \theta \csc \theta$。

</ul>

</ul>

### <span style="color: silver;">描点法

<ul>

#### <span style="color: silver;">心形线（外摆线）

<ul>

心形线又称为心脏线，表示一个圆上的固定一点在它绕着与其相切且半径相同的另一个圆周滚动时所形成的轨迹。

**表达式**：水平为 $r = a (1 \pm \cos \theta)$，垂直为 $r = a (1 \pm \sin \theta)$。一般为 $r = a (1 - \cos \theta)$（如下图所示），若符号为 $+$ 则心尖开口向左。

其中 $r$ 为线的 <span style="color: Gold;">极</span>径，$\theta$ 为 <span style="color: Gold;">极</span>角，$a$ 为形状参数且 $a > 0$，周期为 $2\pi$。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9rjjk8m4hh.png)
*图像描述：心形曲线，起点在原点，心尖向下，与两个相切圆相关。*

**直角坐标系下表达式**：$x^2 + y^2 + a \cdot x = a \cdot \sqrt{x^2 + y^2}$ 和 $x^2 + y^2 - a \cdot x = a \cdot \sqrt{x^2 + y^2}$。

**参数方程**：$x = a \cdot (2 \cdot \cos(t) - \cos(2 \cdot t))$，$y = a \cdot (2 \cdot \sin(t) - \sin(2 \cdot t))$。

**水平心形线对应参数表：**

| $\theta$      | $0$ | $\dfrac{\pi}{6}$       | $\dfrac{\pi}{4}$       | $\dfrac{\pi}{3}$ | $\dfrac{\pi}{2}$ | $\dfrac{2\pi}{3}$ | $\dfrac{3\pi}{4}$       | $\dfrac{5\pi}{6}$       | $\pi$ |
|---------------|-----|------------------------|------------------------|------------------|------------------|-------------------|-------------------------|-------------------------|-------|
| $r$           | $0$ | $\dfrac{2-\sqrt{3}}{2}a$ | $\dfrac{2-\sqrt{2}}{2}a$ | $\dfrac{1}{2}a$  | $a$             | $\dfrac{3}{2}a$   | $\dfrac{2+\sqrt{2}}{2}a$ | $\dfrac{2+\sqrt{3}}{2}a$ | $2a$  |

</ul>

#### <span style="color: silver;">玫瑰线

<ul>

**表达式**：$r = a \sin(n \theta)$，周期为 $\dfrac{2\pi}{n}$。

当 $n=3$ 时为三叶，$n=2$ 时为四叶，$n=\dfrac{3}{2}$ 时为六叶。三叶时周期为 $\dfrac{2\pi}{3}$。

**直角坐标系下表达式**：$x = a \cdot \sin(n \cdot \theta) \cdot \cos(\theta)$，$y = a \cdot \sin(n \cdot \theta) \cdot \sin(\theta)$。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.3k85k2qjmc.png)
*图像描述：三叶玫瑰线，中心在原点，三片花瓣对称分布。*

**三叶玫瑰线对应参数表：**

| $\theta$      | $0$ | $\dfrac{\pi}{12}$     | $\dfrac{\pi}{6}$ | $\dfrac{\pi}{4}$      | $\dfrac{\pi}{3}$ | $\dfrac{5\pi}{12}$    | $\dfrac{\pi}{2}$ | $\dfrac{7\pi}{12}$    | $\dfrac{3\pi}{2}$ |
|---------------|-----|-----------------------|------------------|-----------------------|------------------|-----------------------|------------------|-----------------------|-------------------|
| $r$           | $0$ | $\dfrac{\sqrt{2}}{2}a$ | $a$             | $\dfrac{\sqrt{2}}{2}a$ | $0$             | $-\dfrac{\sqrt{2}}{2}a$ | $-a$            | $-\dfrac{\sqrt{2}}{2}a$ | $0$              |

</ul>

#### <span style="color: silver;">阿基米德螺线

<ul>

**表达式**：$r = a \theta$，其中 $a > 0$，$\theta \geqslant 0$ 由 0 开始增大时 $r$ 也在不断增大。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.99thvnl2r9.png)
*图像描述：从原点开始向外扩展的螺旋线，间距均匀。*

</ul>

#### <span style="color: silver;">伯努利双扭线

<ul>

设定线段 $F_1 F_2$ 长度为 $2a$，伯努利双扭线上所有点 $M$ 满足 $MF_1 \cdot MF_2 = a^2$。

**表达式**：$r^2 = 2a^2 \cos 2\theta$ 或 $r^2 = 2a^2 \sin 2\theta$。

**直角坐标系下表达式**：$(x^2 + y^2)^2 = 2a^2 (x^2 - y^2)$。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.6wqveg7o33.png)
*图像描述：两个图像展示 $r^2 = 2a^2 \cos 2\theta$（水平 8 字形）和 $r^2 = 2a^2 \sin 2\theta$（垂直 8 字形）。*

</ul>

</ul>

### <span style="color: silver;">直角坐标系下画 <span style="color: Gold;">极</span>坐标图像

<ul>

令 $\theta$ 为 $x$，令 $r$ 为 $y$。如心形线 $r = 2(1 - \cos \theta)$：

按直角坐标系的图就可以计算出对应的 $r$ 从而能画出对应的图像。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.1zieklu1vy.png)
*图像描述：曲线从 (0, 0) 开始，上升至峰值后回落，形似心形线的直角坐标表示。*

</ul>

</ul>

## <span style="color: silver;">参数法

<ul>

如果很难使用直角坐标或 <span style="color: Gold;">极</span>坐标表示曲线，可以引入一个新的变量参数来表示，即得到参数方程：

$$
\begin{cases}
x = x(t) \\
y = y(t)
\end{cases}
$$

### <span style="color: silver;">摆线（平摆线）

<ul>

摆线，又称旋轮线、圆滚线，是一个圆沿一条直线滚动时，圆边界上一定点所形成的轨迹。

令圆半径为 $r$，摆点与圆心所成直线所转动夹角对应弧度为 $t$，其中 $t \in [0, 2\pi]$，所对应参数方程为：

$$
\begin{cases}
x = r (t - \sin t) \\
y = r (1 - \cos t)
\end{cases}
$$

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.7lk4ygvxqe.png)
*图像描述：波浪形曲线，从原点开始，展示圆滚动时的轨迹，圆心和摆点位置标注。*

</ul>

### <span style="color: silver;">星形线（内摆线）

<ul>

与半径为 $r$ 的定圆内切的半径为 $\dfrac{r}{4}$ 的动圆沿定圆无滑动地滚动，动圆上一点的轨迹称为星形线。

令 $t$ 表示摆点与圆心的连线所构成夹角的弧度，其中 $t \in [0, 2\pi]$，得对应参数方程：

$$
\begin{cases}
x = r \cos^3 t \\
y = r \sin^3 t
\end{cases}
$$

由 $\cos^2 t + \sin^2 t = 1$ 得到直角坐标方程：$x^{\dfrac{2}{3}} + y^{\dfrac{2}{3}} = r^{\dfrac{2}{3}}$。

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.6f0tpv77qd.png)
*图像描述：四角星形曲线，中心在原点，与定圆和动圆相关。*

</ul>

</ul>

</ul>

# <span style="color: silver;">常用基础知识

<ul>

## <span style="color: silver;">数列

<ul>

### <span style="color: silver;">等差数列

<ul>

首项为 $a_1$，公差为 $d (d \neq 0)$ 的数列：$a_1, a_1 + d, a_1 + 2d, \dots, a_1 + (n-1)d$。

**通项公式**：$a_n = a_1 + (n-1)d$。

**前 $n$ 项和**：$S_n = \dfrac{n}{2} [2a_1 + (n-1)d] = \dfrac{n}{2} (a_1 + a_n)$。

</ul>

### <span style="color: silver;">等比数列

<ul>

首项为 $a_1$，公比为 $q (q \neq 0)$ 的数列：$a_1, a_1 q, a_1 q^2, \dots, a_1 q^{n-1}$。

**通项公式**：$a_n = a_1 q^{n-1}$。

**前 $n$ 项和**：

$$
S_n = \begin{cases}
n a_1, & r = 1 \\
\dfrac{a_1 (1 - r^n)}{1 - r}, & r \neq 1
\end{cases}
$$

若首项为 1，则 $1 + r + r^2 + \cdots + r^{n-1} = \dfrac{1 - r^n}{1 - r} (r \neq 1)$。

对无穷的 <span style="color: Gold;">极</span>限为 $\dfrac{1}{1 - r}$。

</ul>

### <span style="color: silver;">常见数列前 $n$ 项和

<ul>

1. $\sum_{k=1}^n k = 1 + 2 + \cdots + n = \dfrac{n (n+1)}{2}$。
2. $\sum_{k=1}^n k^2 = 1^2 + 2^2 + \cdots + n^2 = \dfrac{n (n+1) (2n+1)}{6}$。
3. $\sum_{k=1}^n \dfrac{1}{k (k+1)} = \dfrac{1}{1 \times 2} + \dfrac{1}{2 \times 3} + \cdots + \dfrac{1}{n (n+1)} = \dfrac{n}{n+1}$。

</ul>

</ul>

## <span style="color: silver;">三角~

<ul>

### <span style="color: silver;">基本关系

<ul>

$\csc \alpha = \dfrac{1}{\sin \alpha}$，$\sec \alpha = \dfrac{1}{\cos \alpha}$，$\cot \alpha = \dfrac{1}{\tan \alpha}$，$\tan \alpha = \dfrac{\sin \alpha}{\cos \alpha}$，$\cot \alpha = \dfrac{\cos \alpha}{\sin \alpha}$。

$\sin^2 \alpha + \cos^2 \alpha = 1$，$1 + \tan^2 \alpha = \sec^2 \alpha$，$1 + \cot^2 \alpha = \csc^2 \alpha$。

$\cos^2 \alpha = 1 - \sin^2 \alpha = (1 + \sin \alpha)(1 - \sin \alpha)$，$\sin^2 \alpha = 1 - \cos^2 \alpha = (1 + \cos \alpha)(1 - \cos \alpha)$。

</ul>

### <span style="color: silver;">诱导公式

<ul>

奇变偶不变，符号看象限。奇指前面添加的常数项是否为 $\pi$ 的整数倍，是则需改变~ ；看象限指添加常数后整体的符号依~ 所在象限确定。

1. $\sin \left( \dfrac{\pi}{2} \pm \alpha \right) = \cos \alpha$
2. $\cos \left( \dfrac{\pi}{2} \pm \alpha \right) = \mp \sin \alpha$
3. $\sin (\pi \pm \alpha) = \mp \sin \alpha$
4. $\cos (\pi \pm \alpha) = -\cos \alpha$

</ul>

### <span style="color: silver;">倍角公式

<ul>

$\sin 2\alpha = 2 \sin \alpha \cos \alpha$，  
$\cos 2\alpha = \cos^2 \alpha - \sin^2 \alpha = (\sin \alpha + \cos \alpha)(\cos \alpha - \sin \alpha) = 1 - 2 \sin^2 \alpha = 2 \cos^2 \alpha - 1$。

$1 + \sin 2\alpha = (\sin \alpha + \cos \alpha)^2$，$1 - \sin 2\alpha = (\sin \alpha - \cos \alpha)^2$。

$\sin 3\alpha = -4 \sin^3 \alpha + 3 \sin \alpha$，$\cos 3\alpha = 4 \cos^3 \alpha - 3 \cos \alpha$。

$\tan 2\alpha = \dfrac{2 \tan \alpha}{1 - \tan^2 \alpha}$，$\cot 2\alpha = \dfrac{\cot^2 \alpha - 1}{2 \cot \alpha}$。

</ul>

### <span style="color: silver;">半角公式

<ul>

$\sin^2 \dfrac{\alpha}{2} = \dfrac{1}{2} (1 - \cos \alpha)$，$\cos^2 \dfrac{\alpha}{2} = \dfrac{1}{2} (1 + \cos \alpha)$（降幂公式）。

$\sin \dfrac{\alpha}{2} = \pm \sqrt{\dfrac{1 - \cos \alpha}{2}}$，$\cos \dfrac{\alpha}{2} = \pm \sqrt{\dfrac{1 + \cos \alpha}{2}}$。

$\tan \dfrac{\alpha}{2} = \dfrac{1 - \cos \alpha}{\sin \alpha} = \dfrac{\sin \alpha}{1 + \cos \alpha} = \pm \sqrt{\dfrac{1 - \cos \alpha}{1 + \cos \alpha}} = \dfrac{1}{\cot \dfrac{\alpha}{2}}$。

</ul>

### <span style="color: silver;">和差公式

<ul>

$\sin$ 和 $\tan$ 的和差公式更容易考到。

$\sin (\alpha \pm \beta) = \sin \alpha \cos \beta \pm \cos \alpha \sin \beta$，  
$\cos (\alpha \pm \beta) = \cos \alpha \cos \beta \mp \sin \alpha \sin \beta$。

$\tan (\alpha \pm \beta) = \dfrac{\tan \alpha \pm \tan \beta}{1 \mp \tan \alpha \tan \beta}$，  
$\cot (\alpha \pm \beta) = \dfrac{\cot \alpha \cot \beta \mp 1}{\cot \beta \pm \cot \alpha}$。

</ul>

### <span style="color: silver;">积化和差公式

<ul>

和差化积与积化和差不需要背，都是和差公式的推导。

$\sin \alpha \cos \beta = \dfrac{1}{2} [\sin (\alpha + \beta) + \sin (\alpha - \beta)]$，  
$\cos \alpha \sin \beta = \dfrac{1}{2} [\sin (\alpha + \beta) - \sin (\alpha - \beta)]$。

$\cos \alpha \cos \beta = \dfrac{1}{2} [\cos (\alpha + \beta) + \cos (\alpha - \beta)]$，  
$\sin \alpha \sin \beta = \dfrac{1}{2} [\cos (\alpha - \beta) - \cos (\alpha + \beta)]$。

</ul>

### <span style="color: silver;">和差化积公式

<ul>

$\sin \alpha + \sin \beta = 2 \sin \dfrac{\alpha + \beta}{2} \cos \dfrac{\alpha - \beta}{2}$，  
$\sin \alpha - \sin \beta = 2 \sin \dfrac{\alpha - \beta}{2} \cos \dfrac{\alpha + \beta}{2}$。

$\cos \alpha + \cos \beta = 2 \cos \dfrac{\alpha + \beta}{2} \cos \dfrac{\alpha - \beta}{2}$，  
$\cos \alpha - \cos \beta = -2 \sin \dfrac{\alpha + \beta}{2} \sin \dfrac{\alpha - \beta}{2}$。

**推理和差化积公式（以第一个为例）：**

$$
\sin \alpha + \sin \beta = \sin \left( \dfrac{\alpha + \beta}{2} + \dfrac{\alpha - \beta}{2} \right) + \sin \left( \dfrac{\alpha + \beta}{2} - \dfrac{\alpha - \beta}{2} \right) = \\
\sin \dfrac{\alpha + \beta}{2} \cos \dfrac{\alpha - \beta}{2} + \cos \dfrac{\alpha + \beta}{2} \sin \dfrac{\alpha - \beta}{2} + \sin \dfrac{\alpha + \beta}{2} \cos \dfrac{\alpha - \beta}{2} - \cos \dfrac{\alpha + \beta}{2} \sin \dfrac{\alpha - \beta}{2} = \\
2 \sin \dfrac{\alpha + \beta}{2} \cos \dfrac{\alpha - \beta}{2}
$$

</ul>

### <span style="color: silver;">万能公式

<ul>

可视为特殊的倍角公式，将单角变为半角。

若 $u = \tan \dfrac{x}{2} (-\pi < x < \pi)$，则 $\sin x = \dfrac{2u}{1 + u^2}$，$\cos x = \dfrac{1 - u^2}{1 + u^2}$。

</ul>

### <span style="color: silver;">辅助角公式

<ul>

$a \sin x + b \cos x = \sqrt{a^2 + b^2} \sin (x + \phi)$，  
其中 $\sin \phi = \dfrac{b}{\sqrt{a^2 + b^2}}$，$\cos \phi = \dfrac{a}{\sqrt{a^2 + b^2}}$。

</ul>

### <span style="color: silver;">正弦定理

<ul>

$\dfrac{a}{\sin A} = \dfrac{b}{\sin B} = \dfrac{c}{\sin C}$。

</ul>

### <span style="color: silver;">余弦定理

<ul>

$a^2 = b^2 + c^2 - 2bc \cos A$，  
$b^2 = a^2 + c^2 - 2ac \cos B$，  
$c^2 = a^2 + b^2 - 2ab \cos C$。

</ul>

### <span style="color: silver;">三角形面积公式

<ul>

$S_{\triangle ABC} = \dfrac{1}{2} bc \sin A = \dfrac{1}{2} ac \sin B = \dfrac{1}{2} ab \sin C$。

</ul>

### <span style="color: silver;">海伦公式

<ul>

$S_{\triangle ABC} = \sqrt{p (p - a)(p - b)(p - c)}$，其中 $p = \dfrac{a + b + c}{2}$。

</ul>

</ul>

## <span style="color: silver;">反三角~

<ul>

因为只有单调~ 才有反~ ，所以对于三角~ 必须选取其单调区间才有反~ 。一般只讨论三角~ 在其主值区间上的反~ （主值区间即包括锐角最大的单调区间）。

可以画单位圆直观思考。

### <span style="color: silver;">反正弦~

<ul>

正弦~ $y = \sin x$ 在主值区间 $\left[-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right]$ 上的反~ 为反正弦~ ，记为 $y = \arcsin x$ 或 $y = \sin^{-1} x$。表示其区间上正弦值等于 $x$ 的一个角。

反正弦~ 与正弦~ 图像一样，都是关于原点对称、严格单调递增、有界的奇~ 。

- 当 $x \in [-1, 1]$ 时，$\arcsin (-x) = -\arcsin x$。
- 当 $x \in \left[-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right]$ 时，$\arcsin (\sin x) = x$。
- 当 $x \in [-1, 1]$ 时，$\sin (\arcsin x) = x$。

</ul>

### <span style="color: silver;">反余弦~

<ul>

余弦~ $y = \cos x$ 在主值区间 $[0, \pi]$ 上的反~ 为反余弦~ ，记为 $y = \arccos x$ 或 $y = \cos^{-1} x$。表示其区间上余弦值等于 $x$ 的一个角。

反余弦~ 是严格单调递减、有界的非奇非偶~ ，图像关于 $\left(0, \dfrac{\pi}{2}\right)$ 对称。

- 因为关于 $\left(0, \dfrac{\pi}{2}\right)$ 对称，若 $x_1, x_2 \in (-1, 1)$，$x_1 = -x_2$，则 $\arccos x_1 + \arccos x_2 = \pi$。
- 当 $x \in (-1, 1)$ 时，$\arccos (-x) + \arccos x = \pi$。
- 当 $x \in [0, \pi]$ 时，$\arccos (\cos x) = x$。
- 当 $x \in [-1, 1]$ 时，$\cos (\arccos x) = x$。
- 当 $x \in [-1, 1]$ 时，$\sin (\arccos x) = \sqrt{1 - x^2}$。  
  证明：令 $u = \arccos x \in [0, \pi]$，则 $\cos u = x$，从而 $\sin (\arccos x) = \sin u = \sqrt{1 - \cos^2 u} = \sqrt{1 - x^2}$。
- 同理，$\cos (\arcsin x) = \sqrt{1 - x^2}$。
- $\arcsin x + \arccos x = \dfrac{\pi}{2}$（证明需分三种情况，这里略）。

</ul>

### <span style="color: silver;">反正切~

<ul>

正切~ $y = \tan x$ 在主值区间 $\left[-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right]$ 上的反~ 为反正切~ ，记为 $y = \arctan x$ 或 $y = \tan^{-1} x$。表示其区间上正切值等于 $x$ 的一个角。

正切~ 是关于原点对称、严格单调递增、有界的奇~ 。值域为 $\left(-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right)$，定义域为 $(-\infty, +\infty)$。

- 当 $x \in (-\infty, +\infty)$ 时，$\arctan (-x) = -\arctan x$。
- 当 $x \in \left(-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right)$ 时，$\arctan (\tan x) = x$。
- 当 $x \in (-\infty, +\infty)$ 时，$\tan (\arctan x) = x$。

**例题：** 求 $\arctan \dfrac{1}{2} + \arctan \dfrac{1}{3}$ 的值。

**解：**  
由于求反正切~ 不便，直接转换为正切~ 求解。  
令 $\arctan \dfrac{1}{2} = \alpha$，$\arctan \dfrac{1}{3} = \beta$，则 $\tan \alpha = \dfrac{1}{2}$，$\tan \beta = \dfrac{1}{3}$。  
由反正切~ 定义，$\alpha, \beta \in \left(-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right)$，$\alpha + \beta \in (-\pi, \pi)$。  
利用和差公式：  
$\tan (\alpha + \beta) = \dfrac{\tan \alpha + \tan \beta}{1 - \tan \alpha \tan \beta} = \dfrac{\dfrac{1}{2} + \dfrac{1}{3}}{1 - \dfrac{1}{2} \cdot \dfrac{1}{3}} = \dfrac{\dfrac{5}{6}}{\dfrac{5}{6}} = 1$。  
即 $\alpha + \beta = \dfrac{\pi}{4}$，故 $\arctan \dfrac{1}{2} + \arctan \dfrac{1}{3} = \dfrac{\pi}{4}$。

</ul>

### <span style="color: silver;">反余切~

<ul>

余切~ $y = \cot x$ 在主值区间 $[0, \pi]$ 上的反~ 为反余切~ ，记为 $y = \textrm{arccot}\,x$ 或 $y = \cot^{-1} x$。表示其区间上余切值等于 $x$ 的一个角。

余切~ 是关于 $\left(0, \dfrac{\pi}{2}\right)$ 中心对称、严格单调递减、有界的非奇非偶~ 。值域为 $(0, \pi)$，定义域为 $(-\infty, +\infty)$。

- 当 $x \in (-\infty, +\infty)$ 时，$\textrm{arccot} (-x) = \pi - \textrm{arccot}\,x$。
- 当 $x \in \left(-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right)$ 时，$\textrm{arccot} (\cot x) = x$。
- 当 $x \in (-\infty, +\infty)$ 时，$\cot (\textrm{arccot}\,x) = x$。
- 当 $x \in (-\infty, 0) \cup (0, +\infty)$ 时，$\tan (\textrm{arccot}\,x) = \dfrac{1}{x}$，$\cot (\arctan x) = \dfrac{1}{x}$。
- 当 $x \in (-\infty, +\infty)$ 时，$\arctan x + \textrm{arccot}\,x = \dfrac{\pi}{2}$。

</ul>

</ul>

## <span style="color: silver;">指数运算法则

<ul>

$a^{\alpha} \cdot a^{\beta} = a^{\alpha + \beta}$，$\dfrac{a^{\alpha}}{a^{\beta}} = a^{\alpha - \beta}$，$(a^{\alpha})^{\beta} = a^{\alpha \beta}$，$(ab)^{\alpha} = a^{\alpha} b^{\alpha}$，$\left(\dfrac{a}{b}\right)^{\alpha} = \dfrac{a^{\alpha}}{b^{\alpha}}$。

其中 $a$，$b$ 为正实数，$\alpha$，$\beta$ 为任意实数。

</ul>

## <span style="color: silver;">对数运算法则

<ul>

**重点：**

1. $\log_a (MN) = \log_a M + \log_a N$（积的对数 = 对数的和）。
2. $\log_a \left(\dfrac{M}{N}\right) = \log_a M - \log_a N$（商的对数 = 对数的差）。
3. $\log_a M^n = n \log_a M$（幂的对数 = 对数的倍数）。
4. $\log_a \sqrt[n]{M} = \dfrac{1}{n} \log_a M$。

所以以后多项相乘、相除、乘方、开方都**取对数**进行化简。

对于分数相减的对数先**通分**再进行对数减法。

**例题：** 证明 $\dfrac{1}{x + 1} < \ln \left(1 + \dfrac{1}{x}\right) < \dfrac{1}{x}$，其中 $x > 0$。

**证明：**  
因为中间项是对数，难以直接处理，先通分：  
$\ln \left(1 + \dfrac{1}{x}\right) = \ln \dfrac{x + 1}{x} = \ln (x + 1) - \ln x$。  
要证明中间式在一个区间内成立，考虑拉格朗日中值定理：  
$f(b) - f(a) = f'(\xi) (b - a)$。  
令 $f(x) = \ln x$，则 $f'(x) = \dfrac{1}{x}$，  
$\ln (x + 1) - \ln x = f'(x) = \dfrac{1}{\xi}$，其中 $x < \xi < x + 1$。  
因 $x > 0$，则 $\dfrac{1}{x + 1} < \dfrac{1}{\xi} < \dfrac{1}{x}$，  
故 $\dfrac{1}{x + 1} < \ln \left(1 + \dfrac{1}{x}\right) < \dfrac{1}{x}$ 成立。

</ul>

## <span style="color: silver;">一元二次方程基础

<ul>

1. 基本格式为 $ax^2 + bx + c = 0 (a \neq 0)$。
2. 如果 $\Delta = \sqrt{b^2 - 4ac} \geqslant 0$，根的公式为 $x_{1,2} = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a}$，  
   - 若 $\Delta = 0$，为唯一实根；  
   - 若 $\Delta > 0$，为二重实根；  
   - 若 $\Delta < 0$，则得到共轭复数根 $-\dfrac{b}{2a} \pm \dfrac{\sqrt{4ac - b^2}}{2a} i$。
3. 根与系数的关系（韦达定理）：$x_1 + x_2 = -\dfrac{b}{a}$，$x_1 x_2 = \dfrac{c}{a}$。
4. 抛物线顶点为 $\left(-\dfrac{b}{2a}, c - \dfrac{b^2}{4a}\right)$。

</ul>

## <span style="color: silver;">因式分解公式

<ul>

重点为 3、4、7 和 11 的公式。

1. $(a + b)^2 = a^2 + 2ab + b^2$。
2. $(a - b)^2 = a^2 - 2ab + b^2$。
3. $(a + b)^3 = a^3 + 3a^2 b + 3ab^2 + b^3$。
4. $(a - b)^3 = a^3 - 3a^2 b + 3ab^2 - b^3$。
5. $a^2 - b^2 = (a + b)(a - b)$。
6. $a^3 - b^3 = (a - b)(a^2 + ab + b^2)$。
7. $a^3 + b^3 = (a + b)(a^2 - ab + b^2)$。
8. $n$ 为正整数时，$a^n - b^n = (a - b)(a^{n-1} + a^{n-2} b + \cdots + ab^{n-2} + b^{n-1})$。
9. $n$ 为正偶数时，$a^n - b^n = (a + b)(a^{n-1} - a^{n-2} b + \cdots + ab^{n-2} - b^{n-1})$。
10. $n$ 为正奇数时，$a^n + b^n = (a + b)(a^{n-1} - a^{n-2} b + \cdots - ab^{n-2} + b^{n-1})$。
11. 二项式定理：  
    $(a + b)^n = \sum_{k=0}^n C_n^k a^{n-k} b^k = a^n + n a^{n-1} b + \dfrac{n (n-1)}{2!} a^{n-2} b^2 + \cdots + \dfrac{n (n-1) \cdots (n-k+1)}{k!} a^{n-k} b^k + \cdots + n a b^{n-1} + b^n$。

对于二项式定理需记忆，杨辉三角形可帮助记忆系数：

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.3rbdfif1pb.png)

</ul>

## <span style="color: silver;">阶乘与双阶乘

<ul>

1. $n! = 1 \times 2 \times 3 \times \cdots \times n$，其中 $0! = 1$。
2. $(2n)!! = 2 \times 4 \times 6 \times \cdots \times (2n) = 2^n \cdot n!$。
3. $(2n-1)!! = 1 \times 3 \times 5 \times \cdots \times (2n-1)$。

**例题：** 计算 $\int_0^{\dfrac{\pi}{2}} \sin^{10} x \, dx$ 与 $\int_0^{\dfrac{\pi}{2}} \cos^9 x \, dx$。

**解：**  
- 原式 1 为偶数次幂：  
  $\dfrac{9}{10} \cdot \dfrac{7}{8} \cdot \dfrac{5}{6} \cdot \dfrac{3}{4} \cdot \dfrac{1}{2} \cdot \dfrac{\pi}{2} = \dfrac{\pi}{2} \cdot \dfrac{9!!}{10!!}$。  
- 原式 2 为奇数次幂：  
  $\dfrac{8}{9} \cdot \dfrac{6}{7} \cdot \dfrac{4}{5} \cdot \dfrac{2}{3} = \dfrac{8!!}{9!!}$。

</ul>

## <span style="color: silver;">常用 <span style="color: GreenYellow;">不等式

<ul>

very important

### <span style="color: silver;">绝对值 -

<ul>

若 $a$，$b$ 为实数，则：

1. $|a \pm b| \leqslant |a| + |b|$。
2. 推广到离散区间：$|a_1 \pm a_2 \pm a_3 \pm \cdots \pm a_n| \leqslant |a_1| + |a_2| + \cdots + |a_n|$。
3. 推广到连续区间且 $f(x)$ 在 $[a, b] (a < b)$ 上可积：$\left| \int_a^b f(x) \, dx \right| \leqslant \int_a^b |f(x)| \, dx$。
   - 原因：符号不一定相同的面积代数和一定小于同为正的面积代数和。
4. $||a| - |b|| \leqslant |a - b|$。  
   - 后式为两点之差，前式为 $a$、$b$ 与 0 间距离的差，若异号则抵消一部分，若同号则等于后式。

</ul>

### <span style="color: silver;">根号 -

<ul>

公式 1 非常重要，即算术平均值大于几何平均值。

$a, b, c > 0$：

1. $\sqrt{ab} \leqslant \dfrac{a + b}{2} \leqslant \sqrt{\dfrac{a^2 + b^2}{2}}$。
2. $\sqrt[3]{abc} \leqslant \dfrac{a + b + c}{3} \leqslant \dfrac{a^2 + b^2 + c^2}{3}$。

**例题：** 证明~ $f(x) = \dfrac{x}{1 + x^2}$ 在 $(-\infty, +\infty)$ 内有界。

**证明：**  
可以用 <span style="color: Gold;">极</span>限证明，这里使用有界性定义与 - 完成。  
① 当 $x = 0$ 时，$f(0) = \dfrac{0}{1} = 0$，有界。  
② 当 $x \neq 0$ 时，$f(x) = \dfrac{\dfrac{x}{x}}{\dfrac{1 + x^2}{x}} = \dfrac{1}{\dfrac{1}{x} + x}$。  
因需证明有界性，且根号 - 要求参数大于 0，故证明：  
$|f(x)| = \dfrac{1}{\dfrac{1}{|x|} + |x|} \leqslant M$。  
由 $\dfrac{a + b}{2} \geqslant \sqrt{ab}$，得 $\dfrac{\dfrac{1}{|x|} + |x|}{2} \geqslant \sqrt{\dfrac{1}{|x|} \cdot |x|} = 1$，  
则 $|f(x)| = \dfrac{1}{\dfrac{1}{|x|} + |x|} \leqslant \dfrac{1}{2}$。  
故~ 在 $\mathbb{R}$ 上有界。

</ul>

### <span style="color: silver;">指数 -

<ul>

设 $a > b > 0$，则：

$$
\begin{cases}
a^n > b^n, & \text{当 } n > 0 \\
a^n < b^n, & \text{当 } n < 0
\end{cases}
$$

$e^x \geqslant x + 1 (\forall x)$。

</ul>

### <span style="color: silver;">分数 -

<ul>

若 $0 < a < x < b$，$0 < c < y < d$，则 $\dfrac{c}{b} < \dfrac{y}{x} < \dfrac{d}{a}$。

</ul>

### <span style="color: silver;">三角 -

<ul>

1. $\sin x < x < \tan x (0 < x < \dfrac{\pi}{2})$。
2. $\sin x < x (x > 0)$。
3. $\arctan x \leqslant x \leqslant \arcsin x (0 \leqslant x \leqslant 1)$。

</ul>

### <span style="color: silver;">对数 -

<ul>

1. $x - 1 \geqslant \ln x (x > 0)$。
2. $\dfrac{1}{1 + x} < \ln \left(1 + \dfrac{1}{x}\right) < \dfrac{1}{x} (x > 0)$。

</ul>

</ul>

</ul>

</ul>