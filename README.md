# 三码拼音方案

配方： ℞ arsenali/rime-triple-pinyin

[Rime](https://rime.im/) 按“声、韵、调”的顺序三码输入一个带调音节，15键内无重音

## 安装

[东风破](https://github.com/rime/plum) 安装口令： <code> bash rime-install arsenali/rime-triple-pinyin </code>

本方案词库依赖于 [地球拼音](https://github.com/rime/rime-terra-pinyin) ℞ rime-terra-pinyin，安装本方案前请先安装 ℞ rime-terra-pinyin。

皮肤（主题）文件依赖于 [同文安卓輸入法平臺](https://github.com/osfans/trime) ℞ trime，安卓平台使用本方案前请先安装 ℞ trime。


## 简介

三码拼音是为方便在触屏手机上快速、准确地打字而设计的，方案原则包括：
1. 键数要少（只使用15个按键），方便单手打字；
2. 避免像九宫键一样的重复音节，以实现准确输入；
3. 为准确输入，编码包括声调（也可使用无声调模式）；
4. 易学易用。

<br>

编码方式为“声母+韵母+去重码&声调”，编码规则是：
- 第一码声母：23个声母合并在15键上，基本按照声母表顺序排列，方便记忆。其中部分声母共键，共键声母将在第二码去重；
- 第二码韵母：24个韵母合并在15键上，分布规律是： 1. aoe开头的韵母（第1类）在第1行， 2. i开头的韵母（第2类）在第2行， 3. u开头的韵母（第3类）在第3行， 4. ü开头的韵母（第4类）在第5列。；
- 第三码去重码&声调：1. 韵母去重：第二码中的三个共键韵母按照韵尾的不同分布在1-3行上，以区分重复音节；2. 声调：用1-5列分别输入1-4声和轻声。

<br>

“三码拼音”方案采用动态键盘，以方便熟悉键位，只能打三码全码；熟悉之后可使用“三码拼音快打”方案，采用静态键盘，可使用首码简 拼和前两码简拼，打前两码简拼类似于普通有重音的双拼，第三码相当于直接辅助码。

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
