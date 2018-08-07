C是一门编译型语言(可以发布机械码)，Python是一门解释型语言(只能发布源代码)。  
Python的默认解释器是CPython，是用C语言开发的。  
在Windows系统上编写.py文件不要用记事本。  
ASCII是英文体系编码，Unicode把所有语言统一到一套编码里，不会有乱码问题，但英文文本占用空间变大。  
UTF-8编码把一个Unicode字符根据不同的数字大小编码成1-6个字节，常用英文字母被编码成1个字节，汉字通常是3个字节。  
在计算机内存中，统一使用Unicode编码，当需要保存到硬盘或者需要传输的时候，就转换为UTF-8编码。  
用记事本编辑的时候，从文件读取的UTF-8字符被转换为Unicode字符到内存里，编辑完成后，保存的时候再把Unicode转换为UTF-8保存到文件。  
Python3.x的字符串以Unicode编码，可以打印中文，而Python2.x不支持。  
由于Python源代码也是一个文本文件，当源代码中包含中文的时候，在保存源代码时，需声明# -*- coding: utf-8 -*-  