# vscode-comment
Adds simple jsdoc comments for the parameters of a selected function signature

## Using
In a typescript or javascript  file, select a function signature, ideally one that contains one or more parameters. Select the whole function signature then invoke the Add Doc Comments extension (open the command palette (F1 on Windows) and look for the command 'Add doc comments'. Hit enter.)

## 使用

在该插件中，你可以通过点击鼠标右键，在参数名称上添加注释。或者在编辑器的右上角/Mac的touchBar上点击 💫 图标，就可以直接生成注释。不用再cmd shift p，执行命令,方便很多。

## 说明

该插件fork自 https://github.com/microsoft/vscode-comment。自用。
更新项:
- 支持多种启动方式
- 支持ts/js/vue项目
- 图标更新

![install and work](images/addDocComments.gif)


The extension will parse the selected signature and add @param and @return tags for each parameter and any return type in the selected signature, directly above the signature.

## Limitations
The extension does not support any other type of jsdoc tags. It only calculates @param and @return

Parameter types are not inferred based on usage. If a type is not specified, empty braces {} are returned.
