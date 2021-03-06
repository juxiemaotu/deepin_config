[TOC]

## 声明
这里仅仅发布西风瘦码个人版的使用版，且不做商业用途。
学习西风瘦码请联系西风的发明人之一——化外愚民。
可在贴吧或西风的论坛上找到他，可获得西风编码原理，学习帮助等。以便快速学习。

当然，个人认为，西风瘦码其实不用学，跟着反查码打就行。追求字由心生的境界！

## 使用方法
* 直接使用（发布版）
    * 将发布版里的文件复制到Rime的用户文件夹中，重新部署即可
    * 最基本运行文件，放进去即可部署使用
      * default.custom.yaml
      * xifeng_danzi_simp.schema.yaml
      * xifeng_danzi_simp_fancha.table.bin
      * xifeng_danzi_simp.table.bin
      * xifeng_danzi_simp.reverse.bin
* 定制使用（参考编辑版）
    将参考编辑版里的文件复制到Rime用户文件夹中。
    参考编辑版含有配置文件、码表的源代码，且注释的很清楚，结合Rime官方文档可轻松定制
    第一次部署有两个部分：
    * 西风瘦码反查：需要先编辑好其配置文件和字典
    * 西风瘦码：编辑配置文件和字典
    重新部署，两个部分都要部署，西风瘦码的反查字典是bin文件作用，单独的码表是没有用的
    以后使用就可以用已经生成好的bin文件结合配置和西风字典一起用了。也就是所谓的发布版

## 版本说明
这里对西风瘦码单字版（个人版）进行说明。毕竟选择用瘦码本身就追求极致追求定制。
**瘦码最大的魅力不是码长，不是打字的巅峰速度，而是极致由心。**这一点我现在深有体会。
正如选择Rime一样。
个人习惯的不同，会带来不同的版本。

### 版本1.0

#### 版本信息 1.0
* 输入法名称：西风单字_Rime
* 版本背景：小小版对Deepin支持较差，想用只能自定义Rime
* 版本号：zh_1.0
* 框架：Rime
* 作者：homy8023
* 原作者：西风瘦码-化外愚民

#### 个人习惯整理
* 标点改动：
  * 因编码影响非四码字连惯输入，故改动标点映射。
    ；→  *  （md常用）
    /  →  $  （md公式）
    {  →  、
    }  →  ；
    [  →  { } 结合自动补全，很好用
    ]  →  [ ] 结合自动补全，很好用
  * 使用自带标点
    o引导+f
  * 使用自带命令
    o引导+m
  * 使用自带缩写
    o引导+s
  * 更多可自定义
* 数字键使用
    数字键不选重，直接顶功上屏
* 编码改动
  *五码优化为四码
    全部单字四码以内，在大体遵循编码规则的前提下，将五码字优化到四码中。毕竟23583个编码空间，才只用到5710个。
  *其他编码为化外愚民2017年5月放出的小小版编码，未作改动。（也不需要改，同15年版基本相同）

#### 版本改动
* 建立第一版
* 因‘\\键’尚未能完成调制，使用“`”作为反查引导。
* Shift + A-Z，不能直接上屏，要打空格。
    * 一个是因为刚接触Rime对其使用掌握不够，Shift控制上屏技术没解决
    * 另一个是，Rime的理念中Shift键就不大写上屏，方便中英混输。发现对于单字来说，真的挺不错。就适用一下先。

### 版本2.0

#### 版本信息 2.0
* 输入法名称：西风单字_Rime
* 版本背景：入坑Rime，努力完善中
* 版本号：zh_2.0
* 框架：Rime
* 作者：homy8023
* 原作者：西风瘦码-化外愚民

#### 版本改动
**标点-使用symbols标点**
  * 去除码表标点，常用缩写、命令不变。
  * 采用Rime symbols标点，使用\\引导。
  * TAB键左右选择
  * 翻页快捷键 “-”、“=”
  * 标点映射，数字键直接选择
    *  ';': [ '$$', '**', "###", '```' ]            # 替换成常用标点，以TAB切换，方便输入(markdown常用)，建议最多设四个，避免出错也不便捷
    * '[': [ ';', '/', ÷, ／, 「, 【, 〔, ［ ]         # 补“;”，“/”，及本身
    * ']': [ 、, '\', ＼, 」, 】, 〕, ］ ]             # 补“、”，“\”，及本身
**自动上屏**
*对auto_select有了正确理解，
  *它不是个开关,而是有具体规则内容的唯一码上屏的实现语句。
  *因此，去除auto_select_pattern的内容，无用，还不知道对错。
