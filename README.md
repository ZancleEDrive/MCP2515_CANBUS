# MCP2515_CANBUS
Libreria per interfacciare schede Nucleo con CANBUS tramite MCP2515 e protocollo SPI

La velocità di comunicazione può essere impostata andando a modificare i valori dei registri **CNF1**, **CNF2**, **CNF3** all'interno del file *CAN_SPI.C* a partire dalla riga 112.

I possibili valori sono:  

Speed 8M \
8MHz 1000kBPS CNF1 -  0x00 \
8MHz 1000kBPS CNF2 -  0x80 \
8MHz 1000kBPS CNF3 -  0x80 

8MHz 500kBPS CNF1 -  0x00 \
8MHz 500kBPS CNF2 -  0x90 \
8MHz 500kBPS CNF3 -  0x82 

8MHz 250kBPS CNF1 -  0x00 \
8MHz 250kBPS CNF2 -  0xB1 \
8MHz 250kBPS CNF3 -  0x85 

8MHz 200kBPS CNF1 -  0x00 \
8MHz 200kBPS CNF2 -  0xB4 \
8MHz 200kBPS CNF3 -  0x86 

8MHz 125kBPS CNF1 -  0x01 \
8MHz 125kBPS CNF2 -  0xB1 \
8MHz 125kBPS CNF3 -  0x85 

8MHz 100kBPS CNF1 -  0x01 \
8MHz 100kBPS CNF2 -  0xB4 \
8MHz 100kBPS CNF3 -  0x86

8MHz 80kBPS CNF1 -  0x01 \
8MHz 80kBPS CNF2 -  0xBF \
8MHz 80kBPS CNF3 -  0x87 

8MHz 50kBPS CNF1 -  0x03 \
8MHz 50kBPS CNF2 -  0xB4 \
8MHz 50kBPS CNF3 -  0x86 

8MHz 40kBPS CNF1 -  0x03 \
8MHz 40kBPS CNF2 -  0xBF \
8MHz 40kBPS CNF3 -  0x87 

8MHz 33k3BPS CNF1 -  0x47 \
8MHz 33k3BPS CNF2 -  0xE2 \
8MHz 33k3BPS CNF3 -  0x85 

8MHz 31k25BPS CNF1 -  0x07 \
8MHz 31k25BPS CNF2 -  0xA4 \
8MHz 31k25BPS CNF3 -  0x84 

8MHz 20kBPS CNF1 -  0x07 \
8MHz 20kBPS CNF2 -  0xBF \
8MHz 20kBPS CNF3 -  0x87 

8MHz 10kBPS CNF1 -  0x0F \
8MHz 10kBPS CNF2 -  0xBF \
8MHz 10kBPS CNF3 -  0x87 

8MHz 5kBPS CNF1 -  0x1F \
8MHz 5kBPS CNF2 -  0xBF \
8MHz 5kBPS CNF3 -  0x87 
