## Dol_欲都孤儿-衣物mod公共仓库

#### 介绍
收集Dol衣物mod的一公共仓库

没有什么限制，只有不进行破坏操作欢迎进行更改

收集的衣物总览：
![输入图片说明](README%E5%9B%BE%E7%89%87%E5%AD%98%E6%94%BE/%E4%BB%8B%E7%BB%8D.png)


##### 仓库文件介绍

美化合集

    存放打包好的美化包
    注：如果进行了添加，在推送时标明改动了那些文件。如果改的过多可忽略

 **衣物-基于BJ** 

基于BJ特写制作的mod

![输入图片说明](%E7%89%B9%E5%86%99mod/BJ%E7%89%B9%E5%86%99/BJ%E9%9F%A9%E7%AB%99%E7%89%B9%E5%86%99.png)

 **衣物-基于PB** 

基于PB特写制作的mod

![输入图片说明](%E7%89%B9%E5%86%99mod/PB%E7%89%B9%E5%86%99/PB%E7%89%B9%E5%86%99.png)

#### mod安装教程

##### 替换

```
将美化文件直接复制到游戏img文件内

注：查看美化文件是否解压(查到最后一跳)

一般美化作者都会在帖子或美化文件里标注好路径，只要确认文件解压好了以后直接将文件夹拖进来就好
```
##### 添加

```
打开"Degrees of Lewdity.html"
	
搜索 setup.moddedClothes.衣服类型[             //把代码复制到"[]"中

{    index: 1,   //衣物序号，如果有添加其他mod，上个mod的index+=1
}, ];

复制图片:  //注意放在对应文件中，我在收集时有些作者未放在正确的文件内

图标：img\misc\icon\clothes

衣服贴图：img\clothes\对应衣服类型

衣服类型：源作者应该有给
	upper上装 lower下装 under_lower内裤  under_upper内衣 head头饰 face面饰 neck颈饰 hands手饰 leg袜子 feet鞋类 genitals贞操带
```

#### 衣服制作

图标：30x30         img\misc\icon\clothes

图片：              img\clothes\衣服类型
    
    静态：256x256 

​    ![输入图片说明](README%E5%9B%BE%E7%89%87%E5%AD%98%E6%94%BE/Static.png)

    动态：512x256     每1秒进行切换

​    ![输入图片说明](README%E5%9B%BE%E7%89%87%E5%AD%98%E6%94%BE/Current.png)

##### 图片文件信息 

图片显示在人物后
```
back.png
```
图片显示在人物前      
```
衣服完好度：完整的 磨损 破烂的 撕裂
    full
    frayed
    tattered 
    torn  
acc     组件
*_gray      颜色
```
##### 图片制作
只制作full.png即可

![输入图片说明](README%E5%9B%BE%E7%89%87%E5%AD%98%E6%94%BE/Picture%20production-2.png)

打开绘图软件(PS)，对着画。如果制作动态，两图层,画完

对齐打开(PS:视图->对齐)制作的衣物置入两份   注:不论用那款软件能合到一块就行

![输入图片说明](README%E5%9B%BE%E7%89%87%E5%AD%98%E6%94%BE/Picture%20production-1.png)


