# Android技能自我评测
- 有个开发人员曾经跟我说，他很迷茫，接下来是该去看Android系统源码，还是每天继续做应用，但是感觉每天都是画UI和调用MobileAPI处理JSON,没有技术上的提升空间。
这个问题我思考了一个晚上，列出来一个从事Android应用的开发人员所需要精通的20个技能点：

1. Activity相关。App应用开发，以Activity使用最多，涉及LaunchMode、onSaveInsatnceState、生命周期等技术
2. Fragment相关技术。用的人不少，想明白是咋回事的人不多。这里推荐一本书《Creating Dynamic UI with Android Fragments》
3. 序列化技术。有Parcelable和Serializable两种。前者是基于Service的，后者是基于Bundle的，二者实现原理不同但是达到的效果差不多。
4. ImageLoader的原理和使用。类似的，还可以学习Facebook新近开源的Fresco，它对图片的处理会更好一些。
5. fastJSON或GSON的使用。做App不会用实体自动匹配JSON数据，相当于白做。
6. 多线程相关。包括Handler、Looper、ExecutorService等。
7. Adapter和ListView。这两个技术捆绑在一起，经常容易崩溃，尤其是分页的时候，要仔细研究深刻体会。
8. 用户Cookie设计。需要吧登陆机制彻底搞清楚，包括在HttpRequest头中夹带Cookie来进行用户身份登陆验证的技术。
9. 网络请求封装。使用AsyncTask的网络底层封装，使用Handler + Runnable的网络底层封装。
10. Android与HTML5的交互。包括Android调用HTML5的方法，以及HTML5调用Android的方法。
11. 代码混淆。没用过ProGuard，不知道keep相关语法，就还是初级水平。
12. Android打包机制。涉及Android SDK中的若干命令。对Android打包过程做的每一件事都很清楚。进一步是Android多项目依赖的打包技术。Ant、Gradle或者Maven，掌握其中任何一种打包机制即可。
13. 线上Crash分析并修复。要具备通过分析Crash信息修复线上Crash的能力。
14. 内存泄露。包括内存优化、内存泄漏的场景、MAT工具的使用。
15. 调试工具。包括DDMS、Eclipse或者Android Studio的调试功能。
16. Monkey机制。Android开发人员如何对一款App进行Monkey测试。这算是附加技能吧。
17. 单元测试。这里指的是JUnit。对复杂的算法写过单元测试以保证其没有问题。
18. GIT的高级功能。包括Stage、Rebase、Revert、Stash、CherryPick和Sub Module等概念。如果项目中使用的是SVN,那么要掌握SVN的版本管理策略。
19. 插件化编程。哪怕知道一点DexClassLoader的概念也好。这年头，没做过插件化编程，出门面试都不好意思说自己是做Android开发的。
20. 设计模式。对常见的设计模式如工厂、生成器、适配器、代理、策略模式耳熟能详。

- 由此而看到，做Android应用开发，不需要花太多精力去看Android系统源码，要先确保我上面罗列的20点所涉及的技术都掌握了。
