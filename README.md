# Python implementation of 植物大战僵尸 ol 助手

使用 Python 实现的植物大战僵尸 ol 助手。

该项目为开源项目，项目地址：https://github.com/bwnotfound/pypvzol

注意，目前支持私服不支持官服，等私服适配加完后再适配官服。

## 关于开源协议

植物大战僵尸ol助手 © 2023/11/25 by 蓝白bw is licensed under CC BY-NC-SA 4.0. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/

本项目使用的开源协议为 CC BY-NC-SA 4.0，该协议要求署名、非商业使用、相同方式共享。

## 声明

本项目为开源项目，项目的贡献者不知道所有用户的输入，因此不负责任何用户的输入。

因使用本项目而造成的任何损失和影响都与本项目贡献者无关，用户需对自己的操作负责。

本项目仅供学习交流使用，不得用于商业用途，否则后果自负。

将该项目用于任何途径造成的任何损失均由自己承担，项目拥有者不负任何责任。

使用本项目的任何代码或者二进制文件都视为已同意本声明以及LICENSE文件声明的协议。

## 使用规约

1.  本项目是基于学术交流目的建立，仅供交流与学习使用，并非为生产环境准备，因其造成的损失将由自己承担。
2.  任何基于本项目制作的视频都必须在简介中声明项目来源。
3.  不可用本项目进行网络攻击。
4.  禁止使用该项目从事违法行为与宗教、政治等活动，该项目维护者坚决抵制上述行为，不同意此条则禁止使用该项目。
5.  继续使用视为已同意本仓库 README 所述相关条例，本仓库 README 已进行劝导义务，不对后续可能存在问题负责。
6.  如果将此项目用于任何其他企划，请提前联系并告知本仓库作者，十分感谢。

## 使用提醒

1.  请一定要看控制台的输出，因为报错信息并不会全部都在日志面板上显示，同时日志面板也不是很方便
2.  Cookie 的获取方法如下：打开`cookie.xml`文件找到`<UserCookies>......</UserCookies>`。中间省略的就是cookie。

## 通用使用方法

1.  要删除列表物品，选中物品并按“删除键(Delete)或者“退格键(Backspace)”即可（这点操作基本是通用的）
2.  大部分列表支持多选。多选方法：按住 ctrl 然后左键即可
3.  当希望刷新助手数据，请手动点击`刷新仓库`然后再打开对应窗口即可

### 运行源码

1.  python 版本选择: 3.10.6 (理论上 3.8~3.11 都可用)
2.  安装依赖:
    ```shell
    # 如果可以的话，建议使用虚拟环境venv
    $ pip install -r requirements.txt
    ```
3.  运行：
    ```shell
    $ python webUI.py
    ```

## 后话

~~关注 B 站[蓝白 bw](https://space.bilibili.com/107433411)喵， 关注[蓝白 bw](https://space.bilibili.com/107433411)谢谢喵~~

### Q&A

1.  Q: 为什么要叠这么多甲呢？

    A: 别问，问就是没版权爱发电。

2.  Q: 为什么压缩包这么大

    A: 因为 python 的一个库(pyqt6)很大

3.  Q: 为什么官服不能用？

    A: 小傻瓜，还玩官服呢。之后可能会适配官服，当然大概率是不考虑官服适配了

4.  Q: 私服怎么玩？

    A: 请自行B站查找教程，这里不提供相关教程


## TODO LIST:

#### 新加内容

1.  能够刷新用户面板的数据
2.  添加一键指令：打洞、jjc。例如jjc就是允许指令的话就一键打，不能再一个个打
3.  把带级和刷洞区分一下
4.  自动速度复合
5.  自动复合加入是否全传给主力的选项。自动复合优化ui，分隔按钮
6.  添加一键设置所有账号的延时时间功能
7.  自动开魔神，选择是否刷无极，然后带级并自动复合
8.  (可选)云端助手，提供服务器选项，可以搭载到云端然后远程使用，类似远程操控
9.  (可选)加默认模板和种子文件识别功能
10. 多个账号共同设置除了打洞之外的功能
11. 日志本地存储
12. 跨服次数限制到多少次为止
13. 多线程开箱
14. 加入一键剔除合成池复合池中数值超标的植物
15. 战斗模拟，模拟不同专属和配队的性价比
16. 判断难度4打的是谁
17. 检测领地设定难度以上是否有好打的的智能机制
18. 自动复合加速，底座分出去的时候分出去的和底座同时滚
19. 自动复合并行滚多个属性后再全传
20. 多开小号功能改善：
    1.  添加统一时延选项
    2.  添加运行检测是否已经完成所有工作了
    3.  添加账号运行池，即每个时刻都只有m个账号运行，一个账号完成所有工作后退出并打开新的账号运行
21. 添加跨服队伍设置
22. 全自动能检测背包剩余容量

#### BUG LIST

1. 进化、自动开箱的超时bug处理并单独线程处理
2. 领地开打前检测是否有挑战次数，没有就不打，避免上植物搞得别人打不了
3. 全自动留待修复：
   1. 买东西如果买相同的东西就会无法成功购买