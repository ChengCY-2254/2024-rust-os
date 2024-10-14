```shell
qemu-system-riscv64\
	-machine virt\
	-nographic \
	-bios ../bootloader/rustsbi-qemu.bin \
	-device loader,file=target/riscv64gc-unknown-none-elf/release/os.bin,addr=0x8200000
```
- -nographic 表示无需图形界面，只需要字符流。
- bios 为rust的sbi
- loader参数和addr参数可以设置载入文件的路径以及将文件载入到qemu物理内存上的物理地址。
- 将二进制文件放到加载器中，并设置地址为0x8200000，这是sbi加载完毕后的调用路径。