# Challenge: Plain
## Author: r1c3t
## Link: 
    https://tamuctf.com/challenges#Plain-9

- The challenge asks us to find the flag in the plain.zip file
<p align="center"><img src="./images/plain1.png"></p>

- Check file plain.zip and extract file
<p align="center"><img src="./images/plain2.png"></p>

- We see pcap file in the plain.zip file, we will open it on wireshark tool
<p align="center"><img src="./images/plain3.png"></p>

- Notice, we will see a telet protocol between the machine .129 and the machine .133, we will observe it with TCP stream.

- In the conversation between the two machines, we see the command line read Flag: cat flag.txt... What we get is a base64 string `Z2lnZW17ZDBudF91czNfdDNsbmV0X2V2M3J9Cg==`
<p align="center"><img src="./images/plain4.png"></p>

- Decoding us is flag is `gigem{d0nt_us3_t3lnet_ev3r}`

## Flag is `gigem{d0nt_us3_t3lnet_ev3r}`