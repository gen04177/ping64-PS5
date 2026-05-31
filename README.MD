# ping64 PS5

## Description
This is a simple tool developed in C, designed to be used on a jailbroken PS5 for network diagnostics.



## Prerequisites
- elfldr.elf
- shsrv.elf
- ftpsrv.elf


## How to Use
1. Send the elfldr.elf payload to port 9020/9026/50000 of your PS5.
2. Send the shsrv.elf payload to port 9021 of your PS5.
3. Send the ftpsrv.elf payload to port 9021 of your PS5.
4. Copy the ping64.elf payload to `/data` or `/user/data` directory on your PS5.
5. Execute `telnet [PS5-IP] 2323`.
6. Run the command, e.g. `hbldr /data/ping64.elf -4 192.168.0.1` or `hbldr /data/ping64.elf -6 -c 10 2001:4860:4860::8888`.
7. `cat /user/temp/ping64.log` (optional)

Ping64 don´t resolve names only numeric IPv4/IPv6 addresses.

## Credits
- ps5-payload-dev
