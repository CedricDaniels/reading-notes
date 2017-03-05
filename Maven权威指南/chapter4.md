1. 普通java项目配置加载log4j配置

``` java
PropertyConfigurator.configure(Main.class.getClassLoader().getResource("log4j.properties"));
```
2. `URLconnection` 和 `HttpURLconnection` 也可以发送网络请求
3. 可以使用 Velocity 模板定制控制台输出
4. mvn install -X 可以进行详细的依赖追踪， mvn dependency:tree 可以查看依赖树，mvn dependency:resolve 查看最终依赖
5. Apache Commons IO 可以摆脱繁琐的IO操作
6. 设置 maven-surefire-plugin 的testFailureIgnore 为true可以在测试失败时，继续构建项目
7. maven-assembly-plugin 的 jar-with-dependencies 可以构建有完整依赖的程序，我们还可以自定义该插件的自定义装配描述符 