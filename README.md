# Non-GKI Kernel with KSU and SUSFS
Automatic build Non-GKI Kernel with KSU and SUSFS
由于Non-GKI内核存在严重的碎片化，不仅仅体现在内核无法通用，更是存在编译环境参差不齐，包括但不限于系统版本，GCC版本，Clang版本等等，因此决定开始自动化编译Non-GKI内核项目
本项目欢迎Fork后自行编辑使用，也欢迎增加修改后提交合并，或者成为合作伙伴

# 使用例
## Profiles/设备名称_ROM名称.env
总共由以下内容组成：
CONFIG_ENV - 用来表明在Action环境中具体配置文件位置
DEVICE_NAME - 设备全程，格式：设备品牌_型号_地区
DEVICE_CODENAME - 设备代号
CUSTOM_CMDS - 通常用于指明所用编译器/备用编译器
EXTRA_CMDS - 通常用于编译器所需的自定义参数
KERNEL_SOURCE - 内核源码所在之处
KERNEL_BRANCH - 内核源码所需分支
CLANG_SOURCE - Clang所在之处，但支持git、tar.gz、tar.xz
CLANG_BRANCH - Clang所需分支，但前提是git
GCC_XX_SOURCE - GCC所在之处，但支持git、tar.gz、zip
GCC_XX_BRANCH - GCC所需分支，但前提是git
DEFCONFIG_SOURCE - 若有自定义DEFCONFIG文件需求可提供具体文件所在地址
DEFCONFIG_NAME - 不管是否自定义，都需要提供用于编译的必要DEFCONFIG文件，通常格式为：设备_defconfig、vendor/设备_defconfig
SUSFS_ENABLE - 是否在编译时启用SUSFS，true或false
SUSFS_FIXED - 是否启用SUSFS错误修补，一般用于内核修补时产生错误后，二次补充修补
AK3_SOURCE - Anykernel3所在之处，若需要的话，仅支持git
AK3_BRANCH - Anykernel3所需分支
ROM_TEXT - 用于编译成功后用于上传文件标题，声明内核可用的ROM

## .github/workflow/build_kernel_设备简称型号_ROM.yml
这里仅指出大概可供修改的地方，具体可按需求修改
runs-on: ubuntu-XX.XX - 不同内核所需系统不同，默认为22.04
Extra Kernel Options - 有些内核编译时需要提供更多设置项