##### 填写代码      
```
{
    index: 56,    //衣服ID，不可重复
    name: "starhairpin",   
    name_cap: "starhairpin",cn_name_cap: "星星发卡",     //星星发卡：显示的名称
    variable: "starhairpin",    
 /*
     starhairpin：衣服存放的文件名
     衣服图片:
         在img\clothes\衣物类型，创建同名文件夹
         星星发卡是头部物品：
             因此需写在setup.moddedClothes.head代码段内
             需在img\clothes\head创建一名为starhairpin的文件
             
         衣物类型：upper上装 lower下装 under_lower内裤  under_upper内衣 head头饰 face面饰 neck颈饰 hands手饰 leg袜子 feet鞋类 genitals贞操带
 */
    iconFile: "star_hairpin.png",    //缩略图：\img\misc\icon\clothes
    integrity: 50,
    integrity_max: 50,         //衣物耐久度以及耐久度上限
    fabric_strength: 20,       //暴露度
    warmth: 0,                 //保暖度
 //三项数值与面板对应关系：0-20一颗星，20-50两颗星，50-100三颗星，100-200四颗星，200-500五颗星，500-900六颗星，900以上7颗星。
    cost: 1500,                             //衣服价格，向前数两位为衣物的真实价格   例: 1500 = 15
    description: "一闪一闪的反光。",          //介绍
    shop: ["clothing"],                    //购买地点。forest森林商店，adult成人店，clothing服装店
    type: ["normal"],                      //词条。给予衣物特殊的属性normal = 便装     查看：http://https://tieba.baidu.com/p/8596267626?see_lz=1#148576648382l
    gender: "n",                           //衣物适用性别。f为女，n为男
    reveal: 1,
    word: "a",
    plural: 0,
    colour: 0,
    colour_options: [],
    colour_sidebar: 0,
    colour_combat: 0,
    femininity: 0,
    accessory: 0,
    accessory_colour: 0,
    accessory_colour_options: [],
    accessory_colour_sidebar: 0,
    back_img: 0,
    cursed: 0,
    location: 0,
    accIcon: 0,
}
```

