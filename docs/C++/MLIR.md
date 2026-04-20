# MLIR相关

## Attr和Enum

Attr是IR里的对象，Enum只是值域。

较老的MLIR中的相关实现，使用IntEnumAttr/BitEnumAttr，I32EnumAttr同时包含了`Enum信息`和`attribute旧式存储描述`两种角色

在更新的版本当中，推荐使用`EnumAttr`包一个`EnumInfo`，更加层次化。

