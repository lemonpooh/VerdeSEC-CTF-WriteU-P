# Innocent

This is pcap file. We need to open this file with `Wireshark` packet capture software.
To find the flag, search the HTTP protocol from the wireshark.

![image](https://user-images.githubusercontent.com/59368650/138399367-a291b3b8-da29-4237-bf83-912749d6f154.png)

Then, go to 
> **file** > **export object** > **HTTP** > **save all** 

From one of the file, we can see the encoded message.
copy this encoded msg to [cyberchef](https://gchq.github.io/CyberChef/) and decode it with base64 and we will get the flag.
![image](https://user-images.githubusercontent.com/59368650/138399986-64c3abb1-3f44-4494-bad6-258766dbbf86.png)
