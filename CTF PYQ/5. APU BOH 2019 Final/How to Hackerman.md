> flag format: apuboh2019{}

The flag is hidden top header and is invisivle, so we need change the color of the text.

![image](https://user-images.githubusercontent.com/59368650/138410828-5cd0da77-f3ef-48cb-9c92-31d9e0770d4c.png)

So, we get an encoded/encrypted cipher.
probably, I did not know what it is so we put it into cyberchef.
If the cyberchef couldn't detect it, then it probably is MD5/SHA hashing.

![image](https://user-images.githubusercontent.com/59368650/138411199-04fb3403-60e8-45d8-b373-1cb2795b3a2c.png)

so, after we decrypted it using crackstation site cracking tools. we got the first part of the flag.

![image](https://user-images.githubusercontent.com/59368650/138411562-b06ed548-6ae7-4b44-99b0-f1e1851a6e08.png)

then we also check on footer.

![image](https://user-images.githubusercontent.com/59368650/138411915-5365bf68-b9c2-49af-a1fb-c5f19a902b3d.png)

place it to cyberchef, try all possible base.

![image](https://user-images.githubusercontent.com/59368650/138412396-7aaefe87-daf9-4a97-865e-20f51507bfc1.png)

we also can check for hidden content by clicking the paragraph button.
then, we also can see there is another encrypt hash. From here I know that I have no patient for this chall😫 to guess all possible flag!too stressy ..sorry, lets continue.

![image](https://user-images.githubusercontent.com/59368650/138412929-8344b177-3fd2-48c5-91f4-18d27e7c51e0.png)
![image](https://user-images.githubusercontent.com/59368650/138413623-b0e30844-1828-43a9-8ebc-94fc4c58adee.png)

next, uncrop 2 image.

![image](https://user-images.githubusercontent.com/59368650/138413826-cb5acea3-c94e-4914-8c60-261c24caf128.png)
![image](https://user-images.githubusercontent.com/59368650/138413953-2bf6b246-2c29-4561-a634-085deee06aa2.png)

lazy people can use [OCR](https://www.onlineocr.net/) tools to extract the text from the image.
then decode it using cyberchef which we know that it is base64, if you dont know can use the magic pen ![image](https://user-images.githubusercontent.com/59368650/138414611-2d4915f3-c9f0-4b01-b0f5-39cb9d666640.png)

next part,
![image](https://user-images.githubusercontent.com/59368650/138414973-56601de9-3c23-43d2-954e-ab7ce3f6b475.png)

last part,
```
reference > manage source > follow the red arrow
```
it is an encoded url,decode it using cyberchef with urldecode we get last part of the flag.

![image](https://user-images.githubusercontent.com/59368650/138415454-ab0c6d8a-27c9-4529-9140-74ffd902bc97.png)

I know person who did this writeup probably have no passion anymore, no doubt as me.😞
N0TE that sometimes, the flag might be grammar mistake, we need to change it by ourself. hv fun
```
flag: apuboh2019{s1mp1c1ty_13t_k3y_s0m3t1m3s} 
```

