also:: 归来还是苹果
icon:: 📝
created:: [[20240831]]
exclude-from-graph-view:: true
status:: writing/draft
tags:: #macbook

- okey，[之前喷过]([[weekly/1170-refund-macbook-pro-m2pro-16]])，但现在仍然选择入手，这让我感觉自己是个小丑 🤡
- 这次和今年过年的情景不太一样，ARM on Windows 已经发布，我也明白了 Mac 的设计有多傲慢，并且可以随时全款拿下最新的 MBP，但我最近还是分期买了 13 inch MBA 24 + 512，而这是我给出的理由：
  - 设计
    logseq.order-list-type:: number
    - Apple 本来就不是一家科技公司，而是是一家设计公司；
      logseq.order-list-type:: number
    - 双持永远是最优解
      logseq.order-list-type:: number
      collapsed:: true
      - 须知参差多态，乃是幸福的本源。
        logseq.order-list-type:: number
      - 很多争论，比如选 Android 还是 Apple，选 Windows 还是 Mac，双方各执一词，各有所长，各有所短，却总是追着互相揭短，看久了完全没有意思。
        logseq.order-list-type:: number
  - 体重
    logseq.order-list-type:: number
    - 13 inch 的体重只有 1.3kg，比起 14MBP（1.56kg）和16MBP（2.1kg）来说，好上不少
      logseq.order-list-type:: number
    - 外出（春运、图书馆）来回很方便；
      logseq.order-list-type:: number
    - related: ((66d29d71-3685-4d6e-bcb9-045e6256c024))
      logseq.order-list-type:: number
  - 续航
    logseq.order-list-type:: number
    - 长时间 [[logseq]] 的码字，而非敲代码，或是做编译；
      logseq.order-list-type:: number
      id:: 66d3d99d-1941-45a4-9e44-82f4a019ed12
    - 之前买 [[pad]] 的原因，也有一部分看重轻便和码字
      logseq.order-list-type:: number
      collapsed:: true
      - 系统（PadOS 和 Android OS）完全限制了 Pad 的用途；
        logseq.order-list-type:: number
  - 无风扇
    logseq.order-list-type:: number
    - 被动散热影响散热，但参考使用场景： ((66d3d99d-1941-45a4-9e44-82f4a019ed12))
      logseq.order-list-type:: number
    - 不需要清灰，直到用坏那天也不会打开后盖，省事；
      logseq.order-list-type:: number
  - M4 设计思路的转变
    logseq.order-list-type:: number
    collapsed:: true
    - {{video https://www.youtube.com/watch?v=EbDPvcbilCs}}
      - {{youtube-timestamp 499}} 用 60% 的功耗，去跑 20% 的性能提升？
        - 跟 M1 和 M2 的设计思路完全不一样
  - 类 Unix，Shell 支持好；
    logseq.order-list-type:: number
  - Mac 的色彩管理、字体显示非常舒服；
    logseq.order-list-type:: number
  - ARM on Windows 兼容性一般，并且续航仍然不敌 Mac；
    logseq.order-list-type:: number
  - {{embed ((66d2906b-7503-4d60-9e2b-93322b1e623d))}}
    logseq.order-list-type:: number
-
- 但说实话，很多软件，其实是 Apple 在依赖 Linux on ARM，Apple 真的应该付钱给 Linux...
-
- ## ↩ Reference
  - > 差不多 10 年前，我特别喜欢苹果笔记本电脑。我现在还记得当时有这些优势：
    * Retina 屏幕。在那个桌面平台 1440x900 ，笔记本 1366x768 分辨率的时代，2K 分辨率真的十分惊艳，画面特别细腻；
    * 屏幕色彩好。当年的笔记本普遍使用 42% NTSC 色域的 TN 屏幕，色彩方面挺糟糕，可视角度也很一般，画面上下两半的颜色都不太一样；
    * 好用的终端。当时 Windows 终端不说字体和生态之类的问题，光是 cmd.exe 这玩意，最大化都只能占左半边屏幕，宽度是固定的。虽然有 Cygwin 和 MSYS2 ，但仍然有许多开源软件没有移植到 Windows 平台，或者存在兼容性问题。虽然有第三方终端软件，但仍然没有任何一款能做到选定后按 Ctrl+C 复制；
    * PCIe 协议的固态硬盘。虽然那个时代的 HFS+文件系统性能不怎么样，但在硬件方面，PCIe 的固态硬盘顺序读写速度能超过 1000MB/s ，那时候绝大多数 Windows 笔记本只会配备机械硬盘，或者 32GB 的固态加上一个大容量机械硬盘。买一个 128GB 的镁光 M4 固态都要 1000 多元，而且顺序读写因为 SATA3 的限制，只有 550MB/s ；
    * 大电池。当年的 Windows 笔记本虽然厚，但是内部空间利用率不高。许多笔记本的电池做在屏幕下方，只有两个拇指的宽度那么大。而 MBP 内部设计紧凑，剩余的空间塞满了电池，在当时就拥有了相对更长的续航；
    * 触摸板。当时的 PC 触摸板有一部分低端产品不支持多指触控，没有任何手势支持，甚至还有延迟。好一点的支持多指触控，但只是驱动程序会把手势映射成键盘快捷键或者鼠标滚轮操作。大多数手势都是做完动作之后才开始响应，滚动页面也是按行滚动，而不是按像素滚动。
    * 开源软件生态。我记得当时前端工程化刚起步，很多东西不完善，npm 下载的依赖路径会超级深，在 Windows 上因为路径长度限制都会抽风。虽然这是 npm 的设计缺陷，不过用 Mac OS X 确实能规避这些问题，比较省心。
    * 虽然不完全是操作系统的优势，但硬件和价格（没错）方面都有实在的优势，只要预算够了，买了之后基本上不会觉得不值。不喜欢 Mac OS X 也可以装一个 Windows ，体验也不会比同期的 Windows 笔记本差。
    如今的话，优势大概有续航、外放音质、MiniLED 屏幕这些，对比起来曾经拥有的优势如今也没有那么明显了。音乐创作、自媒体、平面设计师可能会有生态优势。
    * 软件开发方面，我个人感觉已经没太多优势了，倒是 Windows 更有优势。现在苹果迁移到了 ARM 指令集，只要做的项目用到的东西多，总能碰到兼容性问题。有时候到网上一问，问题可能没解决，反而有不少人会说“公司没有开发用的服务器吗？什么年代了还需要在本地调试？”。如果是指本地只需要开个浏览器或者 IDE ，再开个终端，其他的一切都在云端，电脑坏了换一台开机连上去马上无缝衔接工作的那种，那还真没有。我只知道字节跳动有。
    当年就有一种说法，现在仍然有。说的是本地和生产环境如果更接近，开发和测试都更方便。我感觉如今的 Mac 系统和生产环境差异其实挺大的，除非做的是前端之类的。
    多年前因为这个说法，我有超过 3 年的时间完全用 Linux 桌面来干活。做开发是挺爽的，就是桌面环境小毛病挺多，图形界面软件生态少。有时候硬件驱动之类的毛病也多，比如 WiFi 突然掉了，不重启则再也连不上。
    后来我就想要一个既有部分 Windows 优势，又有部分 Linux 优势的系统。曾经 Mac OS X 是个不错的选择，办公、文档、沟通协作之类的没问题，软件开发大多数时候也没问题，一些问题也可以用虚拟机或者 Docker 解决。
    * 自从苹果迁移到 ARM 指令集之后，我反而感觉今天的 Windows 才更接近这个形态。虽然有人说 WSL 也有问题，比如 IO 性能差（访问 NTFS 分区的时候），WSL2 跑在虚拟机里，没有 systemd （现在有了，mac 从未有过）等等。
    这类问题确实存在，不过若标准是“要无比接近真正的 Linux 环境，否则没办法开发”的话，那 macOS 反而差的更远了。很难想象会有个 Linux 相关的问题，WSL 下没办法搞定，换 macOS 反而解决了。这个要求当然得直接用 Linux ，不必考虑 Windows 和 macOS 。但大多数后端开发工作还真没有这么高的要求，很多都是曾经的 macOS 也可以干的。
    * 我现在可以把沟通协作、编写代码之类的工作放在 Windows 环境中，运行调试放在 WSL 里。若直接用 Windows 运行调试也行的话，就更方便了，更显不出 Mac 曾经的优势了。用 WSL 开始可能会略微折腾一些，但确实能解决问题，测完上生产环境基本不用担心有什么差异。比起 Linux 桌面的那些问题，我更能接受这个。
    * 最近有些项目用到了 PyTorch 和 CUDA ，如今的 WSL 环境做测试也可以搞定。当然训练不必本地跑，但本地做的工作有时候是一些针对 NVIDIA 显卡的调优工作，改善一下性能。这些用 CPU 运行的模式下其实走不同的代码分支，并不一样。至于“公司没有开发用的服务器吗？”这个问题，有，但不方便，比本地开发调试麻烦多了。
    之前还看到过一种说法：“WSL2 也是跑在虚拟机里，那为什么不直接用虚拟机？”。其实上面的例子用虚拟机就很难搞。WSL 启动速度远比虚拟机快，和 Windows 的集成也很便利。例如，WSL 里面的端口会自动转发出来，直接用 Windows 程序连接上；管理 WSL 内部的文件，可以在命令行里输入 explorer.exe .来用 Windows 资源管理器直接打开，就好像在管理 Windows 的文件一样； WSL 能访问 NTFS 分区上的文件，如果需求对 IO 性能不敏感，也可以在 WSL 下直接编译运行 NTFS 分区里的代码。
    要是做嵌入式，尤其是那种编译工具链只给 Linux 下的，烧录工具只给 Windows 下的，直接打开 WSL 编译就完事了。
    Mac 的话，如今的体验有点像用能跑 JetBrain 全家桶的高性能树莓派来做开发，很多东西的生态其实还得看 Linux ARM 的生态。
    如果需求是买来当终端机用，远程连接开发环境，或者做前端开发，或者只用完全跨平台的语言和库来做开发，甚至是 iOS 和 macOS 开发这种不得不用的，那么用 mac 的开发体验应该还不错。系统界面还好看。就是之前 JetBrain 的 IDE 时不时会卡顿，我不知道现在怎么样了。
    https://v2ex.com/t/920796
  -