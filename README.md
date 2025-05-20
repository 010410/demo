# Spring Boot Hello World 示例

## 前置条件

1. 安装 Java 17
2. 安装 Maven

## 项目简介

这是一个基于 Spring Boot 3.2.0 和 Spring Security 的示例项目，包含：
- 一个受保护的 `/hello` 接口，返回 "Hello World"
- 基于表单的用户名密码认证

## 默认账号密码
- 用户名：`test`
- 密码：`123456`

## 启动方式

1. 安装 Maven（可根据你的操作系统选择安装方式）：
   ```bash
   # 例如使用包管理器安装
   # macOS: brew install maven
   # Ubuntu: sudo apt-get install maven
   # Windows: 请参考 https://maven.apache.org/install.html
   ```

2. 在项目根目录下运行：
   ```bash
   mvn spring-boot:run
   ```

3. 访问接口：
   - 打开浏览器访问 http://localhost:8080/hello
   - 会自动跳转到登录页面
   - 输入上面的账号密码
   - 登录成功后即可看到 "Hello World" 信息

## 目录结构

- `pom.xml`：Maven 配置文件
- `src/main/java/com/example/demo/`
  - `DemoApplication.java`：主应用类
  - `config/SecurityConfig.java`：Spring Security 配置
  - `controller/HelloController.java`：Hello World 接口控制器