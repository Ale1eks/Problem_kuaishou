# BUG & FIX

## 2021.6.15 IDEA MAVEN 崩溃问题

###  问题描述：MAVEN 崩溃，在IDEA当中无法打开，并且一直报错：

```
     org.jetbrains.idea.maven.server.MavenServerConnectorImpl$StartServerTask.run(MavenServerConnectorImpl.java:247)

at com.intellij.execution.rmi.RemoteProcessSupport.acquire(RemoteProcessSupport.java:177)

```

>  IDEA 本身编辑器的问题，但是容易被忽略
   1.在 Applications 目录当中删除 IDEA
   2.在一下两个目录当中删除 IDEA 缓存以及备份数据
```
~/Library/Application Support/JetBrains/IntelliJIdea2021.1
~/Library/Caches/JetBrains/IntelliJIdea2021.1
```
   3.在项目文件当中删除（重要）