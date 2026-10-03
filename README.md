[index.html](https://github.com/user-attachments/files/33004396/index.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的学习主页</title>
    <style>
        /* 简单CSS美化，让页面不那么简陋，看不懂没关系，先复制用 */
        body {
            max-width: 800px;
            margin: 30px auto;
            font-size: 18px;
            font-family: "微软雅黑",sans-serif;
            padding: 0 20px;
        }
        a {
            display: block;
            margin:10px 0;
        }
    </style>
</head>
<body>
    <h1>我的个人学习站</h1>
    <p>这里存放我的前端、Python学习笔记</p>
    <hr>
    <h2>笔记导航</h2>
    <ul>
        <li><a href="html-notes.html">HTML笔记</a></li>
        <li><a href="python-notes.html">Python基础语法笔记</a></li>
        <li><a href="cet6-notes.html">英语六级备考笔记</a></li>

    </ul>
</body>
</html>
[html-notes.html](https://github.com/user-attachments/files/33004405/html-notes.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML学习笔记</title>
    <style>
        body {
            max-width: 850px;
            margin: 32px auto;
            font-size: 17px;
            font-family: "Microsoft Yahei", sans-serif;
            padding: 0 20px;
            line-height: 1.6;
        }
        pre {
            background-color: #f4f4f4;
            padding: 14px;
            border-radius: 6px;
            overflow-x: auto;
        }
        .back {
            font-size: 16px;
        }
        h2 {
            border-left: 4px solid #4285f4;
            padding-left: 10px;
            margin-top: 35px;
        }
    </style>
</head>
<body>
    <a href="index.html" class="back">← 返回学习首页</a>
    <h1>HTML 学习笔记</h1>
    <hr>

    <h2>1. HTML基础介绍</h2>
    <p>HTML：超文本标记语言，用来搭建网页结构。</p>
    <p>标签大部分成对：&lt;标签名&gt; 开始，&lt;/标签名&gt;结束；少数是单标签。</p>

    <h2>2. HTML5标准骨架（必须背诵）</h2>
<pre>
&lt;!DOCTYPE html&gt;
&lt;html lang="zh-CN"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;
    &lt;title>网页标题&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
    页面可见内容写在这里
&lt;/body&gt;
&lt;/html&gt;
</pre>

    <h2>3. 常用文本标签</h2>
    <ul>
        <li>&lt;h1&gt; ~ &lt;h6&gt; 标题，h1最大，一个页面只能1个h1</li>
        <li>&lt;p&gt; 段落标签，自带上下间距</li>
        <li>&lt;br&gt; 换行（单标签）</li>
        <li>&lt;hr&gt; 水平分割线（单标签）</li>
        <li>&lt;b&gt;&lt;/b&gt; / &lt;strong&gt;&lt;/strong&gt; 文字加粗</li>
        <li>&lt;i&gt;&lt;/i&gt; / &lt;em&gt;&lt;/em&gt; 文字斜体</li>
        <li>&lt;div&gt; 块级容器，划分大块区域</li>
        <li>&lt;span&gt; 行内小容器，包裹小段文字</li>
    </ul>

    <h2>4. 链接与图片</h2>
    <p>超链接 a 标签：</p>
<pre>
&lt;a href="目标地址" target="_blank"&gt;链接文字&lt;/a&gt;
</pre>
    <ul>
        <li>href：跳转地址，可以是网址或者本地html文件</li>
        <li>target="_blank"：在新标签页打开页面</li>
    </ul>

    <p>图片 img 单标签：</p>
<pre>
&lt;img src="图片路径" alt="图片描述文字"&gt;
</pre>
    <ul>
        <li>src：图片的文件路径</li>
        <li>alt：图片加载失败时显示的替代文字</li>
    </ul>

    <h2>5. 列表</h2>
    <p>无序列表（圆点 ul + li）</p>
<pre>
&lt;ul&gt;
    &lt;li&gt;项目1&lt;/li&gt;
    &lt;li&gt;项目2&lt;/li&gt;
&lt;/ul&gt;
</pre>
    <p>有序列表（数字 ol + li）</p>
<pre>
&lt;ol&gt;
    &lt;li&gt;第一步&lt;/li&gt;
    &lt;li&gt;第二步&lt;/li&gt;
&lt;/ol&gt;
</pre>

    <h2>6. 块级元素 vs 行内元素</h2>
    <p><strong>块级元素：独占一行</strong>：div、h1~h6、p、ul、ol、section</p>
    <p><strong>行内元素：同一行并排，宽高由内容决定</strong>：span、a、b、em、img</p>

    <h2>7. 标签属性</h2>
    <p>属性写在<strong>开始标签内部</strong>，格式：属性名="值"</p>
    <ul>
        <li>class：类名，多个元素可以共用，用于CSS</li>
        <li>id：唯一标识，一个页面id只能出现一次</li>
    </ul>

    <h2>8. 阅读HTML代码的步骤</h2>
    <ol>
        <li>区分 head（页面配置，看不见）和 body（页面可见内容）</li>
        <li>从外到内看标签嵌套关系，标签不能交叉</li>
        <li>识别标签作用</li>
        <li>读取标签上的属性</li>
    </ol>

    <h2>9. 浏览器查看网页源码</h2>
    <ul>
        <li>Ctrl+U：查看页面原始源代码</li>
        <li>F12 / Ctrl+Shift+I：开发者工具，Elements面板看渲染后的HTML</li>
        <li>箭头工具：点击页面元素，自动定位对应HTML代码</li>
    </ul>

</body>
</html>
[python-notes.html](https://github.com/user-attachments/files/33004408/python-notes.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Python基础笔记</title>
    <style>
        body {
            max-width: 850px;
            margin: 32px auto;
            font-size: 17px;
            font-family: "Microsoft Yahei", sans-serif;
            padding: 0 20px;
            line-height: 1.6;
        }
        pre {
            background-color: #f4f4f4;
            padding: 14px;
            border-radius: 6px;
            overflow-x: auto;
        }
        .back {
            font-size: 16px;
        }
        h2 {
            border-left: 4px solid #4285f4;
            padding-left: 10px;
            margin-top: 35px;
        }
    </style>
</head>
<body>
    <a href="index.html" class="back">← 返回学习首页</a>
    <h1>Python基础语法笔记（考试版）</h1>
    <hr>

    <h2>1. 注释</h2>
    <p>注释不会被程序执行，用来写说明文字</p>
<pre>
# 单行注释  #后面所有文字都是注释
"""
三引号：多行注释
可以写很多行
"""
</pre>

    <h2>2. 输出 print() 与输入 input()</h2>
<pre>
print("hello")  # 输出内容到控制台
print(10, 20, 30) # 多个内容，默认空格隔开

# input() 获取用户输入，**返回永远是字符串str类型**
name = input("请输入名字：")
age = input("请输入年龄：")
# 需要数字必须类型转换
age = int(input("请输入年龄："))
</pre>

    <h2>3. 变量与命名规则（考点）</h2>
    <ul>
        <li>变量：存储数据的容器，用=赋值</li>
        <li>命名：字母、数字、下划线；<strong>不能数字开头</strong></li>
        <li>区分大小写；不能使用Python关键字：if,for,while,def,else等</li>
        <li>推荐命名：下划线命名 student_name</li>
    </ul>
<pre>
a = 10
b = 3.14
name = "小明"
is_ok = True
</pre>

    <h2>4. 基础数据类型（必考）</h2>
    <ul>
        <li>int 整数：10, -5</li>
        <li>float 浮点数（小数）：3.14</li>
        <li>str 字符串："文字" 或 '文字'</li>
        <li>bool 布尔：只有 True / False（首字母大写）</li>
        <li>list 列表 [] 、tuple元组()、dict字典{}、set集合{}</li>
    </ul>
    <p>类型转换函数</p>
<pre>
int("123")    # 字符串转整数
str(666)      # 转字符串
float("2.2")  # 转小数
type(变量)    # 查看变量类型
</pre>

    <h2>5. 运算符（计算题必考）</h2>
    <h3>算术运算符</h3>
<pre>
+ 加
- 减
* 乘
/ 除法 → 结果一定是浮点数
// 整除，取商的整数部分（向下取整）
% 取余数（求模），判断奇偶常用
** 幂运算  2**3 = 8
</pre>
    <h3>赋值运算符</h3>
<pre>
a = 10
a += 2   # a = a+2
a -= 1
a *= 3
a //= 2
a %= 5
</pre>
    <h3>比较运算符（结果是True/False）</h3>
<pre>
> 大于  < 小于
>= 大于等于  <=小于等于
== 判断相等
!= 不等于
</pre>
    <h3>逻辑运算符</h3>
<pre>
and 并且：两边都True才True
or 或者：一边True就True
not 取反：True变False，False变True
优先级：not > and > or
</pre>

    <h2>6. 字符串与三种格式化占位（高频考点）</h2>
<pre>
# 方法1：% 旧式占位符
info = "姓名：%s，年龄：%d，成绩%.1f" % ("小红",18,95.5)

# 方法2：format
info = "姓名：{}，年龄：{}".format("小红",18)

# 方法3：f-string（推荐，Python3.6+）
name = "小红"
age = 18
info = f"姓名{name}，年龄{age}"
</pre>
    <p>字符串常用方法</p>
<pre>
s = " Hello Python "
s.strip()   # 去除首尾空格
s.upper()   # 全部大写
s.lower()   # 全部小写
s.replace("H","A") #替换
s.split(",") #分割成列表
len(s) #获取字符串长度
s[0] #下标取值，从0开始
s[起始:结束:步长] #切片
s[::-1] #字符串反转
</pre>

    <h2>7. 列表 list []（考试大题常客）</h2>
<pre>
lst = [10,20,30,"abc"]
lst.append(40)      #末尾追加元素
lst.insert(1,99)    #在下标1位置插入99
lst.pop(2)          #按下标删除元素，返回被删掉的值
lst.remove(20)      #删除第一个匹配的元素
lst.clear()         #清空列表
len(lst)            #获取列表长度
lst[0] = 66         #修改下标对应的元素
</pre>
    <p>成员判断：<code>in / not in</code></p>
<pre>
lst = [1,2,3]
print(2 in lst) # True
print(5 not in lst) # True
</pre>

    <h2>8. 元组 tuple ()</h2>
    <p>元组元素<strong>不能修改、增加、删除</strong>，只能读取</p>
<pre>
t = (1,2,3)
print(t[0])
# 只有一个元素时，必须加逗号 t=(10,)
</pre>

    <h2>9. 字典 dict {键:值}</h2>
    <p>键key：不可变类型（字符串、数字）；值value可以任意类型</p>
<pre>
d = {"name":"小明","age":16}
print(d["name"])        # 根据键取值
d["age"] = 17           # 修改值
d["sex"] = "男"         # 添加新键值对
del d["sex"]            # 删除键值对

d.get("name")
d.keys()    # 获取所有键
d.values()  # 获取所有值
d.items()   # 获取全部键值对
</pre>

    <h2>10. 集合 set</h2>
    <p>无序、自动去重，常用于去重题目</p>
<pre>
s = {1,2,2,3} # 自动变成 {1,2,3}
s.add(5)
s.remove(1)
</pre>

    <h2>11. 分支 if 判断（必考）</h2>
<pre>
# 单分支
if 条件:
    语句

# 双分支
if 条件:
    满足条件执行
else:
    不满足执行

# 多分支
if 条件1:
    pass
elif 条件2:
    pass
else:
    pass
</pre>
<p>pass是空语句，占位，暂时不写代码，防止语法报错</p>

    <h2>12. 循环 while / for（大题高频）</h2>
    <h3>while循环</h3>
<pre>
i = 1
while i <= 10:
    print(i)
    i += 1
</pre>
    <h3>for循环 + range()</h3>
    <p>range(开始,结束,步长)，<strong>结束数字取不到</strong></p>
<pre>
# range(1,11) 产生 1~10
for i in range(1,11):
    print(i)

# 遍历列表
lst = [11,22,33]
for x in lst:
    print(x)
</pre>
    <h3>循环关键字 break / continue（选择题必考）</h3>
<pre>
break    # 立刻终止整个循环，跳出循环
continue # 跳过本次循环剩下代码，直接进入下一轮
</pre>

    <h2>13. 函数 def（考试重点）</h2>
<pre>
# 定义函数
def 函数名(形参):
    代码
    return 返回值

# 调用
def add(a,b):
    return a + b

res = add(3,5)
print(res)
</pre>
    <ul>
        <li>形参：定义时括号里的变量 a,b</li>
        <li>实参：调用时传入的数据 3,5</li>
        <li>return：终止函数，返回结果；无return默认返回None</li>
        <li>默认参数：def func(x,y=10): y不传入就默认等于10</li>
    </ul>

    <h2>14. 常用内置函数（选择填空）</h2>
<pre>
len()   获取长度
max()   最大值
min()   最小值
sum()   求和
range()生成整数序列
type() 查看数据类型
print()输出
input()输入
</pre>

    <h2>15. 异常捕获 try-except（基础了解）</h2>
<pre>
try:
    # 可能报错的代码
    num = int(input("输入数字："))
except:
    # 发生错误执行这里
    print("输入不是数字！")
</pre>

    <h2>16. 导入模块</h2>
<pre>
import time
time.sleep(2) #暂停2秒

from random import randint
num = randint(1,10) #生成1~10随机整数，包含两端
</pre>

    <h2>📌 考试常见坑总结（考前看一遍）</h2>
    <ul>
        <li>input()得到的永远是字符串，做计算必须int/float转换</li>
        <li>range(1,10) 只取到9，取不到10</li>
        <li>//整除，%取余数，区分 / 和 //</li>
        <li>列表可以修改；元组不能修改</li>
        <li>break跳出循环；continue跳过本次，不会终止循环</li>
        <li>布尔值True、False首字母大写，小写会报错</li>
    </ul>

</body>
</html>
[cet6-notes.html](https://github.com/user-attachments/files/33004412/cet6-notes.html)

<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>英语六级备考笔记</title>
    <style>
        body {
            max-width: 850px;
            margin: 32px auto;
            font-size: 17px;
            font-family: "Microsoft Yahei", sans-serif;
            padding: 0 20px;
            line-height: 1.6;
        }
        pre {
            background-color: #f4f4f4;
            padding: 14px;
            border-radius: 6px;
            overflow-x: auto;
        }
        .back {
            font-size: 16px;
        }
        h2 {
            border-left: 4px solid #4285f4;
            padding-left: 10px;
            margin-top: 35px;
        }
    </style>
</head>
<body>
    <a href="index.html" class="back">← 返回学习首页</a>
    <h1>英语六级备考笔记</h1>
    <hr>

    <h2>一、六级试卷结构与分值（必看，规划做题时间）</h2>
    <ul>
        <li>写作：15%，106.5分，30分钟</li>
        <li>听力理解：35%，248.5分，25分钟</li>
        <li>阅读理解：35%，248.5分，40分钟</li>
        <li>翻译：15%，106.5分，30分钟</li>
    </ul>
    <p>总分710，及格线：425分。</p>

    <h2>二、写作</h2>
    <h3>写作题型</h3>
    <p>议论文为主：名言引言类、现象解释类、观点对比类。</p>
    <h3>写作模板框架（三段式）</h3>
<pre>
第一段：引入话题，复述题干，简单表态（2~3句）
第二段：展开论点 + 理由/举例（3~4句）
第三段：总结+提出建议/展望（2句）
</pre>
    <h3>高分替换词（替换简单词汇）</h3>
    <ul>
        <li>important → vital / crucial / significant</li>
        <li>many → a host of / numerous</li>
        <li>think → argue / maintain / hold the view that</li>
        <li>help → facilitate / contribute to</li>
        <li>good → beneficial / favorable</li>
    </ul>

    <h2>三、听力</h2>
    <h3>题型分布</h3>
    <ul>
        <li>长对话：8题</li>
        <li>听力篇章：7题</li>
        <li>讲座/讲话：10题（分值最高，重点）</li>
    </ul>
    <h3>做题策略</h3>
    <ol>
        <li>预读选项：看选项关键词，预判话题</li>
        <li>视听一致原则：听到的内容和选项重合度高，大概率是答案</li>
        <li>信号词重点：but、however、so、therefore、because后面往往是答案</li>
    </ol>

    <h2>四、阅读（分值很高，提分重点）</h2>
    <h3>题型顺序&时间分配</h3>
    <ol>
        <li>仔细阅读（2篇，20%）：优先做，性价比最高</li>
        <li>长篇阅读（段落匹配，10%）：找同义替换，不用读懂全文</li>
        <li>选词填空（10%）：难度大、分值低，放最后做</li>
    </ol>
    <h3>阅读核心技巧</h3>
    <ul>
        <li>仔细阅读：先看题干，回原文定位，找同义替换</li>
        <li>段落匹配：抓专有名词、数字、特殊词，原词/同义匹配即可，不精读</li>
        <li>选词填空：先标注选项词性，再看空格前后判断需要什么词性</li>
    </ul>

    <h2>五、翻译（汉译英，中国文化/社会/经济类）</h2>
    <p>常考主题：历史建筑、传统文化、社会发展、地理、节日。</p>
    <h3>翻译注意要点</h3>
    <ul>
        <li>优先保证语法正确，不要强行写复杂长句</li>
        <li>中文多短句，英文适当合并，多用从句、非谓语</li>
        <li>注意时态：历史事件用过去时；客观描述用一般现在时</li>
        <li>遇到不会的词，用简单同义表达改写，不要空着</li>
    </ul>
<pre>
示例：中国拥有悠久的历史。
China has a long history.
</pre>

    <h2>六、高频语法考点（写作+翻译通用）</h2>
    <ul>
        <li>定语从句：which / who / that</li>
        <li>状语从句：if, when, although, because</li>
        <li>非谓语动词：to do / doing / done</li>
        <li>被动语态：be done（翻译很常用）</li>
    </ul>

    <h2>七、备考计划</h2>
    <ul>
        <li>单词：每天背六级核心词，反复复习；重点记熟阅读选项同义替换词</li>
        <li>真题：只做真题，不做模拟题；精做近10年真题</li>
        <li>听力：每天精听1段，跟读，抓连读</li>
        <li>写作翻译：每周各写1篇，对照范文修改表达</li>
    </ul>

    <h2>八、考场注意事项</h2>
    <ol>
        <li>听力播放完毕立刻收答题卡，听力一定要边听边涂卡，不要最后统一涂</li>
        <li>合理分配阅读时间，选词填空不要浪费过多时间</li>
        <li>写作翻译字迹工整，减少拼写错误</li>
    </ol>

</body>
</html>
