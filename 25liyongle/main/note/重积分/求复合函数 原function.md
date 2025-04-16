<div style="float: left; width: 64%; padding: 1%;">

### 问题重述


$$ \iint\limits_D \sqrt{y^2 - xy} \, dxdy $$
 $ D $ 是由直线 $ y = x $、$ y = 1 $、$ x = 0 $ 所围成的平面区域


### 原函数的求解

$ \int \sqrt{y^2 - xy} \, dx $ 的原函数

换元法：
<ul>

设 $ u = y^2 - xy $，则 $ du = -y dx $，即 $ dx = -\frac{du}{y} $。

因此：
$$ \int \sqrt{y^2 - xy} \, dx = \int \sqrt{u} \left( -\frac{du}{y} \right) = -\frac{1}{y} \int u^{1/2} \, du = -\frac{1}{y} \cdot \frac{2}{3} u^{3/2} + C $$
$$ = -\frac{2}{3y} (y^2 - xy)^{3/2} + C $$

</ul>

代入区间：
$$ \left[ -\frac{2}{3y} (y^2 - xy)^{3/2} \right]_0^y = -\frac{2}{3y} (0 - y^3) = \frac{2}{3} y^2 $$



</div>
<div style="float: right; width: 26%; padding: 1%;">

对于较为复杂的, 还是不要硬凑, 还是用换元法找令u=f 或 $u=\sqrt{f}
$ 等

 <span style="color: silver;">其实还是 一元积分的base计算</span>


</div>
<div style="clear: both;"></div>
