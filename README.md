# Simulasi-Blender-Menggunakan-Motor-DC
Simulasi ini menggunakan komponen utama  IC AT89C51,Motor DC dan Switch


ORG 00H
MOV P0,#00000001B
simulasi : MOV A,P0
RRC A
JC lanjut
SETB P2.0
SETB P2.1

SJMP simulasi
lanjut : RRC A         
JC simulasi
CLR P2.0
CLR P2.1


SJMP simulasi
END
