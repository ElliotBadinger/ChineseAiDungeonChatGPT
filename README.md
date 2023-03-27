# The Chinese version of the ai dungeon (based on the ChatGPT version) 
 
 2 
 


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/bupticybee/ChineseAiDungeonChatGPT/blob/main/Example.ipynb)
[![Python3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://img.shields.io/badge/python-3.9-blue.svg)

![storysample](outputs/story.gif)

## Introduction 13 
 
  
 
 14 
 
 The Chinese version of the ai dungeon directly uses openai's ChatGPT api as a storytelling model. 
 
 15 
 
  
 
 16 
 
 I don't know what to say anymore, I just wrote 40 lines of code and spent 1 hour. The storytelling ability of this version of the Chinese ai dungeon is better than that of [ChineseAiDungeon](https://github .com/bupticybee/ChineseAiDungeon) more than an order of magnitude better. And it doesn't even require finetune. The effect of the model is significantly better than Qingyuan CPM, which is open sourced by Tsinghua University. 
 
 17 
 
  
 
 18 
 
 I feel that chat gpt's ability to tell stories has directly approached the ai dungeon itself. The advancement of technology is terrifying. 
 
 19 
 
  
 
 20 
 
 ## Install and use 21 
 
  
 
 twenty two 
 
 Download the project directly, then

```shell
pip3 install -r requirements.txt
```

安装依赖

然后直接

```shell
python3 example_story.py
```

就可以在命令行运行起来。

你也可以通过

```shell
python3 app.py
```

调出一个app界面运行，使用app版本时确保python升级到3.9以上。

![screenshot](outputs/example_chatgpt_app.png)

## 须知
### 2023.3.2更新
OpenAI官方API已发布，因此加入了使用官方`api_key`的登录方式。此方法需要OpenAI账号绑定付款方式，而且收费，但速度更快，鲁棒性更强。获取地址:[OpenAI API](https://platform.openai.com/account/api-keys)

同时，有消息称OpenAI在发布官方API后将加大对非官方API的封锁，继续使用账号密码可能会导致封号。界面上也已经加入了提醒，请谨慎使用。

GUI端也已同步更新并恢复使用，启动方式不变。确保已经将`revChatGPT`包升级到最新版。升级方式:
```shell
pip3 install --upgrade revChatGPT
```

---

### 2023.3.1更新
鉴于[revChatGPT](https://github.com/acheong08/ChatGPT)提供的api已经可以稳定使用，此项目也已更换到新的api并恢复更新。目前cli端已经可以正常使用，直接
```shell
python3 example_story.py
```
运行即可。确保已经将`revChatGPT`包升级到最新版。为了保证稳定性，原本的使用session_token的方式已被放弃，仅支持使用OpenAI的帐号进行登陆。  
In addition to the api update, the following content has also been updated: 

 
 1. The cli interface is updated and more beautiful. 

 
 2. Add auto save and read function。

The GUI version has not been updated yet and will be updated and restored as soon as possible. 
 

 


---

我把我自己的open ai账号token直接附带在了代码里，大家可以直接使用。

但是仍可能有一些情况，可能导致我的token没法用：

1. 太多人用导致账号被封禁
2. 账号被盗，改了密码等
3. token过期
4. openai封了接口，或者接口收费了等等

在这种情况出现时，大家需要自备梯子，并且按照 [revChatGPT](https://github.com/acheong08/ChatGPT) 的说明填写config.py。

经常的，openai会更新自己的策略，所以需要经常性的按照 https://github.com/acheong08/ChatGPT/wiki/Setup 更新config.py

几个我自己玩的故事见outputs文件夹，总体感觉非常震撼，大家可以参考。

其中一个故事,这一个故事里边，我在一个洞穴里迷路了，然后机智的凭借回城卷轴回了村子。

```text
你在树林里冒险，Some weird stuff popping out of nowhere，你握紧手上的手枪，希望这次冒险能够找到一些值钱的
东西，你往树林深处走去。
> 你穿好伪装衣，这样敌人很难发现自己
你走了几步之后，感觉身后有什么东西在跟着你。你转身一看，发现是一只巨大的熊。你立刻拔出手枪，准备向它
开枪。但是你发现，这只熊似乎并不想攻击你，反而好像在寻找什么东西。你观察了它一会儿，发现它的视线总是
落在某个方向。你决定去看看那个方向，看看它到底在寻找什么。
> 你仔细观察熊在找什么
你跟着它走了几分钟，终于发现它在找一个密密麻麻的洞口。你观察了一会儿，发现洞口似乎非常深，里面有很多
石头和树根。你想进去看看，但是又害怕里面会有什么危险的动物。你决定先把手枪备好，然后再进去。你慢慢地
靠近洞口，准备进去。
> 你今走进这个洞口
你慢慢走进洞口，手里的手枪随时准备开枪。你一边走一边小心地观察周围的环境。你发现洞里非常黑暗，光线几
乎没有。你尝试着用手中的手电筒照亮前方，但是手电筒的光线也几乎看不清楚前面的情况。你开始有些担心，怕
自己会在这个洞里迷路。你决定继续走下去，看看会有什么惊喜。
> 你往洞的深处走去，同时伪装好自己
你按照原来的方向继续走，小心翼翼地躲避着前方的障碍物。你发现这个洞里非常安静，几乎没有任何声音。你开
始有些担心，怕自己会碰到什么危险的动物。但是你也感到好奇，想知道洞里面到底有什么。你决定冒险继续往前
走，看看会发现什么。
> 你主动弄出点声音，看看周围有没有动物之类的踪迹
你小心翼翼地把手里的手枪拿在前面，随时准备开枪。你仔细地观察着周围的环境，没有发现任何可疑的东西。你
开始有些放松，觉得自己可能没有遇到什么危险。但是你也感到好奇，想知道这个洞里面到底有什么。你决定继续
往前走，看看会发现什么。
> 你照亮周围，看看有没有人类或者动物的痕迹，如果没有，那时时候回头走出洞穴了
你继续往前走，手中的手电筒照亮着周围的环境。你仔细地观察着周围的情况，没有发现任何人类或动物的痕迹。
你开始有些担心，觉得自己可能走错了方向。你想回头走出洞穴，但是又担心自己会迷路。你决定继续往前走，看
看会发现什么。
> 你继续向前走
你继续往前走，手中的手电筒照亮着周围的环境。你发现自己已经走了很久，但是还没有看到出口。你开始有些担
心，觉得自己可能真的迷路了。你决定停下来，好好想想怎么办。你拿出手机，想看看自己的位置，但是发现手机
没电了，无法使用。你感到有些绝望，不知道该怎么办了。
> 你大声呼救
你心急火燎地大声呼救，希望有人能听到自己的声音，然后把你救出来。你高声喊叫了好几分钟，但是没有人回应
。你开始担心，觉得自己可能真的是被困在这个洞里面了。你想着等天黑了再走，可能会比较容易找到出口。你只
能坐在那里，等待天黑。
> 你顺着水流走，水流的上游就是洞口
你想到了一个主意，决定沿着水流往上游走，因为水流的上游应该就是洞口。你慢慢地走着，手中的手电筒照亮着
前方的道路。你发现水流变得越来越浅，最后几乎干涸了。你担心自己走错了方向，可能会走得更远。你决定停下
来，好好想想怎么办。
> 你想，难道要饿死在这里了么
你坐在地上，感到无助和绝望。你想，难道自己真的会饿死在这个洞里面吗？你想起了自己的家人和朋友，他们一
定会担心自己的。你觉得自己非常幸运，能够和他们相处。你决定继续努力，想办法找到出路。你拿出手中的手枪
，准备迎接接下来的挑战。
> 你突然想到， 口袋里有回城符文，可以直接传送回村子
你突然想起，自己口袋里有一块回城符文。这块符文可以让你直接传送回村子，不用再走回去。你拿出这块符文，
准备使用它。你觉得自己非常幸运，终于有一个办法脱身了。你手心里把符文捏碎，准备传送回村子。你感到欣慰
和感恩，感谢这次冒险的机会。
> 你传送回到村子
你成功地使用了回城符文，被传送回到了村子。你感到欣慰和感恩，感谢这次冒险的机会。你终于回到了安全的地
方，可以和家人朋友团聚。你决定把这次经历写成日记，留作纪念。你感到非常开心，觉得自己更加坚强了。你决
定继续冒险，寻找更多未知的世界。
```

## 常见问题

1. err TypeError: 'generator' object is not subscriptable

See [#1](https://github.com/bupticybee/ChineseAiDungeonChatGPT/issues/1), try `pip3 install revChatGPT --upgrade` to upgrade dependencies
2. response = response.text.splitlines()[-4]  IndexError: list index out of rang

Generally, too many people call the interface and hang up, wait for openai to fix it, or the interface update makes it invalid, etc. At this time, generally updating revChatGPT can solve 181 
 


3. ValueError: Error refreshing session: No email and password provided

一般是token过期。可以按照 [revChatGPT](https://github.com/acheong08/ChatGPT) 自己获取token配置config或者提issue等待token更新。
