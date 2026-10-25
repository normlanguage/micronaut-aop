# micronaut.aop Skill

Use this skill to work with Norm module `micronaut.aop` version 5. Use only declarations listed below.

## `micronaut.aop`

### `Around`

```norm
annotation Around implements TypeTarget, FunctionTarget, RuntimeRetention
```

#### `cacheableLazyTarget`

```norm
Boolean cacheableLazyTarget
```

#### `hotswap`

```norm
Boolean hotswap
```

#### `lazy`

```norm
Boolean lazy
```

#### `proxyTarget`

```norm
Boolean proxyTarget
```

#### `proxyTargetMode`

```norm
AroundProxyTargetConstructorMode proxyTargetMode
```

#### `Around`

```norm
Around(Boolean? cacheableLazyTarget, Boolean? hotswap, Boolean? lazy, Boolean? proxyTarget, AroundProxyTargetConstructorMode? proxyTargetMode)
```

## `micronaut.aop`

### `AroundProxyTargetConstructorMode`

```norm
enum AroundProxyTargetConstructorMode
```

#### `ALLOW`

```norm
ALLOW
```

#### `ERROR`

```norm
ERROR
```

#### `WARN`

```norm
WARN
```

## `micronaut.aop`

### `InterceptorBean`

```norm
annotation InterceptorBean implements TypeTarget, FunctionTarget, RuntimeRetention
```

#### `value`

```norm
List<Class<?>> value
```

## `micronaut.aop`

### `InvocationContext`

```norm
interface InvocationContext<T, R> extends Executable<T, R>, AnnotationMetadataDelegate, MutableAttributeHolder
```

#### `proceed`

```norm
R? proceed()
```

## `micronaut.aop`

### `MethodInterceptor`

```norm
interface MethodInterceptor<T, R> extends Interceptor<T, R>
```

#### `intercept`

```norm
R? intercept(MethodInvocationContext<T, R>? arg0)
```

## `micronaut.aop`

### `MethodInvocationContext`

```norm
interface MethodInvocationContext<T, R> extends InvocationContext<T, R>, Executable<T, R>, ExecutableMethod<T, R>
```

