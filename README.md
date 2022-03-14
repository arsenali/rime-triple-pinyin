# 三码拼音方案

配方： ℞ arsenali/rime-triple-pinyin

[Rime](https://rime.im/) 大致按“声、韵、调”三码输入一个带调音节，15键内无重音

## 安装

[东风破](https://github.com/rime/plum) 安装口令： <code> bash rime-install arsenali/rime-triple-pinyin </code>

本方案词库依赖于 [地球拼音](https://github.com/rime/rime-terra-pinyin) ℞ rime-terra-pinyin，安装本方案前请先安装 ℞ rime-terra-pinyin。

皮肤（主题）文件依赖于 [同文安卓輸入法平臺](https://github.com/osfans/trime) ℞ trime，安卓平台使用本方案前请先安装 ℞ trime。


## 简介

三码拼音是为方便在触屏手机上快速、准确地打字而设计的，方案原则包括：
键数要少（只使用15个按键），方便单手打字；
避免像九宫键一样的重复音节，以实现准确输入；
为准确输入，编码包括声调（也可使用无声调模式）；
易学易用。

编码方式为“声母+韵头韵腹+韵尾声调”，编码规则是：
第一码：23个声母合并在15个按键上，通过声、韵组合消除重复音节；
第二码：韵头（介母）分为无介母、i、u、ü四类，对应第二码的四个区域（123行和第5列）；
韵腹分为a(a,an,ang)、e(e,en,eng)、o(o,ou,ong)三类，剩下的ai,ei,ao归为第4类，对应四个区域中的4个按键；
第三码：韵尾分为空,n,ng三类，对应第三码的1-3行，声调分为1-4声和轻声5类，对应第三码的5列。

专用主题中默认使用动态键盘，会逐码提示下一码键位，可快速上手，熟练之后可使用三码拼音快打（静态键盘）模式，速度会快很多。

按三码拼音的编码规则，可设计出多种三拼方案，本项目中除“三码拼音”外，还初步设计了“三码拼音aoe”和“三码注音”两套派生方案，供不同用户选用。用户亦可根据自己的习惯设计出自己的三码拼音韵母布局。

---

详细介绍请看专用主题皮肤中的教程。

默认只载入地球拼音词库，需要用更多其他词库请到网盘或QQ群下载。

下载地址：http://www.lssp.ysepan.com/

或：https://pan.baidu.com/s/1i4X3WFz 密码: 1jpd

QQ群：[150478288](https://jq.qq.com/?_wv=1027&k=5wf1uTQ)


<br>

### &#8627; Stargazers
[![Stargazers repo roster for @arsenali/rime-triple-pinyin](https://reporoster.com/stars/arsenali/rime-triple-pinyin)](https://github.com/arsenali/rime-triple-pinyin/stargazers)

### &#8627; Forkers
[![Forkers repo roster for @arsenali/rime-triple-pinyin](https://reporoster.com/forks/arsenali/rime-triple-pinyin)](https://github.com/arsenali/rime-triple-pinyin/network/members)
