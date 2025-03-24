## 项目更新日志
- **Ver.1.3 Fixed 4**
    - 为 红米Note 7(lavender) 设备修改内核源码地址，同时修改了支持设备列表相关内容

- **Ver.1.3 Fixed 3**
    - 修正说明内容中排版错误的地方

- **Ver.1.3 Fixed 2**
    - 修正说明内容中的版本号部分

- **Ver.1.3 Fixed 1**
    - 增加了对补丁适用性的声明
    - 增加了用于KernelSU反向移植的补丁，并添加了对补丁的执行
    - 将更新发布Tag切换成1.3
    - 修正了示例文件中此前不完善的内容
    - 停止对KernelSU-Next的支持，当前维护设备至多维护2个版本后就会更换KernelSU分支，这项决策对自行Fork的用户不受影响，我们不会删除协助执行或判断KernelSU-Next分支的相关代码
    
- **Ver.1.3**
    - 修正了系统在应对仅Gcc编译时，无法如期切换至仅Gcc的问题
    - 增加了切换Ubuntu系统版本的相关变量和代码
    - 增加了切换Python2的相关变量和代码
    - 增加了解析Image文件包含的defconfig的功能
    - 增加了build debugger功能，该功能目前支持展示patch错误的文件
    - 切换一加8 nameless 15所需defconfig
