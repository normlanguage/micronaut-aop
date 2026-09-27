# Micronaut AOP samples

[English](README.md) | [简体中文](README.zh-CN.md)

[Around advice](sample/aop/Main.norm) is an independent consumer module. `AuditInterceptor` intercepts `AuditService.label()` and changes the observed result from `Norm` to `AOP:Norm`. The [sample module](sample/aop/module.norm) declares its dependency set; the [library module](../micronaut/aop/module.norm) defines the bound AOP API.

From the repository root, run:

```sh
norm run samples/sample/aop/Main.norm
```

Expected program output: `AOP:Norm`. Micronaut may also warn on stderr that no SLF4J provider is installed.
