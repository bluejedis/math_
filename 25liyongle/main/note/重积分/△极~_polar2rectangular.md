

<div style="float: left; width: 64%; padding: 1%;">

##  <span style="color: silver;">极 → 直


$$ \int_{0}^{\frac{\pi}{2}} d\theta \int_{0}^{\cos\theta} f(r\cos\theta, r\sin\theta) r dr $$
极 $\rightarrow$ rectangular

---

###  <span style="color: silver;">① draw $D$ (polar)


$\theta \in [0, \frac{\pi}{2}]$ ← Ⅰ quatrant

 $r \in [0, \cos\theta]$ ← $D$ 完整

- 特殊点：
$r = 2a\cos\theta$ → $a = \frac{r}{2\cos\theta}$
又$r=\cos\theta$ → $a = \frac{1}{2}$

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9nzzdz0gbx1.969xpebxjg.png)

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; | 
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; | *correspond rectangular*
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; ↓
![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9nzzdz0gbx2.7egyuhsknh.png)

---

###  <span style="color: silver;">② range: x, y

discuss积分次序： $\int dy \int dx$ or $\int dx \int dy$

<div style="display: flex; justify-content: space-between;">
<div style="flex: 1; padding-right: 10px; border-right: 1px solid #ccc;">

####  <span style="color: silver;">1) 先对 $x$ 积分，再对 $y$ 积分 ($\int dy \int dx$)


![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9nzzdz0gbx_x.39ldidveku.png)

* (y 范围确定)
  *  $y$ 表示 $x$ 的取值范围。
      - ↑
  * use semicycle的 rectangular 方程
- $(x-x_0)^2+(y-y_0)^2=a^2$
    - $$ (x - \frac{1}{2})^2 + y^2 = \left(\frac{1}{2}\right)^2 = \frac{1}{4} $$
    解$x$:
    $$ (x - \frac{1}{2})^2 = \frac{1}{4} - y^2 $$
    $$ x - \frac{1}{2} = \pm \sqrt{\frac{1}{4} - y^2} $$
    $$ x = \frac{1}{2} \pm \sqrt{\frac{1}{4} - y^2} $$


* 积分形式：
    $$ \int_{0}^{\frac{1}{2}} dy \int_{\frac{1}{2} - \sqrt{\frac{1}{4} - y^2}}^{\frac{1}{2} + \sqrt{\frac{1}{4} - y^2}} f(x, y) dx $$

</div>
<div style="flex: 1; padding-left: 10px;">

####  <span style="color: silver;">2) 先对 $y$ 积分，再对 $x$ 积分 ($\int dx \int dy$)

![image](https://bluejedis.github.io/picx-images-hosting/Math/image.9nzzdz0gbx_y.2a5a57snez.png)
<br>
* (x 范围确定)
  * 用 $x$ 表示 $y$ 的取值范围。


* 推导 $y$ 的范围 (same equation):
    $$ (x - \frac{1}{2})^2 + y^2 = \frac{1}{4} $$
    解$y$:
    $$ y^2 = \frac{1}{4} - (x - \frac{1}{2})^2 $$
    $$ y^2 = \frac{1}{4} - x^2 + x - \frac{1}{4} $$
    $$ y^2 = -x^2 + x $$
    $$ y = \pm \sqrt{-x^2 + x} $$
* 由图可知 (abandon负)
    $$ \therefore y = \sqrt{-x^2 + x} $$
  * $y$ 的下界:$ y = 0 $
    
* 积分形式：
    $$ \int_{0}^{1} dx \int_{0}^{\sqrt{-x^2+x}} f(x, y) dy $$
</div>
</div>

</div>
<div style="float: right; width: 26%; padding: 1%;">
 <span style="color: silver;">

$(x - x_0)^2 + (y - y_0)^2 = {\bold {\color{darkred}{a}}}^2$
~~- <span style="font-size: 12px;"> 各坐标系的process 各自独立 ← 思路是对的~~    



</div>
<div style="clear: both;"></div>