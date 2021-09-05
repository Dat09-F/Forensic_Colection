# Problem
Image information:

![alt text](https://github.com/Dat09-F/Forensic_Colection/blob/21e842f04cf4e48c8b62c43c11adb2339ee22d87/Misc_HPPD/Img_File/1.png)

And 1 link alphabetic https://notepad.pw/kcsc-hpbd-2021

Find the flag???

# Solution

* Flag_1: Trong thư chúng ta thấy các chữ có khoảng cách bất thường --> Mã morse
  
  Thay thế 1 space = space
           2 spcae = .
           3 space = -
  
  --> Truy cập https://www.dcode.fr/morse-code và decode khối mã vừa chuyển, ta thu được
  
  >KCSC(TH4NK_Y0U
  
 * Flag_2: Link https://notepad.pw/kcsc-hpbd-2021
   
   Truy cập link, ta thấy có định dạng hex ở đây, loại bỏ một vài ký tự thừa, ta được
   
   ![alt text](https://github.com/Dat09-F/Forensic_Colection/blob/21e842f04cf4e48c8b62c43c11adb2339ee22d87/Misc_HPPD/Img_File/2.png)
   
   Output cho ta thấy có 1 file rar chứa flag2.txt và password: 08082022
   
   --> Signatures của rar file start is 52 61 72 21 1A 07 00 and end is 77 56 51 03 05 04 00
   
   ![alt text](https://github.com/Dat09-F/Forensic_Colection/blob/21e842f04cf4e48c8b62c43c11adb2339ee22d87/Misc_HPPD/Img_File/3.png)
   
   --> Save output to file để xuât file rar và extract theo password đã biết ta được
   
   ![alt text](https://github.com/Dat09-F/Forensic_Colection/blob/21e842f04cf4e48c8b62c43c11adb2339ee22d87/Misc_HPPD/Img_File/5.png)
   
 * Flag_3: Trong thư có đề cập đến DinDonDon nên osint thông tin về member này https://kcsc-club.github.io/team-members/#media
 
   --> Ta nhận đc 1 mã
   
   ![alt text](https://github.com/Dat09-F/Forensic_Colection/blob/484a4043141a7de45554604eed3c8d5b4c67b1b6/Misc_HPPD/Img_File/6.png)
   
   --> Decode base58 
   
   ![alt text](https://github.com/Dat09-F/Forensic_Colection/blob/484a4043141a7de45554604eed3c8d5b4c67b1b6/Misc_HPPD/Img_File/7.png)


>Flag : KSCS(TH4NK_Y0U_F0R_ALL_&_G00D_H34LTH)
   
