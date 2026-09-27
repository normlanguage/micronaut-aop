# Micronaut AOP 示例

[English](README.md) | [简体中文](README.zh-CN.md)

[环绕通知](sample/aop/Main.norm)是独立的消费者模块。`AuditInterceptor` 拦截 `AuditService.label()`，把实际观察结果从 `Norm` 改为 `AOP:Norm`。[示例模块](sample/aop/module.norm)声明依赖集合；[库模块](../micronaut/aop/module.norm)定义绑定的 AOP API。

在仓库根目录运行：

```sh
norm run samples/sample/aop/Main.norm
```

预期程序输出：`AOP:Norm`。Micronaut 也可能在标准错误输出中提示没有安装 SLF4J provider。
