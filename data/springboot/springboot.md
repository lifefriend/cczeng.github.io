本机环境： java JDK8

## 1、下载  spring-tool-suite

```html
https://spring.io/tools3/sts/legacy
```

![1552295132933](./1.png)

## 2、解压运行

```shell
sts-bundle\sts-3.9.7.RELEASE\STS.exe
```

![1552295132933](./2.jpg)

## 3、新建工程

打开 Dashboard,点击 CREATE SPRING STARTER PROJECT

![1552295132933](./3.jpg)



进入 New Spring Starter Project,设置项目名称(Name)、项目 maven 坐标(Group、Artifact),点击 Next

![1552295132933](./5.jpg)



进入 New Spring Starter Project Dependencies,选择项目依赖 jar 包

![1552295132933](./8.jpg)



点击 Finish,进入项目

![1552295132933](./9.jpg)

## 4、Hello World

新建 HelloWorld.java，输入如下代码：

```java
package com.example.demo;

import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class HelloWorld {

	@RequestMapping("/")
	public String Hello() {
		return "Hello World！";
	}
	
}
```
![1552295132933](./11.jpg)

## 5、运行

选中 DemoApplication.java，右键 Run As -> Spring Boot App
![1552295132933](./12.jpg)

浏览器输入：http://localhost:8080/
![1552295132933](./13.jpg)

完