[衣物添加](#添加)

#### 头发制作或替换

##### 文件信息

**sides 侧发**：img\hair\sides 

**fringe 刘海**：img\hair\fringe  

**png文件**：头发长度   

  Chest：胸部

  Feet：脚

  Navel：肚脐

  Short：短

  Shoulder：肩膀

  Thighs：大腿 

##### 更改原版：

估计为加特写，进sides/fringe拿过来加就行

![Hair production picture2.png](README%E5%9B%BE%E7%89%87%E5%AD%98%E6%94%BE/Hair%20production%20picture2.png)

![Hair production picture1.png](README%E5%9B%BE%E7%89%87%E5%AD%98%E6%94%BE/Hair%20production%20picture1.png)


##### 添加：

**刘海**   搜索：set setup.hairstyles.fringe to 或 头发名称 

[  在"[]"内添加

{   name: &quot;default&quot;,   //文件名

  name_cap:  &quot;顺其自然&quot;,  //显示名

  variable:  &quot;default&quot;,  //文件名

  type: 0,              //不清楚，似乎没什么影响

  shop: [&quot;mirrorhair&quot;],    //地点：镜子

}, ]

 **侧发**   搜索：set setup.hairstyles.sides to 或 头发名称
	参数和刘海一样  

**图片制作：** 制作相应的图片存放在"variable"变量对应的文件中并复制到sides/fringe文件内 

​	如：variable: &quot;default&quot;       需创建一名为default的文件并放到sides/fringe文件内 

如嫌麻烦制作一个，复制粘贴几个重命名为   

​	Chest/Feet/Navel/Short/Shoulder/Thighs 



#### 添加/修改剧情

```
测试使用:
搜索：海报			它的所属结构：switch _furniture.poster.name
使用：去购物中心买一份，注意海报名，买完回卧室
	&lt;&lt;furnitureicon   _poster.iconFile&gt;&gt;墙上挂着一张牛女孩的海报。
		使用在后面直接添加	
		例：[[瞬移到农场|Farmland]]

添加剧情/场景:
注：为方便查看加了几个空格，但<>两边不允许有空格，使用时注意把空格删了
					 事件ID			   		场景名称				  位置&大小(似乎没什么用)
<  tw-passagedata    pid="4740"   name="Orphanage Loft Spray"  tags=""    position="1225,59225"   size="100,100" >
	你正呆在学校食堂。		//对话或介绍
	
	//调用事件：吃午饭
	&lt;&lt;  foodicon  &gt;&gt;		//写在foodicon和lstress之间
		&lt;&lt;  link [[吃午饭 (0:10)|Canteen Lunch]]  &gt;&gt;
		//吃午饭：在游戏链接中看到的内容
		//Canteen Lunch：跳转的场景名称
		
		//内容：此事件对玩家的影响	例：pass 10：游戏进行10分钟		stress：压力-6
		&lt;&lt;pass 10&gt;&gt;      &lt;&lt; stress -6 &gt;&gt;  &lt;&lt; /link &gt;&gt;
	&lt;&lt;  lstress  &gt;&gt;

<  /tw-passagedata  >	
//tw-passagedata标签建议存放位置：
	//搜索→存到此处 <tw-passagedata pid="10658" 


属性/事件查看：
https://gitee.com/onegot/Dol/blob/master/%E5%89%A7%E6%83%85_%E6%B7%BB%E5%8A%A0_%E4%BF%AE%E6%94%B9/%E5%89%A7%E6%83%85-%E5%AF%B9%E8%AF%9D.md


部件：
if判断变量，不清楚大部些变量是干什么的/什么意思，但
例：
	顺从：<<if $submissive gte 1150>>		如果顺从大于等于1150打印：
		“你都紧张了，”你说，当你等待许可继续。
	抗拒:<<elseif $submissive lte 850>>		如果顺从小于等于850打印：
		“你在发抖，“你低声说。“我就当你同意我继续了。”
	中性:<<else>>		                        如果都不是打印：
		“我可以吗？”你小声说

<<generate1>>，<<person1>>，<<endevent>>...：场景/部件，--- 待处理
官方链接：https://gitgud.io/Vrelnir/degrees-of-lewdity/-/wikis/Writing/Writer's-Guide
```


#### HP显示mod

```
示例：
	他们看起来很急切。 HP: 750/750 | 200/200/200/150
	他们看起来被激起了性欲。 他们看起来很平静。 他们看起来有些谨慎。

//标记  搜索:很急切
&lt;&lt;if $loveDrunk&gt;&gt;
    &lt;span class=&quot;lustful&quot;&gt;&lt;&lt;He&gt;&gt;_looks&lt;&lt;print either(&quot;陶醉于爱情&quot;, &quot;罪孽深重&quot;, &quot;疯了&quot;, &quot;欲火焚身&quot;, &quot;极度狂喜&quot;)&gt;&gt;。&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte $enemyhealthmax&gt;&gt;
    &lt;span class=&quot;red&quot;&gt;&lt;&lt;He&gt;&gt;_looks很急切。&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 4&gt;&gt;
    &lt;span class=&quot;pink&quot;&gt;&lt;&lt;He&gt;&gt;_looks有些难受。&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 3&gt;&gt;
    &lt;span class=&quot;purple&quot;&gt;&lt;&lt;He&gt;&gt;_looks有些痛苦。&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 2&gt;&gt;
    &lt;span class=&quot;blue&quot;&gt;&lt;&lt;He&gt;&gt;_looks十分痛苦。&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 1&gt;&gt;
    &lt;span class=&quot;lblue&quot;&gt;&lt;&lt;He&gt;&gt;_looks受到了不少伤害。&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gt 0&gt;&gt;
    &lt;span class=&quot;teal&quot;&gt;&lt;&lt;He&gt;&gt;看起来无法承受更多的痛苦。&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth lte 0&gt;&gt;
    &lt;span class=&quot;green&quot;&gt;&lt;&lt;He&gt;&gt;吃痛退开。&lt;/span&gt;
    &lt;&lt;combatcontrol 15&gt;&gt;&lt;&lt;def 10&gt;&gt;
   &lt;&lt;/if&gt;&gt;

   &lt;&lt;if $enemyhealth gte $enemyhealthmax&gt;&gt;
    &lt;span class=&quot;red&quot;&gt;HP: &lt;&lt;= Math.round($enemyhealth) &gt;&gt;/$enemyhealthmax&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 4&gt;&gt;
    &lt;span class=&quot;pink&quot;&gt;HP: &lt;&lt;= Math.round($enemyhealth) &gt;&gt;/$enemyhealthmax&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 3&gt;&gt;
    &lt;span class=&quot;purple&quot;&gt;HP: &lt;&lt;= Math.round($enemyhealth) &gt;&gt;/$enemyhealthmax&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 2&gt;&gt;
    &lt;span class=&quot;blue&quot;&gt;HP: &lt;&lt;= Math.round($enemyhealth) &gt;&gt;/$enemyhealthmax&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gte ($enemyhealthmax / 5) * 1&gt;&gt;
    &lt;span class=&quot;lblue&quot;&gt;HP: &lt;&lt;= Math.round($enemyhealth) &gt;&gt;/$enemyhealthmax&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth gt 0&gt;&gt;
    &lt;span class=&quot;teal&quot;&gt;HP: &lt;&lt;= Math.round($enemyhealth) &gt;&gt;/$enemyhealthmax&lt;/span&gt;
   &lt;&lt;elseif $enemyhealth lte 0&gt;&gt;
    &lt;span class=&quot;green&quot;&gt;HP: &lt;&lt;= Math.round($enemyhealth) &gt;&gt;/$enemyhealthmax&lt;/span&gt;
   &lt;&lt;/if&gt;&gt;
   &lt;&lt;if $enemynomax isnot 1 &gt;&gt;
    |&lt;span class=&quot;yellow&quot;&gt;
    &lt;&lt;if $enemynomax is 2 &gt;&gt;
     &lt;&lt;= Math.round($NPCList[0].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[1].health) &gt;&gt;
    &lt;&lt;elseif $enemynomax is 3 &gt;&gt;
     &lt;&lt;= Math.round($NPCList[0].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[1].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[2].health) &gt;&gt;
    &lt;&lt;elseif $enemynomax is 4 &gt;&gt;
     &lt;&lt;= Math.round($NPCList[0].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[1].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[2].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[3].health) &gt;&gt;
    &lt;&lt;elseif $enemynomax is 5 &gt;&gt;
     &lt;&lt;= Math.round($NPCList[0].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[1].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[2].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[3].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[4].health) &gt;&gt;
    &lt;&lt;elseif $enemynomax is 6 &gt;&gt;
     &lt;&lt;= Math.round($NPCList[0].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[1].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[2].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[3].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[4].health) &gt;&gt;/&lt;&lt;= Math.round($NPCList[5].health) &gt;&gt;
    &lt;&lt;/if&gt;&gt;
    &lt;/span&gt; 
   &lt;&lt;/if&gt;&gt;
   &lt;br/&gt;

//标记 粘贴至"射精迫在眉睫"上方
   &lt;&lt;if $enemyarousal gte $enemyarousalmax&gt;&gt;
    &lt;&lt;if $NPCList[0].penis isnot &quot;none&quot; and !npcHasStrapon(0)&gt;&gt;
     &lt;span class=&quot;red&quot;&gt;射精迫在眉睫。&lt;/span&gt;
```

#### 上传文件/推送

##### 本仓库

[美化mod提交页](https://gitee.com/onegot/Dol/issues/I8AB1T)



##### win SSH
Git下载:[Git官网](https://git-scm.com/downloads)

```
 **下载/使用私钥**       在发行版内可见
执行：ssh-add  id_rsa    //id_rsa私钥文件名，操作添加缓存/访问私钥的路径
注：对id_rsa这个文件的权限不能过高
    文件属性->安全->高级->只保留对id_rsa读的权限，其余用户访问权限全删

 **克隆**    将仓库内所有文件下载到本地
git clone git@gitee.com:onegot/Dol.git

 **推送**    将本地文件上传到仓库
git push origin   master    //origin：变量/别名存放仓库的地址    master：分支名称
//              可以是任意名称          仓库的SSH地址
git remote add    origin       git@gitee.com:onegot/test.git        //给origin赋值


查看已经添加的秘钥：ssh-add -l

 **在win下ssh-agent服务通常未启动**     //ssh-agent：连接SSH地址的一服务
执行：ssh-add id_rsa
    会报错：Error connecting to agent: No such file or directory
启动：   右键开始菜单选择：windows PowerShel(管理员)
    Set-Service -Name ssh-agent -StartupType Manual
    Start-Service ssh-agent

```

#### 外部链接

```
Vrelnir 的博客
    https://vrelnir.blogspot.com/

英文游戏维基
    https://degreesoflewdity.miraheze.org/wiki/Main_Page

中文游戏维基
     https://degreesoflewditycn.miraheze.org/wiki/%E9%A6%96%E9%A1%B5

官方 Discord
    https://discord.gg/VznUtEh

游戏源码仓库
    https://gitgud.io/Vrelnir/degrees-of-lewdity/-/tree/master/

汉化发布仓库
     https://github.com/Eltirosto/Degrees-of-Lewdity-Chinese-Localization
```