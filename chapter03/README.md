
# 3 CUDA C 简介
## 3.1 本章目标
## 3.2 第一个程序
### 3.2.1 Hello, World!
```bash
nvcc hello_world.cu
```

运行结果
```bash
# linux
a.out

# windows
a.exe
```

### 3.2.2 核函数调用
```bash
nvcc simple_kernel.cu
```

### 3.2.3 传递参数
```bash
nvcc simple_kernel_params.cu
```

## 3.3 查询设备
```bash
nvcc enum_gpu.cu
```

输出结果：
```
   --- General Information for device 0 ---
Name:  NVIDIA GeForce GTX 1070
Compute capability:  6.1
Clock rate:  1695000
Device copy overlap:  Enabled
Kernel execution timeout :  Enabled
   --- Memory Information for device 0 ---
Total global mem:  -327680
Total constant Mem:  65536
Max mem pitch:  2147483647
Texture Alignment:  512
   --- MP Information for device 0 ---
Multiprocessor count:  16
Shared mem per mp:  49152
Registers per mp:  65536
Threads in warp:  32
Max threads per block:  1024
Max thread dimensions:  (1024, 1024, 64)
Max grid dimensions:  (2147483647, 65535, 65535)
```

## 3.4 设备属性的使用
```bash
nvcc set_gpu.cu
```

## 3.5 本章小结

