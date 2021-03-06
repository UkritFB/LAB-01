#HSLIDE
# ใบงานที่ 1 เรื่อง การเขียนโปรแกรม Win32 ด้วยภาษา C

#HSLIDE
##วัตถุประสงค์

1. เพื่อให้นักศึกษาสามารถบอกวิธีการเขียนโปรแกรมบน Windows ด้วยฟังก์ชัน Win32 API ได้
2. เพื่อให้นักศึกษาสามารถใช้เครื่องมือต่างๆ ในการสร้าง Application บน IDE ได้

#HSLIDE
##ลำดับการทดลอง

#VSLIDE
1. เรียกโปรแกรม Microsoft Visual Studio 
#VSLIDE
2. สร้าง Project ใหม่  โดยเลือกเมนู File >> New >> Project… (Ctrl+Shift+N) จะปรากฏหน้าต่าง New Project ดังรูปที่ 1 ให้ทำตามขั้นตอน 2.1 – 2.4
![](https://github.com/Desktop-Programming-Lab-2559/LAB-01/blob/master/imgs/pic1.png)
    2.1 ช่อง Templates: ให้เลือก Visual C++ และเลือกชนิด project เป็น Empty Project

    2.2 ช่อง Name: ให้ใส่ชื่อของ Project เป็น EasyWin32

    2.3 ช่อง Location: ให้เลือกตำแหน่งที่จะสร้าง Project

    2.4 ส่วนที่เหลือ ให้คงไว้ตามที่ปรากฏ กด OK 

#VSLIDE
3 เพิ่ม source code ให้กับ project โดยการเลือกเมนู PROJECT >> Add New Item…
   
    3.1 ตั้งชื่อไฟล์เป็น EasyMain.cpp
    3.2 กด Add เพื่อเพิ่มไฟล์


#VSLIDE
4 พิมพ์โปรแกรมดังต่อไปนี้ลงในไฟล์ EasyMain.cpp
 
```c 
#include <windows.h>
int WINAPI
WinMain(HINSTANCE hInst, HINSTANCE hPrev, LPSTR  lpCmdLine, int nCmdshow)
{
	MessageBox(NULL, "Hello World! This is my first win32 program!",
		"Lesson1", MB_OK);
	return 0;
}
```

#VSLIDE
**หมายเหตุ**
ใน Windows นั้น ฟังก์ชันแรกในโปรแกรมของเราที่จะถูกเรียกใช้คือ WinMain ต่างจากในภาษา C ที่ใช้ main()<br>
อ่านเพิ่มเติม [WinMain entry point](https://msdn.microsoft.com/en-us/library/windows/desktop/ms633559(v=vs.85).aspx)

5 กดปุ่ม Ctrl+F5 เพื่อดูผลการทำงานของโปรแกรม

#HSLIDE
## บันทึกผลการทดลอง

 [ให้สรุปผลการทดลอง แล้ว commit changes จากนั้นให้ส่งไปที่ edmodo]

#HSLIDE
## คำถาม 
1. นักศึกษาพบปัญหาในการคอมไพล์โปรแกรมหรือไม่ ถ้าเจอให้บอกที่ผิดและแนวทางการแก้ไข





#HSLIDE
##[อ้างอิง](https://github.com/Desktop-Programming-Lab-2559/LAB-01/wiki/References)
WinMain (..), MessageBox(..) 
 
