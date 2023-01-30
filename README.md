# knightctf_writeup
url: https://2023.knightctf.com/

**Network**

-----------------------------------------------

- hello

![image](https://user-images.githubusercontent.com/121002781/215470437-fb95af61-0a5c-47da-a9bb-ad39625dd1e1.png)

In the text the word Sir vignere may be a encryption vigenère, hypothetically.

![image](https://user-images.githubusercontent.com/121002781/215470919-6ee3a4ab-809a-4a66-bc5c-e5d2b99b7123.png)

The udp protocol is very suspicious, I will choose it.

I will watch the UDP stream.

![image](https://user-images.githubusercontent.com/121002781/215471634-6d22c54d-be0c-45ab-9b22-d0cbf1b040f7.png)

stream 12

I  found a message encrypt.

![image](https://user-images.githubusercontent.com/121002781/215472380-cbd67575-1996-4050-a363-53eb62a9c3ba.png)

Looks like 1 step is missing.

![image](https://user-images.githubusercontent.com/121002781/215473393-5a645512-9edd-4698-ab82-bc0702a82e1d.png)

I found message encrypt in protocal ICMP

Now let's use the vigenère algorithm to decrypt the key is "knight"

![image](https://user-images.githubusercontent.com/121002781/215473827-f33d0175-3987-4a11-90f0-ee6165fbf0bb.png)

flag: KCTF{h1_th3n_wh0_ar3_y0u}
