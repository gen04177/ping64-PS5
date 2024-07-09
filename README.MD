# ping4 PS5

## Description
This is a simple tool developed in C, designed to be used on a PS5 with Jailbreak firmware (3.xx-4.xx).



## Prerequisites
- elfldr.elf
- shsrv.elf
- ftpsrv.elf


## How to Use
1. Send the elfldr.elf payload to port 9020 of your PS5.
2. Send the shsrv.elf payload to port 9021 of your PS5.
3. Send the ftpsrv.elf payload to port 9021 of your PS5.
4. Copy the ping4.elf payload to `/data` or `/user/data` directory on your PS5.
5. Execute `telnet [PS5-IP] 2323`.
6. cd `/data`
7. Run the command `hbldr ping4.elf 192.168.0.1` (or `hbldr ping4.elf -c 10 192.168.0.1`).

Ping4 don´t resolve names only IPv4 addresses.

## Credits
Credits to J. Tornblom for the SDK, SDL2 port for PS5, and other payloads.
