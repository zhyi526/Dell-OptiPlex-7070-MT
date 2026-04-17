# Dell-OptiPlex-7070-MT
Dell OptiPlex 7070 MT(台式机) Hackintosh EFI configuration

BIOS设置
常规→高级启动选项：取消选中
系统配置→SATA操作：AHCI
安全启动→安全启动启用：禁用
英特尔®Software Guard Extensions™→英特尔®SGX™启用：禁用
电源管理→阻止睡眠：检查
虚拟化支持→用于直接I / O的VT：取消选中

通过GRUB进行BIOS设置（可选）
将预分配的DVMT设置为64M： setup_var 0x8DC 0x02
禁用CFG锁定： setup_var 0x5BE 0x00
