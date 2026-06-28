# 前言

随着社会老龄化程度的加深，社区养老服务成为越来越重要的社会需求。"weixin438-spring boot社区养老保障系统小程序"旨在为社区养老提供便捷、高效的服务平台，通过信息化手段提高养老服务的管理水平，实现智慧养老。

# 内容介绍

本项目是一款基于微信小程序的社区养老保障系统，主要功能包括老人信息管理、服务人员管理、养老服务预约、健康数据监测等。通过本系统，可以方便社区管理人员及时了解老人生活状况，为老人提供及时的帮助和关怀。

# 技术介绍

## 语言：Java

## 使用框架：Spring Boot、Spring MVC，MyBatis

## 前端技术：JS、Vue、CSS3，Uniapp

## 开发工具：IDEA/Eclipse，Uniapp

## 数据库：MySQL 5.7/8.0

## 数据库管理工具：phpstudy/Navicat

## JDK版本：jdk1.8

## Maven：apache-maven 3.8.1-bin

## 前端环境：Node.Js 12\14\16

# 核心代码

以下为老人信息管理的核心代码：

```java
// 老人信息控制器
@RestController
@RequestMapping("/elder")
public class ElderController {

    @Autowired
    private ElderService elderService;

    // 查询老人信息
    @GetMapping("/list")
    public ResponseEntity<List<Elder>> list() {
        List<Elder> elders = elderService.list();
        return ResponseEntity.ok(elders);
    }

    // 新增老人信息
    @PostMapping("/add")
    public ResponseEntity<Void> add(@RequestBody Elder elder) {
        elderService.add(elder);
        return ResponseEntity.ok().build();
    }

    // 更新老人信息
    @PutMapping("/update")
    public ResponseEntity<Void> update(@RequestBody Elder elder) {
        elderService.update(elder);
        return ResponseEntity.ok().build();
    }

    // 删除老人信息
    @DeleteMapping("/delete/{id}")
    public ResponseEntity<Void> delete(@PathVariable("id") Integer id) {
        elderService.delete(id);
        return ResponseEntity.ok().build();
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图
