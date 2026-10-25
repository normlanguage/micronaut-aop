# micronaut.aop Skill

Use this skill to work with Norm module `micronaut.aop` version 7. Use only declarations listed below.

## `micronaut.aop`

Source: `Around.norm`

### `Around`

```norm
annotation Around implements TypeTarget, FunctionTarget, RuntimeRetention
```

#### `cacheableLazyTarget`

```norm
Boolean cacheableLazyTarget
```

Type: `Boolean`

#### `hotswap`

```norm
Boolean hotswap
```

Type: `Boolean`

#### `lazy`

```norm
Boolean lazy
```

Type: `Boolean`

#### `proxyTarget`

```norm
Boolean proxyTarget
```

Type: `Boolean`

#### `proxyTargetMode`

```norm
AroundProxyTargetConstructorMode proxyTargetMode
```

Type: `AroundProxyTargetConstructorMode`

#### `Around`

```norm
Around(Boolean? cacheableLazyTarget, Boolean? hotswap, Boolean? lazy, Boolean? proxyTarget, AroundProxyTargetConstructorMode? proxyTargetMode)
```

Parameters:

- `cacheableLazyTarget`: `Boolean?`
- `hotswap`: `Boolean?`
- `lazy`: `Boolean?`
- `proxyTarget`: `Boolean?`
- `proxyTargetMode`: `AroundProxyTargetConstructorMode?`

## `micronaut.aop`

Source: `AroundProxyTargetConstructorMode.norm`

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

Source: `Interceptor.norm`

### `Interceptor`

```norm
interface Interceptor<T, R> extends Ordered
```

Type parameters:

- `T`
- `R`

## `micronaut.aop`

Source: `InterceptorBean.norm`

### `InterceptorBean`

```norm
annotation InterceptorBean implements TypeTarget, FunctionTarget, RuntimeRetention
```

#### `value`

```norm
List<Class<?>> value
```

Type: `List<Class<?>>`

## `micronaut.aop`

Source: `InvocationContext.norm`

### `InvocationContext`

```norm
interface InvocationContext<T, R> extends Executable<T, R>, AnnotationMetadataDelegate, MutableAttributeHolder
```

Type parameters:

- `T`
- `R`

#### `proceed`

```norm
R? proceed()
```

Returns: `R?`

## `micronaut.aop`

Source: `JavaArrays.norm`

### `JavaClassArray`

```norm
class JavaClassArray
```

#### `JavaClassArray`

```norm
JavaClassArray(JavaClassArrayBindingToken token)
```

Parameters:

- `token`: `JavaClassArrayBindingToken`

#### `size`

```norm
Integer size()
```

Returns: `Integer`

#### `get`

```norm
Class<?>? get(Integer index)
```

Parameters:

- `index`: `Integer`

Returns: `Class<?>?`

#### `set`

```norm
Void set(Integer index, Class<?>? value)
```

Parameters:

- `index`: `Integer`
- `value`: `Class<?>?`

Returns: `Void`

### `javaClassArrayNew`

```norm
JavaClassArray javaClassArrayNew(Integer size)
```

Parameters:

- `size`: `Integer`

Returns: `JavaClassArray`

## `micronaut.aop`

Source: `MethodInterceptor.norm`

### `MethodInterceptor`

```norm
interface MethodInterceptor<T, R> extends Interceptor<T, R>
```

Type parameters:

- `T`
- `R`

#### `intercept`

```norm
R? intercept(MethodInvocationContext<T, R>? arg0)
```

Parameters:

- `arg0`: `MethodInvocationContext<T, R>?`

Returns: `R?`

## `micronaut.aop`

Source: `MethodInvocationContext.norm`

### `MethodInvocationContext`

```norm
interface MethodInvocationContext<T, R> extends InvocationContext<T, R>, Executable<T, R>, ExecutableMethod<T, R>
```

Type parameters:

- `T`
- `R`

## `micronaut.aop.io.micronaut.core.annotation`

Source: `io/micronaut/core/annotation/AnnotatedElement.norm`

### `AnnotatedElement`

```norm
interface AnnotatedElement extends AnnotationMetadataProvider, Named
```

## `micronaut.aop.io.micronaut.core.annotation`

Source: `io/micronaut/core/annotation/AnnotationMetadata.norm`

### `AnnotationMetadata`

```norm
interface AnnotationMetadata extends AnnotationSource
```

## `micronaut.aop.io.micronaut.core.annotation`

Source: `io/micronaut/core/annotation/AnnotationMetadataDelegate.norm`

### `AnnotationMetadataDelegate`

```norm
interface AnnotationMetadataDelegate extends AnnotationMetadataProvider, AnnotationMetadata
```

## `micronaut.aop.io.micronaut.core.annotation`

Source: `io/micronaut/core/annotation/AnnotationMetadataProvider.norm`

### `AnnotationMetadataProvider`

```norm
interface AnnotationMetadataProvider extends AnnotationSource
```

## `micronaut.aop.io.micronaut.core.annotation`

Source: `io/micronaut/core/annotation/AnnotationSource.norm`

### `AnnotationSource`

```norm
interface AnnotationSource
```

## `micronaut.aop.io.micronaut.core.attr`

Source: `io/micronaut/core/attr/AttributeHolder.norm`

### `AttributeHolder`

```norm
interface AttributeHolder
```

## `micronaut.aop.io.micronaut.core.attr`

Source: `io/micronaut/core/attr/MutableAttributeHolder.norm`

### `MutableAttributeHolder`

```norm
interface MutableAttributeHolder extends AttributeHolder
```

## `micronaut.aop.io.micronaut.core.naming`

Source: `io/micronaut/core/naming/Described.norm`

### `Described`

```norm
interface Described
```

## `micronaut.aop.io.micronaut.core.naming`

Source: `io/micronaut/core/naming/Named.norm`

### `Named`

```norm
interface Named
```

## `micronaut.aop.io.micronaut.core.order`

Source: `io/micronaut/core/order/Ordered.norm`

### `Ordered`

```norm
interface Ordered
```

## `micronaut.aop.io.micronaut.core.type`

Source: `io/micronaut/core/type/Executable.norm`

### `Executable`

```norm
interface Executable<T, R> extends AnnotationMetadataProvider
```

Type parameters:

- `T`
- `R`

## `micronaut.aop.io.micronaut.inject`

Source: `io/micronaut/inject/ExecutableMethod.norm`

### `ExecutableMethod`

```norm
interface ExecutableMethod<T, R> extends Executable<T, R>, MethodReference<T, R>, Described
```

Type parameters:

- `T`
- `R`

## `micronaut.aop.io.micronaut.inject`

Source: `io/micronaut/inject/MethodReference.norm`

### `MethodReference`

```norm
interface MethodReference<T, R> extends AnnotationMetadataDelegate, AnnotatedElement
```

Type parameters:

- `T`
- `R`

