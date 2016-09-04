# Try maven with multiple modules

- 使用 maven-source-plugin 控制打包时一并打包源码
- 使用 properties-maven-plugin 读取属性文件、写入所有项目属性到文件, 但读取的属性不能用来配置 dependencyManagement 的 version 值
- 用 bom 使 m2 模块依赖 m1 模块时, 不需要配置 m1 模块的 version 属性值
- 设置属性 project.build.sourceEncoding=UTF-8 控制源码编码为 UTF-8
- 设置属性 maven.compiler.source|target=1.8 控制使用的 jdk 版本