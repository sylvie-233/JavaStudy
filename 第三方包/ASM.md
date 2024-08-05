# ASM


## 基础介绍

一个操作字节码的库

asm-core、asm-tree

core基于visitor模式、tree基于node模式

核心功能：
- 删除方法
- 增加方法
- 修改方法


## 核心内容

```yaml
org.objectweb.asm:
    commons:
        AdviceAdapter:
            onMethodEnter():
            onMethodExit():
    AbstarctInsnNode:
    Attribute:
    ClassNode:
        methods:
    ClassReader: 读取字节码
        accept():
    ClassVisitor:
        visit():
        visitEnd():
        visitField():
        visitMethod():
    ClassWriter: 修改字节码
    FieldVisitor:
        visitAnnotaion():
        visitAttribute():
        visitEnd():
    MethodInsnNode:
        instructions:
        name:
        owner:
    MethodVisistor:
        visitAnnotaion():
        visitAttribute():
        visitCode():
        visitEnd():
        visitFieldInsn(): 字段入栈
        visitInsn(): 指令入栈
        visitLdcInsn(): 常量入栈
        visitMaxs():
        visitMethodInsn(): 方法入栈
        visitVarInsn(): 变量入栈
```