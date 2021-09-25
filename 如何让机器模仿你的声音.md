# 如何让机器模仿你的声音

“Hey Siri ，明早 7 点叫我起床。”

“小度小度，帮我查一下原子弹该怎么造。”
当代生活，你跟机器说的话可能比跟你爸妈说的话都要多。这些触手可及的语音助手、智能音箱不仅能听懂你的意思，做出回答，还能变换各种音色，乃至模仿你的声音。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXR157LqaJRpJRe4liaWic0icgOZiaQw2CjEzribQOZAONfyXRn6lB0UKduOA/640?wx_fmt=png)
这在今天已经不算稀奇，但实际上，想让机器说人话，可比你爸妈当年教你说话难得多，而要想让机器模仿不同人的声音说话更是难上加难。
世界上第一台能合成人声的电子设备，是这款首秀于 1939 年纽约世界博览会的 Voder 。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaX0P6XyDbyaiaETMpNc3bk0N2GgnG7pJeBO5sECoFFqN1jUDEA9eV8uPg/640?wx_fmt=png)
它采用的是参数合成法，准确的说是共振峰合成。什么是共振峰？
人说话产生的声音包含很多不同的频率，其中频率最低的称为基音，决定了音高，此外就是泛音，决定了音色。而共振峰就是频谱上能量相对集中的这些泛音。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXgkIxAhWNy4PF8JeYMZibia5wkeFMIa6Kdbm30m1ib84RRiaqGTibg3DWhEg/640?wx_fmt=png)
比如当发音人为男性时，汉语里 i 这个元音的基频，即基音的频率约为 210Hz，而在泛音中，频率最低的共振峰 F1 约为 290Hz，第二低的共振峰 F2 约为 2360Hz，第三低的共振峰 F3 约为 3570Hz 。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaX7O9oRA8eSv9EOakTB6YnNiaUPV8ZMKUQmOMrALNnXjPqlIkYBWwaSyg/640?wx_fmt=png)
通常来说，只要反过来让机器发出这四个频率的声音，就能简单地还原出带有男性音色的 i 这个元音。
Voder 就是基于这个原理，下面是它的工作流程图。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaX01icDH7ia3RZJlG8lmp2JrMu0PbzOubyrM2mvjEpejF12HX0eibkqJhFg/640?wx_fmt=png)
首先，利用脉冲发生器可以模拟出声带振动产生的浊音，用噪声发生器可以模拟出声带中由气息形成的清音，两者将与手腕处开关生成的基音叠加，进入一个声道滤波器。 这个滤波器由两组按键控制，每个按键对应着不同频率的声音，当操作员同时按下不同的按键，就会加入不同频率的泛音，最终组合成语音。
在此后的半个世纪里，这一直是让机器说话的主流方法，并且通过升级电路和引入更复杂的参数摆脱了人工操作，但合成出来的声音仍然带有非常强的“电音”。

毕竟，人类的语音包含的声音频率信息非常复杂且丰富，用机器简单组合出来的语音在音调上多少会有差距，更别说还有发音的长度、韵律、节奏等影响因素，如果也要人为地用参数来量化，将是个无比庞大的工程。
于是，波形拼接法出现了。
既然用参数很难合成出逼真的人声，那么干脆录下真人的语音，再通过拼接组成我们想要的语句。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXia8icQDvdpAWbm7y4SEne8xiaWFayUiagDIqPVtqT6cx6teBL2gQvAnzUw/640?wx_fmt=png)
比如你手机上的地图应用，在语音导航时如果需要播报 “前方路口右转，进入朝阳门外大街” 这类指示，最简单的方法就是从语料库中选取每个字的发音拼接组合成一句话，不过这样并不自然。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXicwxnHrtqEQMJ95mIEK7vUbpwQyMKcEuwLAeGh3Khibuo2slwPRMuoibw/640?wx_fmt=png)
更高级的方法是从语料库中选取短语拼接，但这样在拼接处依然会有韵律的断裂感。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXZdH468QWwDgh3QVic77UicqnzKntorJTMBEtu3tuGN5NdA9B0icEPcfEw/640?wx_fmt=png)
要想更自然，就得从语料库中选取韵律相近的短语拼接，而这就要求语料库必须足够庞大。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXy7TmhJwtzbaEYib99bcfGYicIrLxEZepjibdayCZ33VrZStViaRxVItzxg/640?wx_fmt=png)
像地图应用推出的明星语音包，使用波形拼接法可能需要提前录制一万句话左右，且还须在专业的录音棚以保证语音质量，再经后期处理制作，前后需要两三个月的时间。
正因为此，定制语音包一直以来都只是明星的特权，直到 9 月 19 日，百度地图上线了一项语音定制功能，任何人只要读 20 句 15 个字左右的短句，传输到云端的服务器，经过约 15 分钟的训练，就可以下载一个具有你说话特征的导航语音包。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXJHWDibSgsYKpicUXE3G6WefS5fop922rIbjwa2FOl3ibRvLGibqnibJllYw/640?wx_fmt=png)
百度地图是如何只用这么少的语音样本、这么短的时间就能让机器模仿你的声音的？
答案是深度学习神经网络。
比如 2017 年百度发布的 Deep Voice 。这个系统以音素为基础的分析单位，音素指的是根据语音的自然属性划分出来的最小语音单位，比如汉语音节 ā 只有一个音素，dā 就有两个音素。
系统中的五个模块会从大量的语音和文字数据中，学习如何划分提取音素、以及音素的基频、持续时长等参数，然后再利用声学模型合成语音。
这种方法本质上也是参数合成，但优势在于，深度学习神经网络能从大量数据中快速学习、找出规律，也就是说，通过这种方法设置的参数相比传统的参数合成法要更准确。

