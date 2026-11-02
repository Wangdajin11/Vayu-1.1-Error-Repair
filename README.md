# Vayu-1.1-Error-Repair
记录 VaYu（Vayu 1.1）在 Windows 上双击打不开的完整排查与修复过程。现象为程序启动即退出，报错 0xC000007B（STATUS_INVALID_IMAGE_FORMAT）；根因是系统缺少 Microsoft Visual C++ 2013 Redistributable (x64) 运行库（msvcr120.dll / msvcp120.dll 缺失，且安装包自带的为 32 位版本，位宽不匹配）。修复方法：从微软官方下载 vc_redist.x64.exe（选 x64 版本）安装即可，支持静默安装。文档含排查流程图，简洁图文并茂。
