# QXDM [0xB821]Paging ng-5G-S-TMSI Converter
online calculate: https://dustinchen26.github.io/paging

## Spec
```
(ng-5G-S-TMSI)=(AMF Set ID)+(AMF Pointer)+(5G-TMSI)
(48 bits)=(10 bits)+(6 bits)+(32 bits)
```

## Example
```
Please enter the 48 bits number from QXDM [0xB821] PCCH / Paging
ue-Identity ng-5G-S-TMSI :
00000001 00000001 00000111 10111010 00111101 00001011

 Convert
 
【Debug Info】:
AMF Set ID (10 bits): 0000000100 (Decimal: 4)
AMF Pointer (6 bits): 000001 (Decimal: 1)
5G-TMSI (32 bits): 00000111101110100011110100001011 (Decimal: 129645835)


【QXDM result】[0xB80A] Registration accept
AMF_SET_ID = 4
AMF_Pointer = 1
_5g_tmsi[0] = 7 (0x7)
_5g_tmsi[1] = 186 (0xba)
_5g_tmsi[2] = 61 (0x3d)
_5g_tmsi[3] = 11 (0xb)


【wireshark result】InitialContextSetupRequest, Registration accept
AMF Set ID: 4
AMF Pointer: 1
5G-TMSI: 129645835
```