# Hackergame 启动

签到题是hg老传统了：改URL参数。

打开题目页面，~~点击开始录制，大喊Hackergame启动，~~点击提交，可以看到URL中多了一个参数`similarity`，将这个值修改为100，再次访问即可。

事实上，你需要录制一次（当然你可以不喊）再提交，否则你无法获取到Hint："说得不够标准哦，相似度大于 99.9% 才能拿到 flag。"。

# 猫咪小测

作为组内一血，我还是想记录一下这道题。可惜的是丢了总一血，因为第四问太着急了，导致没有仔细看是哪个会议，导致第三次提交才正确，提交上去的时候发现已经有三个人做出来了。

1. 想要借阅世界图书出版公司出版的《A Classical Introduction To Modern Number Theory 2nd ed.》，应当前往中国科学技术大学西区图书馆的哪一层？（30 分）
   这个题去[中国科大图书馆](https://lib.ustc.edu.cn)查询书名（可能需要考虑把版本号去掉），会发现这本书藏在外文书库，此时直接Google"西区外文书库"（可能需要考虑加上中国科大相关关键词），会发现[开放时间](https://lib.ustc.edu.cn/hour/)中有提到西区外文书库在12楼。
2. 今年 arXiv 网站的天体物理版块上有人发表了一篇关于「可观测宇宙中的鸡的密度上限」的论文，请问论文中作者计算出的鸡密度函数的上限为 10 的多少次方每立方秒差距？（30 分）
   直接Google"可观测宇宙中的鸡的密度上限"，可以找到[一篇相关知乎](https://www.zhihu.com/question/20337132/answer/3023506910)，可以直接找到答案为10的23次方。
3. 为了支持 TCP BBR 拥塞控制算法，在编译 Linux 内核时应该配置好哪一条内核选项？（20 分）
   这个题我直接问了GPT4，因为我认为这个问题很适合它（不太能说出来原因）。答案是`CONFIG_TCP_CONG_BBR`。
4. 🥒🥒🥒：「我……从没觉得写类型标注有意思过」。在一篇论文中，作者给出了能够让 Python 的类型检查器 MyPY mypy 陷入死循环的代码，并证明 Python 的类型检查和停机问题一样困难。请问这篇论文发表在今年的哪个学术会议上？（20 分）
   我的思路是先找论文，就可以搜到相关会议的网站。Google搜索"mypy infinite loop paper"，这个时候已经找到论文[Python Type Hints Are Turing Complete - DROPS](https://drops.dagstuhl.de/opus/volltexte/2023/18237/pdf/LIPIcs-ECOOP-2023-44.pdf)了。但由于太着急，我就直接提交了DROPS上去，结果发现不对。后来又加了"halting problem"、"filetype:pdf"的关键词，最后确定就是这篇文章，最后再文章的Abstract部分以及会议logo中得到了会议缩写ECOOP。

# 更深更暗

打开题目看完介绍，两个加粗的Hint："hidden flag"和"deep underground"，那就往下翻就完事了。翻了一会感觉不太对劲，于是打开F12，直接搜"flag"就搜到了。

不过身边也有同学按着空格往下翻最后翻到了的，这样的话flag会一闪而过，他拿了录了屏然后回放看到了flag。

# 旅行照片 3.0

今年的旅行照片一筹莫展，放到了比较靠后的位置去做。

由于这道题目的特殊性，我会先展示自己觉得重要的一些文本内容和用到的图片。

## 题目

离开校园后，你和学长走到了附近的一家拉面馆用餐。那家店里的拉面香气扑鼻，店内的装饰和氛围也充满了日式的风格。 学长（下图左一）与你分享了不少学校的趣事。饭后，你们决定在**附近**散步，享受这难得的闲暇时光。**当你们走到一座博物馆前时， 马路对面的喷泉和它周围的景色引起了你的注意**。下午，白色的帐篷里即将举办一场大型活动，人们忙碌的身影穿梭其中，充满了期待与热情。

在参观完博物馆后，学长陪你走到了上野站。你们都感到有些不舍，但知道每次的分别也是为了下次更好的相聚。 **学长那天晚上将继续他的学术之旅，打算乘船欣赏东京的迷人夜景和闪耀的彩虹大桥（Rainbow Bridge）。** 而你则搭乘了**开往马里奥世界的电车**，在那里度过了一段欢乐的时光。~~这一段是我写Writeup时注意到的，做题时没注意到结果也稀里糊涂做出来了。~~

![Nobel Prize](./images/hg23/travel-photo/nobel-prize.jpeg)

![Ramen Shop](./images/hg23/travel-photo/ramen-shop.jpeg)

![Ueno Park](./images/hg23/travel-photo/ueno-park.jpeg)

1. 你还记得与学长见面这天是哪一天吗？（格式：yyyy-mm-dd）
2. 在学校该展厅展示的所有同种金色奖牌的得主中，出生最晚者获奖时所在的研究所缩写是什么？
3. 帐篷中活动招募志愿者时用于收集报名信息的在线问卷的编号（以字母 S 开头后接数字）是多少？
4. 学长购买自己的博物馆门票时，花费了多少日元？
5. 学长当天晚上需要在哪栋标志性建筑物的附近集合呢？（请用简体中文回答，四个汉字）
6. 进站时，你在 JR 上野站中央检票口外看到「ボタン＆カフリンクス」活动正在销售动物周边商品，该活动张贴的粉色背景海报上是什么动物（记作 A，两个汉字）？ 在出站处附近建筑的屋顶广告牌上，每小时都会顽皮出现的那只 3D 动物是什么品种？（记作 B，三个汉字）？（格式：A-B）

## 题解

1. 注意到在拉面馆的合照中，学长带了STATPHYS28会议的的参会牌，可以猜测当天是会议的其中一天，也就是08-07到08-11中的一天。由于每两问对应一个flag，我们可以确定第二问答案之后进行遍历，最后得到是2023-08-10。
2. 直接Google可以知道是诺贝尔奖（好像是物理学奖？不太清楚每个类型的奖牌是否一样），直接去东京大学（因为STATPHYS28是在东京大学举办的）的Wikipedia查看知名校友，可以找到题目所指的得主是[Takaaki Kajita](https://en.wikipedia.org/wiki/Takaaki_Kajita)，可以看到2015年获得诺贝尔物理学奖，此时他在ICRR担任director。
3. 这一问我是做的最后一题（准确来说是最后获取到打开局面的信息的，我以为我第四问找到答案了实际上并没有），关键在于找到题目中的"帐篷中活动"是什么，我也确实找了很久。从Google Map上很容易可以看到这里是上野公园，官方名称上野恩赐公园。
   + 我先是找到了某个东京都官方的网站，可惜上面不展示历史活动信息（不知道为什么我当时的浏览记录没有保存下来，很可惜不能展示更详细的搜索思路），但是我从那个网站找到了广场的官方名称为喷水广场。
   + 考虑到活动会提前通知，同时又需要招募志愿者，所以我在Google上搜索相关关键词时限制了搜索时间范围，最开始从7月到9月，不断缩小范围，最后我发现搜索到了很多具体的活动，但是都不包含8月10日这一天，于是我决定加上一个关键词"8月"，最后在搜索到[一个网站](https://www.uenopark.info/2023/ume-shu-2023/)，上面说明08月10日到08月13日会举办全国梅酒节。
   + 最后搜索"东京全国梅酒节"，可以搜索到[其官方网站](https://umeshu-matsuri.jp/tokyo_ueno)，其中可以找到[招募志愿者的链接](https://umeshu-matsuri.jp/tokyo_staff/)，打开可以看到问卷的链接为[https://ws.formzu.net/dist/S495584522/](https://ws.formzu.net/dist/S495584522/)，答案显而易见。
   + 有点可惜的地方在于没有很快找到[那个记录上野公园活动信息的网站](https://www.uenopark.info)，浪费了不少时间，这里留个链接来帮助上野的朋友们节省时间（笑
4. 这题我以为我很快定位到了答案结果并没有。在Google Map上可以看到上野公园喷水广场附近有两个博物馆：东京国立博物馆和国立科学博物馆，不确定的话把这两个博物馆的所有门票价格都试一遍即可，最后发现是0元。
   + 我本来以为0元是国立科学博物馆的特殊票价，但[官方Writeup](https://github.com/USTC-Hackergame/hackergame2023-writeups/blob/master/official/%E6%97%85%E8%A1%8C%E7%85%A7%E7%89%87%203.0/README.md)给的理由是东京国立博物馆的Visitor Information中有提到Campus Members中学校的学生可以免费参观常规展览，所以为0元。只能说歪打正着吧。
5. 题目中提到了晚上要乘船（事实上我忘记这条信息了，只考虑了晚上），可以在[STATPHYS28的官网](https://statphys28.org/)找到[议程](https://statphys28.org/programtt.html)，观察到08月10日晚上是Banquet，直接在Events中找到[Banquet](https://statphys28.org/banquet.html)，可以找到Meeting Point在Yasuda Auditorium，Google翻译得到安田讲堂。
   + 我看到有一些选手赛后讨论说他得到的翻译是安田礼堂，我觉得有点可惜吧。组委会方面，我没有想清楚为什么要求中文答案，其实直接提交英文也是OK的；选手方面，如果去Wikipedia看一下，可以看到中文是安田讲堂，但我也不确定是不是官方中文名称就是了😂，其实如果看日语（安田講堂）的话，也可以很明显看到是安田讲堂。
6. 直接在Twitter上搜索活动名，可以看到[相关的推文](https://twitter.com/panda_life/status/1688436626895331328)，可以看到是A答案是熊猫。对于B，我直接Google"上野駅 3d動物"，查看图片，发现[一篇文章](https://wow-japan.com/news-flash-shibuya-3d-akida-dog-ads/)，可以看到涩谷站出口广告牌会有3D秋田犬。
   + 事实上我还搜索到了新宿的3D的猫，忘了品种了，好像也是三个字，都试一遍就好了。
   + 按照官方Writeup，应该是可以推出来出口站是涩谷站的（实际上我是按照上野站做的，乐），但可惜不是立本人。

# 赛博井字棋

我最开始的思路是去搜索井字棋先手必胜策略，结果发现好像有后手必平策略。于是就在无聊地点了半天，最后脑洞大开尝试覆盖O（我是X，AI是O），发现不可以点。我就去开发者工具看了看，发现是向后端发送POST请求来表示我所选X的位置，最后利用BurpSuite在第三个X的请求中进行覆盖即可。

# 奶奶的睡前flag故事

我的奶奶为什么不告诉我谷歌亲儿子是Pixel！我一直是当作Nexus去搜索，最后什么也没搜到，甚至还自己修了半天的PNG。

这个题顺着"谷歌"、"Pixel"、"截图"（写Writeup的时候才发现官方给了截图的Hint，我还是自己猜的，可惜了）等关键字就可以搜到Google Pixel今年三月份被爆出来的漏洞Acropalypse，最后找到[相关的利用工具](https://acropalypse.app/)，因为题目所给图片的宽像素为1080，所以猜测Pixel 7（或者自己Custom也行），可以恢复出来下半部分截图，拿到flag。

# 组委会模拟器

简单看一下，第一反应是写一个js跑一下应该就行了，可惜我不怎么会写js。于是F12看了Network，找到了一些后端接口，写了Python代码：

```Python
import requests
import json
import re
import time
import datetime

session = requests.session()

url = "https://hack.lug.ustc.edu.cn/challenge/23/"
cookies = {"cookies-key": "cookies-value"}
headers = {"headers-key": "headers-value"}
resp = session.get(url, headers=headers, cookies=cookies)
resp = session.get("http://202.38.93.111:10021/api/checkToken?token=your_token", headers=headers, cookies=cookies)
resp = session.post("http://202.38.93.111:10021/api/getMessages")
start_time = datetime.datetime.timestamp(datetime.datetime.now())
msgs = json.loads(resp.text)["messages"]

timestamp = 0
flag_pattern = r'hack\[[a-z]+\]'
for idx, msg in enumerate(msgs):
    if re.search(flag_pattern, msg["text"]) is not None:
        flag_idx.append(idx)
        sleep = float(msg["delay"]) - timestamp
        time.sleep(sleep if sleep > 0 else 0)
        timestamp = datetime.datetime.timestamp(datetime.datetime.now()) - start_time
        resp = session.post("http://202.38.93.111:10021/api/deleteMessage", json={"id": idx})

time.sleep(10)
resp = session.post("http://202.38.93.111:10021/api/getflag")
print(resp.text)
```

跑一下就行。写Python就只需要注意sleep的时间就行了，sleep短了会报错"检测到时空穿梭"，sleep久了会撤回失败（题目要求3s内撤回）。

# 虫

这道题我过了很久才做出来（毕竟CTF新手），因为题目Hint是"通过无线信道传输图片的方式"，我没有直接Google到什么东西，所以一直在考虑利用FFT之类的变换将正弦波转换成方波或其他东西来表示0和1，从而恢复图片。之后看到做出来的人越来越多，我决定再看看，这次注意到题目中有提到"接受来自国际空间站（ISS）的图片"，于是通过"ISS"这个关键词检索到了SSTV。

知道是SSTV之后，就可以发现CTF中还是有不少Misc题目跟SSTV有关，也推荐了一些相关软件，可惜我是Mac，很多软件用不了，找到的也是付费的，最后在GitHub上找到一个[小项目](https://github.com/colaclanth/sstv)，直接运行Decode就可以得到包含flag的图片。

# JSON ⊂ YAML?

## JSON ⊄ YAML 1.1

我是随便试出来的，当时的思路是去看YAML1.2中有提到哪些与YAML1.1不一致的地方，然后去尝试，但好像没有找到太多有用的，最后即将放弃的时候好像在哪里看到了一眼科学计数法，于是试了`1e2`作为值，结果成了。

## JSON ⊄ YAML 1.2
我是在对应的库函数中打断点一点点看的，最后看到了个`DuplicateKeyError`，就解出来了，具体过程就不写了，有点折磨说实话。

这一题可以去看[官方Writeup](https://github.com/USTC-Hackergame/hackergame2023-writeups/blob/master/official/JSON%20%E2%8A%82%20YAML/README.md)，看文档还是个好习惯，可惜我没能捕捉到有效信息。

# Git? Git!

恰好前段时间了解了`git reflog`命令，读完题就猜到用这命令解题，毕竟题目中提到了**本地仓库**。

# HTTP集邮册

这题我就是对着MDN的文档一个一个看，看有没有可能触发，最后一个413我找了很久，所以还看了一些RFC的文档，不过也没有什么太多直接的帮助。

我收集到的状态码有：[100, 200, 206, 304, 400, 404, 405, 412, 413, 414, 416, 505]。

+ 100 Continue - `Expect: 100-continue`
+ 200 OK - 点击就送。
+ 206 Partial Content - `Range: bytes=1-1`
+ 304 Not Modified - `If-Modified-Since: Tue, 15 Aug 2023 17:03:04 GMT`
+ 400 Bad Request - 不正确的HTTP请求格式都可以触发。
+ 404 Not Found - 随便一个不存在的文件即可。
+ 405 Method Not Allowed - 随便一个不支持的请求方法（该题中除了`GET`和`HEAD`都不支持）即可。
+ 412 Precondition Failed - `If-Match: "64dbafc8-266"`（原ETag为"64dbafc8-267"）。
+ 413 Content Too Large - `Content-length: 1111111`。这个是我第12个状态码，找了好久，最开始觉得如果我给一个很大的Content，那应该会先被前置的Nginx（即接收我报文的Nginx）返回413，不会请求到题目中的Nginx，最后是在随便试的时候不记得怎么就试了一下，结果出来了。
+ 414 URI Too Long - 一个很长的URI即可触发。我是使用`printf 'a%.0s' {1..10000}`生成的Payload。
+ 416 Range Not Satisfiable - 超出范围的`Range`头即可触发，比如`Range: bytes=615-615`（`index.html`长度为615个bytes）。
+ 505 HTTP Version Not Supported - 修改为一个不支持的HTTP版本即可。

中间无状态我是随便试出来的，在`/`后面加了一个`\r\n`结果触发了，我的flag是`flag{congratu1ations you discovered someth1ng before http1.0}`，后来经过搜索才知道[HTTP/0.9](https://www.w3.org/Protocols/HTTP/AsImplemented.html)，其中也提到了Request格式要求：The client sends a document request consisting of a line of ASCII characters terminated by a CR LF (carriage return, line feed) pair. A well-behaved server will not require the carriage return character.

搜索HTTP/0.9相关信息时还发现了[一个StackOverflow的问题](https://stackoverflow.com/questions/6686261/what-at-the-bare-minimum-is-required-for-an-http-request)还蛮不错，尽管link-only不太好，但我就先不放那么多了。

# Docker for Everyone

我也没想到我会直接就做预期解，可能是因为之前被docker的root用户坑过不少次，所以猜到了可能利用docker这一"特性"。

上来直接看了`/flag`，找到symlink path，发现无权限之后，直接`docker run -it --rm -v /dev/shm:/mnt alpine`映射目录，然后读取flag。

正如flag所说，`Use rootless container please`。具体相关知识可以参考[官方Writeup](https://github.com/USTC-Hackergame/hackergame2023-writeups/blob/master/official/Docker%20for%20Everyone/README.md)。

# 惜字如金 2.0

不太记得去年的惜字如金了，印象里也没很麻烦。

前两个`check_equals`很好改:
```Python
check_equals('creat', 'cre' + 'at')
check_equals('referrer', 'refer' + 'rer')
```

接着往后看：
```Python
cod_dict += ['nymeh1niwemflcir}echaet']
cod_dict += ['a3g7}kidgojernoetlsup?h']
cod_dict += ['ulw!f5soadrhwnrsnstnoeq']
cod_dict += ['ct{l-findiehaai{oveatas']
cod_dict += ['ty9kxborszstguyd?!blm-p']
check_equals(set(len(s) for s in cod_dict), {24})
```

发现每个长度都为23，与要求24不符，于是在每个字符串最后加上`e`，这样可以保证不违反惜字如金的标准。通过修改源代码让其在`check_equals`之前打印flag，可以得到`5laulyoufeepr3cvees3df7weparsn3sfr1gwn!}`。

我们会发现前五个字符并不符合`flag{`的要求，通过查看`decrypt_data`的参数及函数实现（函数实现上没有做任何的复杂变换，只是去了对应index的字符），可以将一些我添加的`e`删除，选择相应的辅音字母（即`f`、`l`、`a`、`g`四个字母）进行重复即可。

最后得到：
```Python
cod_dict += ['nymeh1niwemflcir}echaete']
cod_dict += ['a3g7}kidgojernoetlsup?he']
cod_dict += ['ulw!ff5soadrhwnrsnstnoeq']
cod_dict += ['ctt{l-findiehaai{oveatas']
cod_dict += ['ty9kxborszstgguyd?!blm-p']
```

运行文件即可得到flag。

# 🪐 高频率星球

题目提供了`asciinema`录制的文件，可以直接使用`asciinema cat asciinema_restore.rec > flag.js`导出所有的终端信息，最后将前后无用信息删除，利用编辑器replace的功能将控制字符删除即可得到原js文件。

# 🪐 小型大语言模型星球

## You Are Smart

考虑到这是只是一个类似于续写故事的模型，所以我的Prompt为`The father think his daughter is smart.`。

后来发现直接问`Am I smart?`和`Repeat "you are smart"`更加方便与快捷（注意标点）。

## Accepted

考虑到题目限制7个字符，又是一个无厘头的英文单词，所以我就考虑他的原型`accept`加一个字符是7个字符，当然不加字符也会试一下。最后试出来`accept*`可以。

# 🪐 流式星球

思路也很简单，就是根据`create_video.py`的逻辑，逆向恢复即可。

```Python
import cv2
import numpy as np

def restore_video(input, output, frame_count, frame_width, frame_height):
    # 1. 读取输出文件
    buffer = np.fromfile(input, dtype=np.uint8)
    print(len(buffer))
    if frame_count * frame_width * frame_height * 3 < len(buffer):
        frame_count = len(buffer) // (frame_width * frame_height * 3) + 1
    # 1.1 用0补齐被删除的部分
    buffer = np.pad(buffer, (0, frame_count * frame_width * frame_height * 3 - len(buffer)), 'constant')

    # 2. 恢复原始形状
    buffer = buffer.reshape((frame_count, frame_height, frame_width, 3))

    # 3. 创建新的视频文件
    fourcc = cv2.VideoWriter_fourcc(*'XVID')
    out = cv2.VideoWriter(output, fourcc, 20.0, (frame_width, frame_height))

    # 将 buffer[0] 保存为图片，方便量宽和高之类的
    # cv2.imwrite('frame0.jpg', buffer[0])

    # 4. 写入帧
    for i in range(frame_count):
        out.write(buffer[i])

    out.release()

# 原始视频的属性
frame_count = 10   # 原始视频的帧数
frame_width = 427  # 原始视频的帧宽度，正确值
frame_height = 759  # 原始视频的帧高度，正确值

# 调用函数
restore_video('video.bin', 'restored_video.avi', frame_count, frame_width, frame_height)
```

# 🪐 低带宽星球

## 小试牛刀

网上随便找一个PNG压缩网站即可。

# Komm, süsser Flagge

## 我的 POST

研究了很久，最后用socket解决了。

```Python
import socket

host = '202.38.93.111'
port = 18080

# 创建一个socket连接到服务器
s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
s.connect((host, port))

# 构造一个分块传输编码的HTTP请求，故意将"POST"分割为两部分
# "PO"和"ST"分别作为两个不同的块发送
request = [
    'PO',  # 首个块内容
    'ST / HTTP/1.1\r\n',  # 拼接到第一个块内容，形成"POST"
    f'Host: {host}\r\n',
    'Transfer-Encoding: chunked\r\n',
    '\r\n',
    '64\r\n',  # 第二个块的长度，十六进制的"64"
    'your_token=\r\n',  # 第二个块的内容
    '0\r\n',  # 结束块的长度
    '\r\n'  # 结束块
]

for r in request:
    s.send(r.encode())

# 接收响应
response = s.recv(4096)

# 关闭socket连接
s.close()

# 打印响应数据
print(response.decode())
print(len(response))
```

## 我的 P

这题第二问我非预期解了，也就是[官方Writeup](https://github.com/USTC-Hackergame/hackergame2023-writeups/blob/master/official/Komm,%20s%C3%BCsser%20Flagge/README.md)里提到的非预期解，即，第一问的解法也可以直接解这一问。~~虽然只是干饭前是在没思路了随便试了一下😂~~

# 异星歧途

说实话，感觉这题对不玩Mindustry的人（比如我）很不友好。进去看了半天，甚至因为一些奇怪的原因我都点不了开关。最后决定从第四组开始做（后来朋友说可以去找视频看一下Mindustry逻辑入门会好一些）。

第四组开关应该是（至少我觉得）最有逻辑的一部分，四个开关对应四个发电装置，点一点可以发现门逻辑，最后将电输送过去即可。

第三组开关，每个都点一遍也没看到有什么即时的变化，看了好久才发现发电装置需要某种材料和冷却液，而制造冷却液的机器没有水，总之就是一些连锁反应，然后尝试不同按钮找到相应控制的相应部分的按钮，调整合适即可（这一部分其实没有搞懂，因为开关的作用其实并不是很清楚）。

前两组我都是遍历的，值得一提的是我好像注意到第二组的最后一个开关会导致第三组开关那一部分的冷却液流失，所以相当于少遍历了一个bit。

具体什么道理看[官方Writeup](https://github.com/USTC-Hackergame/hackergame2023-writeups/blob/master/official/%E5%BC%82%E6%98%9F%E6%AD%A7%E9%80%94/README.md)吧，简单看了一下，觉得如果自己知道怎么查看逻辑相关的东西的话，应该很好做出来，感觉有点依赖于游戏熟悉程度了（具体细节我就不再探索了，如果是MineCraft我可能会看一下，我就这么双标🤪）。
