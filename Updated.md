## 项目更新日志
- **Ver.1.3 Fixed 15**
    - 回滚 系统版本 设置

- **Ver.1.3 Fixed 14**
    - 增加 一加8 Realking OOS13.1 设备
    - 修改 BUILD_DEBUGGER 中 cat命令的输出

- **Ver.1.3 Fixed 13**
    - 调整 发布页面 和 支持列表 部分文字大小写
    - 将 发布Tag 版本号递增规则调整回来
    - 修复 SukiSU 版本号获取问题

- **Ver.1.3 Fixed 12**
    - 更改 发布标签 版本号为默认
    - 修正 VFS补丁 判定范围模糊的问题

- **Ver.1.3 Fixed 11**
    - 修复 红米 K20Pro 采用手动Hook时产生的编译错误
    - 修复 黑鲨 4 编译时无法找到新补丁的问题
    - 修复 一加8 Nameless 15 编译时提示重复定义的问题

- **Ver.1.3 Fixed 10**
    - 将 一加8 Nameless 15 切换为KernelSU-rsuntk
    - 将 红米 K20 Pro 切换为KernelSU-rsuntk
    - 将 黑鲨 4 切换为KernelSU-rsuntk
    - 将 小米 10S 切换为KernelSU-rsuntk

- **Ver.1.3 Fixed 9**
    - 增加说明页面中对切换KernelSU分支的内容
    - 更正分支mksu-skn的名称为SukiSU
    - 修正 支持列表 和 发布列表 中对 小米Mix2s 设备对KernelSU分支的描述

- **Ver.1.3 Fixed 8**
    - 修正 小米 Mix2s 对新补丁的执行
    - 修正发布用yaml存在的缺失

- **Ver.1.3 Fixed 7**
    - 去掉说明文件中版本号对小版本的显示
    - 尝试性的为 小米 Mix2s 进行KernelSU分支的迁移
    - 在发布列表中增加 一加Nameless 15 以及 三星 S20 5G（高通版），并将其在支持列表中更正为Beta

- **Ver.1.3 Fixed 6**
    - 为 三星 S20 5G（高通版） 修正yaml文件名称，并修改其所使用的KernelSU分支，和修改其对应的支持列表说明
    - 调整示例文件中，对新补丁执行的判定，以防止未按计划执行新补丁的情况
    - 调整了支持设备中部分设备说明

- **Ver.1.3 Fixed 5**
    - 修正示例文件中对新补丁的调用错误问题
    - 修改了支持列表中部分机型的解释说明

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
