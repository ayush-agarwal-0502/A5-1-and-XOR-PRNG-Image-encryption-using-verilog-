# A5-1-and-XOR-PRNG-Image-encryption-using-verilog-
Image encryption using A5/1 and (XOR with PRNG) algorithms . I-CHIP22 PS2 solution 

## Introduction 

* Team name - ARcheus 
* Team members - Ayush Agarwal (me) , Raghavansh Singla 
* Skills : Verilog , Image Processing , Encryption (CyberSec) , Digital Electronics 
* Tools : Vivado , Icarus 

This repository contains our work on the problem statment for PS2 of I-CHIP 22 , the verilog event of UDYAM , which is the electronics department fest of IIT BHU .
We have encrypted an image using 2 different algorithms ( whose details have been split as Design 1 and Design 2 respectively ) . Image encryption is essential for secure transmission of image data over communication lines hence this project is valuable one . 

## The PS :

![image](https://user-images.githubusercontent.com/86561124/163959542-01705860-5c4f-4c09-8fec-f5fea4002c6a.png)
![image](https://user-images.githubusercontent.com/86561124/163959553-59914495-995e-443c-80cf-8cca6c38d0ce.png)
![image](https://user-images.githubusercontent.com/86561124/163959563-f59af497-5920-4575-9e2a-0a8e28e72b74.png)
![image](https://user-images.githubusercontent.com/86561124/163959599-6130c29a-0aae-4b8a-8c3a-cea4891e7dab.png)
![image](https://user-images.githubusercontent.com/86561124/163959621-ac87ac3c-7d95-4b7c-8ac1-bf8082ae6b4c.png)
![image](https://user-images.githubusercontent.com/86561124/163959633-02400e66-61a8-431b-a0e7-6f54af66748e.png)

## Design 1 details :

Bits were generated using a Pseudo Random Number Generator (PRNG) ( Module for the same has been made and uploaded in the repo ) , and then XORed with the bits of the image . This process is the encryption part . For the decryption part we run the PRNG again and again XOR the same bits . This process decrypts the image since XORing the same number 2 times removes its effect on the original data bit . 

Actual Image :

![image](https://user-images.githubusercontent.com/86561124/163985959-46dfd64c-3c9d-49c6-b097-03a13485eebe.png)

Encrypted Image :

![image](https://user-images.githubusercontent.com/86561124/163986081-eed920fb-38d4-450b-8c74-aa9982bc454a.png)

Decrypted Image :

![image](https://user-images.githubusercontent.com/86561124/163986127-df3e02f5-ae36-4f1f-b4d4-14312a043de5.png)

### Module for PRNG :

Felt important to show hence added the images here , the rest of the code can be referred from the verilog files in this repository . The PRNG can be made by shifting all the values by one bit , and filling the vacant space by xor of combination of few selected bits . 

![image](https://user-images.githubusercontent.com/86561124/163986831-685a00ef-0161-4026-a369-9b78d4084eda.png)

![image](https://user-images.githubusercontent.com/86561124/163986839-a5ea2723-3fcf-44f5-92fc-274c095a2ef6.png)




