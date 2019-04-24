# JavaSE JavaEE JavaMe区别
## JavaSE    Java Platform，Standard Edition
* JavaSE，标准版，主要用于开发和部署桌面、服务器以及嵌入设备和实时环境中的Java应用程序。例如，Java应用程序开发平台Eclipse。
* JavaSE即Java标准版，它是JavaEE和JavaME的基础，之前称为J2SE，用来开发C/S架构软件，通俗来讲，即开发电脑桌面应用软件，电脑上运行的软件，例如，Java应用程序开发平台Eclipse。
## JavaEE    Java Platform，Enterprise Edition
* JavaEE，企业版，主要针对企业应用的开发。例如，电子商务网站、ERP系统。
* JavaEE即企业版，之前称为 J2EE，JavaEE是在JavaSE的基础上构建的，用来开发B/S架构软件，即开发企业级应用，例如，电子商务网站、ERP系统。
* JavaEE在JavaSE的基础进行了扩展，增加了一些更加便捷的应用框架。比如我们现在常用的Java开发三大框架Spring、Struts和Hibernate，我们可以应用这些框架轻松写出企业级的应用软件。
* Java EE 是在 Java SE 的基础上构建的，它提供 Web 服务、组件模型、管理和通信 API，可以用来实现企业级的面向服务体系结构（service-oriented architecture，SOA）和 Web 2.0 应用程序。
* Java EE也可以说是一个框架也是一种规范，说它是框架是因为它包含了很多我们开发时用到的组件，例如：Servlet，EJB，JSP，JSTL等；说它是规范因为我们开发web应用常会用到的一些规范模式，JavaEE提供了很多规范的接口却不实现，将这些接口的具体实现细节转移到厂商身上，这样各家厂商推出的JavaEE产品虽然名称实现不同，但展现给外部使用的却是统一规范的接口。例如，我们编写的JSP代码中，由于大量的显示代码和业务逻辑混淆在一起，彼此嵌套，不利于程序的维护和扩展。当业务需求发生变化的时候，对于程序员和美工都是一个很重的负担。为了程序的易维护性和可扩展性，这就需要我们使用JavaEE技术来进行项目开发。
## JavaMe   Java Platform，Micro Edition 
* JavaME，微型版，主要针对消费类电子设备的。例如，蜂窝电话和可视电话、数字机顶盒、汽车导航系统等等。
* JavaME即微型版，也是以Java为基础的，之前称为 J2ME，它是一套运行专门为嵌入式设备设计的api接口规范，主要用于开发移动设备软件和嵌入式设备软件，例如：手机游戏，电视机顶盒和打印机相关的嵌入式设备软件。
* 简单来说，JavaSE是Java的基础，主要针对桌面程序开发；JavaEE是针对企业级应用开发；而JavaME是主要针对嵌入式设备软件开发。