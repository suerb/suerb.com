# [译文] UX 设计中的功能动效

> 小小译文，翻译很烂，先挖坑，慢慢填。

> 文章来源：[Functional Animation In UX Design - SMASHING MAGAZINE](http://www.smashingmagazine.com/2015/05/14/functional-ux-design-animations/)

> 进入译文。

一个好的 UX 设计师可以轻易地解释任何设计决策背后的逻辑，包括了信息架构、内容层级、流程等等。

终有一天，动效会被引入到产品概念原型里面，到那个时候，设计师们会更难解释原型中的设计想法。“这动效很 cool 啊~”、“很接地气~”、“效果惊呆了”将会

## 什么是功能动效

**微妙**的功能动效作为设计流程的一部分，深藏于日常 UI 设计之中。

功能动效有别于 Disney Studio 、或者专门为电脑游戏设计的动效。它带有明确的、符合逻辑的用途，目的是为了支持我们所推行的设计解决方案。

在理想状态下，我们能通过一套完善的使用原则来验证这些功能动效的可行性。在过去的几年里，我接触过各种各样的项目。在这个过程中，我总结了 9 个类型的动效原则，若我们设计当中的某个动效遵循这些原则之一（或多个），那它就是一个有效的功能动效，证明可以被应用于项目当中。

如果功能动效不符合这些原则，那它可能就是多余的，使用的时候需要三思而后行，这些动效通常会让人感到讨厌和笨拙。

下面是目前为止我所收集到的所有用途。希望对你们的动效设计与验证有所帮助。


## 引导 Orientation

方向阐明结构。在这类型的原则里面，动效作用于界面之间的导航，展示网页信息架构的走向。这类型动效背后的逻辑，就是为了帮助用户感知自己在页面流程中的位置，理解页面的变化，是什么触发这些变化，以及有需要的话如何再次触发它们。

一个典型例子就是通过按钮触发切换「展示/隐藏」 内容，当你点击按钮后会展示一个被隐藏的面板，当你关闭面板后，面板会「缩」回操作按钮里面。

用户在第一次使用的时候无法预知此交互将会带来啥结果，隐藏面板的不断增大的展开动效会帮助用户保持方向感，让他不会感到已经跳出了当前页面，或者内容突然间消失了。关闭动效让用户将不断“收缩”的面板与操作按钮联系起来，这样一来，他们下次就会记得如何打开这个面板了。

**用法：避免突兀的过度转场，帮助用户定位。**

[![Apple Mac OSX 的窗口动效](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-orientation-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-orientation-01.gif)

[![Facebook Paper 的菜单动效](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-orientation-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-orientation-02.gif)


## 操作切换 Same Location, New Action

有一条广为人知的可用性原则，就是让产品保持一致性（译者注：设计与功能的一致性）。保持良好一致性的网站（产品）可让减低用户的学习成本，让内容与交互有良好的可预见性。除此之外，这条原则还适用于操作按钮。

在某些案例里面，当按钮被触发后，我们被迫在特定条件下改变这个贵按钮触发后的功能，通常出现在那些总体空间受限的设计当中。因此，已经理解了按钮初始功能的用户，可能需要学习一下新功能了。

「保存」与「编辑」按钮算是最常见的可切换按钮了。这个算是最简单的案例了，因为只要按钮的定义是相反的（译者注：例如「添加」点击后变成「移除」），就等于他们在同一场景下。在其他情况下，当两个操作没有直接表面关联时，才算是可用性的难题，这时候，你需要功能动效。

**用法：强调操作按钮的功能切换。**

[![Google Material Design 的 Button](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-toggle-actions-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-toggle-actions-01.gif)

[![静音开关](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-toggle-actions-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-toggle-actions-02.gif)


## 放大 Zoom In

第三种类型与「定位」类型相似。在这类动效里，用户在列表视图里面选中某个项来放大进入详情视图（覆盖原有列表视图），并且可以返回列表视图。

通常应用于相册、卡片和项目选择器。用户会选择一个选项然后马上看到与之相应的详情视图。

要使用这类型动效的难处在于，需要确保用户感觉自己仍然能 hold 住局面并且不脱离当前场景。在这个情况下，功能动效是必不可少的。

体验过大量使用这类型的功能动效后，我总结出一些通用规则，若严格执行则功效显著：

1. 动效的初始状态就是原有列表视图；
2. 每个选项都被指定一个视觉线索，这个线索可以是这个应用的主题色，也可以是某种符号、加粗的标题或者缩略图；
3. 当用户作出选择后，将会新建一个页面，然后视觉线索会移动到一个突出的新位置。例如，可以用选项的独有颜色来填充整个页面；选项的符号可以放大并且移动到页面标题处；选项的名字可以放大并作为页面标题来展示；
4. 一个显眼的操作按钮，用于退出这个新页面，例如「取消」，「关闭」，「返回」或者「X」。

**用法：将预览视图与细节视图联系起来。**

[![求来源](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-zoom-in-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-zoom-in-01.gif)

[![Google Material Design 风格的日历](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-zoom-in-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-zoom-in-02.gif)

## 视觉隐喻 Visual Hint

视觉隐喻帮助用户更好地理解如何与产品界面交互，那些含有非主流组件或者特别导航系统的则更加需要视觉隐喻。

这类型功能动效很容易被发现，当我们打开一个页面，一个一次性的动效会立即被触发，并演示某个功能如何使用。

**用法：为不常用功能或者隐形操作提供暗示。**

[![来源：https://dribbble.com/shots/1964352-Tasking-App](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-hint-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-hint-01.gif)

[![www.buildinamsterdam.com](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-hint-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-hint-02.gif)

[![来源：Dejan Markovic](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-hint-03.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-hint-03.gif)




## 强调 Highlight

这类型的动效帮助用户在满布繁杂元素的界面中做出有效操作。

设计师通常都会尽量避免设计出复杂的界面布局————满屏尽是多媒体————不断争夺着用户的眼球。

减少噪音的其中一个方法就是删繁就简，然而有时候这是不可能的任务。你想想，要求一个新闻网站的老板移除新闻的文字内容模块和首页的图片栏目……

在 UI 界面当中，「运动」有一个很重要的特质，就是最容易吸引注意力，文字段落或者静态图片都无法与之媲美。我们可以利用这一点来设计动效。然而请谨记，最容易吸引注意力同时也是一种「干扰」，滥用的话等同于在界面中增加噪音。

**用法：在繁复的界面中吸引用户的注意力。**

[![www.Photojojo.com](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-hightlight-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-hightlight-01.gif)


## 模拟现实 Simulation

有时候，通过数据分析与用户访谈，我们发现用户的某些需求只能通过定制特定的界面来满足。

对于这些特殊用例，我们可以考虑设计一个自定义的功能动效。常用的方法很难完美实现某些独特的案例。

**用法：适用于那些难以表达含义的场景。**

[![来源：Monterosa](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-simulation-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-simulation-01.gif)

[![求来源](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-simulation-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-simulation-02.gif)



## 视觉反馈 Visual Feedback

在 UI 设计当中，视觉反馈非常重要，在真实生活中，按钮、控制器和其他物件都会响应用户的交互操作，这就是用户所期望的事物的运作方式。

但请谨记，视觉反馈这类型功能动效应该尽量“低调”，并且设计得易于理解。按钮反馈被广泛应用于每个 UI 界面，因此如果滥用没必要的动效会适得其反。

**用法：响应用户的操作。**

[![求来源，与此类似的有 tumblr](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-feedback-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-feedback-01.gif)

[![Google Material Design](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-feedback-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-visual-feedback-02.gif)


## 系统状态 System Status

这类型完全就是关于“控制”的。对于用户来说，“控制”意味着在任何时候都可以感知和理解系统的当前场景。

功能动效实时监测系统状态，让用户快速感知操作的开始、剩余时间与准确的完成时间。也许第一个满足此需求的功能动效就是 HTML 页面的“转菊花”GIF，目前还被广泛使用于某些操作指示界面。

优质的系统状态功能动效通常都遵循以下模式：

1. 在进程开始后展示清晰的反馈；
2. 在进程进行中提供反馈；
3. 估算进程的完成度，并提供反馈；
4. 在进程结束后提供成功或失败反馈。

有个很出名的动效“下拉刷新”，就是属于本类型动效，在移动设备上，它常用于触发内容的刷新。在几个不同类型的 apps 中检验一下，你会发现这些动效都没有完全遵循上述 4 个步骤，感觉怪怪的。例如，语意不明地抬升界面来结束进程，会让用户再一次触发下拉刷新。

**用法：传达出操作处理过程的可控性。**

[![求来源](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-system-status-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-system-status-01.gif)

[![http://www.yikyakapp.com 的下拉刷新](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-system-status-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-system-status-02.gif)

## 营销手段 Marketing Tool

这类型虽然只与市场营销有关，但已经有很多有趣的动效。之前的 8 个类型看起来都与理性和逻辑挂钩，但是这类型只与感性有关。

假设我们需要定义一个产品的行为，突出独有的功能，甚至捆绑品牌价值和风格。

在这些场景剧本当中，这些方法虽然未必是以用户为中心来设计，但却拥有明确的功能目标————可以满足公司的营销策略。

**用法：帮助突出公司的品牌价值，或者产品的强项。**

[![来源：https://dribbble.com/shots/1901531-Loading](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-marketing-tool-01.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-marketing-tool-01.gif)

[![www.Bellroy.com](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-marketing-tool-02.gif)](http://7xigda.com1.z0.glb.clouddn.com/functional-ux-design-animations-marketing-tool-02.gif)


## 总结

在我们的网站或者和移动产品添加动效，可以为用户带来很多惊喜与愉悦，但请谨记——**形式服从功能，任何毫无用途，不是为了满足实际功能需求的，为了动效而动效，请勿滥用动效。**