不过，这个模型一次只能学习一个人的语音，且对发音人的录音质量和数量依然有非常高的要求，要想在手机这样算力有限的小型设备上，实现只用 20 句的语音样本花 15 分钟合成定制语音，几乎不可能。
在 Deep Voice 发布的同年，百度陆续又推出了 Deep Voice 2 ，这个模型已经可以学习数百种不同的语音，而后续的 Deep Voice 3 已经能做到在半小时内学习 2500 种语音，并从中提取出不同声音特征的共性和个性。
不仅如此，前两个版本的 Deep Voice 在训练时是基于深度学习神经网络，但在合成语音时还是采用跟传统的参数合成类似的方法，而 Deep Voice 3 不论是训练还是合成都基于深度学习神经网络，这让合成出来的语音要自然得多。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXrXFibH3SpBSy0cv2qnQxNoYSScs413Bg3FKn0Dibrtu55hp575I0Aptw/640?wx_fmt=png)
正是依赖这些语音合成技术的更新换代，百度扫除了阻碍语音定制功能大规模商用的三大难点：如何只用少量的数据合成语音？如何快速地合成语音？如何在手机这样的小型计算平台上使用语音合成？ 百度在地图语音定制功能上应用的 Meitron 模型首次让语音合成技术真正走出了录音棚、实验室。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXibvAZjZo2icgu2xIlI6X1icvibeklb4tJYYBJnMxgPIV91FLIBV0cFaLIA/640?wx_fmt=png)
Meitron 模型可以有效学习和分离声音样本中包含的音调、韵律、节奏等各种维度的信息，在实际使用过程中，20 句的录制语音经过特定挑选，尽可能覆盖了最大的语音要素。
而且，虽然你录制的都是 “夏天要走了，秋天要来了” 这类中文语句，但最终却可以合成出 “GPS” 这样的英文短语，这是传统的参数合成或波形拼接难以做到的。
![img](https://mmbiz.qpic.cn/mmbiz_gif/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXW67eFInZmFCYHPhBCK8icD8oSyH5UvC5GKUxQdlTibNfYgjVrZFjyO9g/640?wx_fmt=gif)
更重要的是，Meitron 模型是一个足够轻量级的训练平台，从而实现迅速部署和服务器上快速的模型训练。当你录完这 20 个短句，只需传输到百度地图的服务器，合成完后就可以把具有你说话特征的导航语音包下载到手机上，过程中无需繁琐的人工调校，方便快捷。
在这项功能的加持下，语音定制从此不再是明星的特权，不仅如此，这些定制化的导航语音包还可以在亲朋好友间共享使用。
当你在异乡生活，开车时听着你爸或你妈的声音导航，不仅多了情感上的陪伴与支持，更能让你心平气和地驾驶，再也不好意思超速、加塞、乱按喇叭了。
![img](https://mmbiz.qpic.cn/mmbiz_png/U6yRaDu1NabLs95X3icIMTIiaXHrahnuiaXLmgfakk6Xwh6lFZKgFu8JnYRXv7e7iaYpUezElDVrXiadYzdVMqXhYWA/640?wx_fmt=png)
现在，你就可以打开百度地图，唤醒 “小度小度” 后说 “我要录制语音包” ，即可体验这项语音定制功能，亲自为自己和别人导航指路。