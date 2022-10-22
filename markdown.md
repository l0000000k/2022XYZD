# C语言

 ## 1.java

 ```java
 package myjava;
 
 import java.io.BufferedInputStream;
 import java.io.BufferedOutputStream;
 import java.io.DataInputStream;
 import java.io.DataOutputStream;
 import java.io.File;
 import java.io.FileInputStream;
 import java.io.FileOutputStream;
 import java.io.IOException;
 import java.util.Date;
 
 public class FileCopy {
     private static void fileData(File f) {
             System.out.println("Absolute path: " + f.getAbsolutePath()
                   + "\n Can read: " + f.canRead() + "\n Can write: " + f.canWrite()
                   + "\n getName: " + f.getName() + "\n getParent: " + f.getParent() 
                   + "\n getPath: " + f.getPath() + "\n length: " + f.length()
                   + "\n lastModified: " + new Date(f.lastModified()));
             if (f.isFile())  System.out.println("It's a file");
             else    System.out.println("It's a directory");
     }
     public static void main(String[] args) {
             File old = new File("D:\\FileCopy.txt");
             File rname = new File("D:\\ffileCopy.txt");
             System.out.println("The original file's information: ");
             fileData(old);
             old.renameTo(rname);
             System.out.println("\n The file information after rename: ");
             fileData(rname);
             if (!old.exists()) 
                   System.out.println("\n The original file never exists");
     }
 }
 
 ```

## 2.插入表格

| 项目 | 男生 | 女生 |
| ---- | ---- | ---- |
|      |      |      |
|      |      |      |
|      |      |      |

## 3.图片

### 1）我的照片



![我的照片](https://img2.pconline.com.cn/pconline/0710/07/1121416_071010Daniel12.jpg)