### Layer1 solution:
1st step: check the filetype with the file command `file Flag.enc`
          it will show the filetype is openssl type.
          
2nd step: check the hints 1, the image combine we can guess that is `aes-256-cbc` encryption

3rd step: decrypt the file with the key by using the command bellow. but doing script kiddie was not a right way to solve, understand the AES encryption concept and the uses of the command will helps to understand better.
> command: `openssl enc -d -aes-256-cbc -in flag.enc -out file.txt -pass file:key.bin`

After the decryption, we will saw the WARNING, but just ignore the warning.
You will saw the file has decrypted in then .txt file.
Open the file content, we saw the fisrt 3 character written PDF.
So, just convert the .txt file into .pdf file and open it we will reach another layer.

### Layer2 solution: crypto + forensic

![image](https://user-images.githubusercontent.com/59368650/137344784-19ed7620-1016-49db-b57b-9e02b887e45c.png)

1st step: identify the file with binwalk command. Extract the file with command `binwalk -e file.pdf` and we will get all the extracting files.

2nd step: extract the zip file, inside contend 2 flag.txt, one is empty, other is inside the another zip file.

3rd step: we know that hints2 was mentioning "rockyou" term, that means we should brute force the ziip file.
          we can use JohnTheRipper tools to do bruteforce. 
          command:
          ```zip2john 9BA4.zip > hash
          john --wordlist=rockyou.txt hash
          ```
          After we brute force we open the file with the password we will get the flag. But so sorry in this chall we dont have flag inside and the prize has been given out to the 1st solver. HAHA
          
