Jupyter Notebook

一、默认工作路径配置

1.找到配置文件位置

在Anaconda Prompt中输入jupyter notebook –generate-config

2.打开配置文件

C:\Users\Administrator\.jupyter\jupyter_notebook.config.py

3.修改配置文件

```
将
# c.NotebookApp.notebook_dir = ''
修改为
c.NotebookApp.notebook_dir = 'F:\\jupyter'
```

4.找到jupyter nootbook的快捷图片，右键-》属性-》快捷方式-》目标

删除最后的“%USERPROFILE%/”

5.在cmd窗口输入jupyter notebook打开就是设置的工作路径了。