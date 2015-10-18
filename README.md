
关于example-dubbo示例<br>

执行 mvn install, maven会自动将source install到repository. <br>
执行 mvn deploy, maven会自动将source deploy到remote-repository. <br>
执行 mvn source:jar, 单独打包源码. <br>

1. 2015-10-15(周四)，构建example-dubbo工程.<br>

测试方法:<br>
1). 修改配置文件resources/dubbo-consumer.xml、resources/dubbo-provider.xml <br>
    主要配置zookeeper地址：<dubbo:registry address="zookeeper://w22.node:2181" /> <br>
2). 启动服务.   ServerProvider.main() <br>
3). 客户端调用.  ClientConsumer.main() <br>

