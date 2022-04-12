# 三码拼音方案

配方： ℞ arsenali/rime-triple-pinyin

[Rime](https://rime.im/) 大致按“声、韵、调”的顺序三码输入一个带调音节，15键内无重音

## 安装

[东风破](https://github.com/rime/plum) 安装口令： <code> bash rime-install arsenali/rime-triple-pinyin </code>

本方案词库依赖于 [地球拼音](https://github.com/rime/rime-terra-pinyin) ℞ rime-terra-pinyin，安装本方案前请先安装 ℞ rime-terra-pinyin。

皮肤（主题）文件依赖于 [同文安卓輸入法平臺](https://github.com/osfans/trime) ℞ trime，安卓平台使用本方案前请先安装 ℞ trime。


## 简介

三码拼音是为方便在触屏手机上快速、准确地打字而设计的，方案设计原则包括：
1. 键数要少（只使用15个按键），方便单手打字；
2. 避免像九宫键一样的重复音节，以实现准确输入；
3. 为准确输入，编码包括声调（也可使用无声调模式）；
4. 易学易用。


### 键位图

![键位图](https://user-images.githubusercontent.com/27876448/162973794-ff104238-7bb0-477d-aa88-6210fe63aef7.jpg)

_截图使用的是 金墨年华-咖啡主题 小鹤配色_


<br>

### 编码规则

编码方式为“声母+韵母+去重码&声调”，编码规则是：

- **第一码：声母**

||1列|2列|3列|4列|5列
:---:|:---:|:---:|:---:|:---:|:---:
1行|b|p|m|r f|zh z
2行|d|t|n|l|ch c
3行|g j|k q|h x|零yw|sh s

23个声母合并在15键上，基本按照声母表顺序排列，方便记忆。其中部分声母共键，共键声母将在第二码去重。

- **第二码：韵母**

||1列|2列|3列|4列|5列
:---:|:---:|:---:|:---:|:---:|:---:
1行|a,an,ang|e,en,eng|o,ou,ong|ai,ei,ao|er,üan,\_
2行|ia,ian,iang|ie,in,ing|io,iu,iong|iai,i,iao|üe,ün,\_
3行|ua,uan,uang|\_,un,ueng|uo,\_,\_|uai,ui,u|\_,\_,ü

39个韵母合并在15键上，分布规律是：

1. aoe开头的韵母（除了er）（第1类）在第1行，
2. i开头的韵母（第2类）在第2行，
3. u开头的韵母（第3类）在第3行，
4. ü开头的韵母（以及er）（第4类）在第5列。

通过前两码声韵组合消除共键声母，规则包括：
1. g/j, k/q, h/x：
因为gkh只和1、3类韵母相拼，jqx只和2、4类韵母相拼，所以共键声母被自然区分；
2. “零声母/y/w”：
因为只有第1类韵母存在零声母音节，第2、4类韵母只和y相拼，第3类韵母只和w相拼，所以三个声母被自然区分；（注：声母y,w也是零声母的一种形式，例如 ya='ia, wa='ua, yue='ue。）
3. zh/z, ch/c, sh/s, r/f：
由于这8个声母都不跟第2、4类韵母，即没有zhian,züan等音节，所以把zh,ch,sh,r所跟韵母放在第1、3行，把z,c,s,f所跟韵母放在第2行和第4列。（注：7个整体认读音节(zhi,chi,shi,ri,zi,ci,si)的韵母虽然写作i，但其实和单音节韵母i不同，因此归为第1类韵母，安排在第3键上。）

通过前两码组合，共键声母全部得以区分。

在第二码中，把相似的韵母安排在同一个键位上，每个键位上都有3个韵母，共键韵母将在第三码中进行去重。

- **第三码：去重码&声调**

1. 韵母去重：第二码中的三个共键韵母按照韵尾的不同分布在1-3行上，以消除重复音节；
2. 声调：用1-5列分别输入1-4声和轻声。

以第一组韵母为例，第三码键位是：

||1列|2列|3列|4列|5列
:---:|:---:|:---:|:---:|:---:|:---:
1行|ā|á|ǎ|à|ȧ
2行|ān|án|ǎn|àn|ȧn
3行|āng|áng|ǎng|àng|ȧng

在输入第三码之后便得到了唯一的一个带调拼音音节，不会有重复音节。

如果不想区分声调，可长按或上滑T键切换为无声调模式，此时可用第三码的第5列输入无声调拼音。

<br>

“三码拼音”方案(triple_pinyin_smpy)采用动态键盘，以方便熟悉键位，只能打三码全码；熟悉之后可使用“三码拼音快打”方案(triple_pinyin_smpy_express)，采用静态键盘，可使用首码简拼和前两码简拼，打前两码简拼类似于普通的有重音的双拼，第三码相当于直接辅助码。

按三码拼音的编码规则，可设计出多种三拼方案，本项目中除“三码拼音”外，还初步设计了“三码拼音aoe”和“[三码注音](https://github.com/arsenali/rime-triple-pinyin-bopomofo)”两套派生方案，供不同用户选用。用户亦可根据自己的习惯设计出自己的三码拼音韵母布局。

---

主题文件中自带简单教程，可点击“帮助”查看。

点击“反查”可使用拼音或笔画进行编码反查。

默认只载入地球拼音词库，需要用更多其他词库请到网盘或QQ群下载。

下载地址：http://www.lssp.ysepan.com/

或：https://pan.baidu.com/s/1i4X3WFz 密码: 1jpd

QQ群：[150478288](https://jq.qq.com/?_wv=1027&k=5wf1uTQ)


<br>

### &#8627; Stargazers
[![Stargazers repo roster for @arsenali/rime-triple-pinyin](https://reporoster.com/stars/arsenali/rime-triple-pinyin)](https://github.com/arsenali/rime-triple-pinyin/stargazers)

### &#8627; Forkers
[![Forkers repo roster for @arsenali/rime-triple-pinyin](https://reporoster.com/forks/arsenali/rime-triple-pinyin)](https://github.com/arsenali/rime-triple-pinyin/network/members)
