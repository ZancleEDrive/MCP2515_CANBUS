# MCP2515_CANBUS
Libreria per interfacciare schede Nucleo con CANBUS tramite MCP2515 e protocollo SPI

La velocità di comunicazione può essere impostata andando a modificare i valori dei registri **CNF1**, **CNF2**, **CNF3** all'interno del file *CAN_SPI.C* a partire dalla riga 112.

I possibili valori sono:
**8MHz**  
#define MCP_8MHz_1000kBPS_CFG1 (0x00)  
#define MCP_8MHz_1000kBPS_CFG2 (0x80)  
#define MCP_8MHz_1000kBPS_CFG3 (0x80)  
  
#define MCP_8MHz_500kBPS_CFG1 (0x00)  
#define MCP_8MHz_500kBPS_CFG2 (0x90)  
#define MCP_8MHz_500kBPS_CFG3 (0x82)  
  
#define MCP_8MHz_250kBPS_CFG1 (0x00)  
#define MCP_8MHz_250kBPS_CFG2 (0xB1)  
#define MCP_8MHz_250kBPS_CFG3 (0x85)  
  
#define MCP_8MHz_200kBPS_CFG1 (0x00)  
#define MCP_8MHz_200kBPS_CFG2 (0xB4)  
#define MCP_8MHz_200kBPS_CFG3 (0x86)  
  
#define MCP_8MHz_125kBPS_CFG1 (0x01)  
#define MCP_8MHz_125kBPS_CFG2 (0xB1)  
#define MCP_8MHz_125kBPS_CFG3 (0x85)  
  
#define MCP_8MHz_100kBPS_CFG1 (0x01)  
#define MCP_8MHz_100kBPS_CFG2 (0xB4)  
#define MCP_8MHz_100kBPS_CFG3 (0x86)  
  
#define MCP_8MHz_80kBPS_CFG1 (0x01)  
#define MCP_8MHz_80kBPS_CFG2 (0xBF)  
#define MCP_8MHz_80kBPS_CFG3 (0x87)  
  
#define MCP_8MHz_50kBPS_CFG1 (0x03)  
#define MCP_8MHz_50kBPS_CFG2 (0xB4)  
#define MCP_8MHz_50kBPS_CFG3 (0x86)  
  
#define MCP_8MHz_40kBPS_CFG1 (0x03)  
#define MCP_8MHz_40kBPS_CFG2 (0xBF)  
#define MCP_8MHz_40kBPS_CFG3 (0x87)  
  
#define MCP_8MHz_33k3BPS_CFG1 (0x47)  
#define MCP_8MHz_33k3BPS_CFG2 (0xE2)  
#define MCP_8MHz_33k3BPS_CFG3 (0x85)  
  
#define MCP_8MHz_31k25BPS_CFG1 (0x07)  
#define MCP_8MHz_31k25BPS_CFG2 (0xA4)  
#define MCP_8MHz_31k25BPS_CFG3 (0x84)  
  
#define MCP_8MHz_20kBPS_CFG1 (0x07)  
#define MCP_8MHz_20kBPS_CFG2 (0xBF)  
#define MCP_8MHz_20kBPS_CFG3 (0x87)  
  
#define MCP_8MHz_10kBPS_CFG1 (0x0F)  
#define MCP_8MHz_10kBPS_CFG2 (0xBF)  
#define MCP_8MHz_10kBPS_CFG3 (0x87)  
  
#define MCP_8MHz_5kBPS_CFG1 (0x1F)  
#define MCP_8MHz_5kBPS_CFG2 (0xBF)  
#define MCP_8MHz_5kBPS_CFG3 (0x87)  
  
**16Mhz**  
#define MCP_16MHz_1000kBPS_CFG1 (0x00)  
#define MCP_16MHz_1000kBPS_CFG2 (0xD0)   
#define MCP_16MHz_1000kBPS_CFG3 (0x82)  
  
#define MCP_16MHz_500kBPS_CFG1 (0x00)  
#define MCP_16MHz_500kBPS_CFG2 (0xF0)  
#define MCP_16MHz_500kBPS_CFG3 (0x86)  
  
#define MCP_16MHz_250kBPS_CFG1 (0x41)  
#define MCP_16MHz_250kBPS_CFG2 (0xF1)  
#define MCP_16MHz_250kBPS_CFG3 (0x85)  
  
#define MCP_16MHz_200kBPS_CFG1 (0x01)  
#define MCP_16MHz_200kBPS_CFG2 (0xFA)  
#define MCP_16MHz_200kBPS_CFG3 (0x87)  
  
#define MCP_16MHz_125kBPS_CFG1 (0x03)  
#define MCP_16MHz_125kBPS_CFG2 (0xF0)  
#define MCP_16MHz_125kBPS_CFG3 (0x86)  
  
#define MCP_16MHz_100kBPS_CFG1 (0x03)  
#define MCP_16MHz_100kBPS_CFG2 (0xFA)  
#define MCP_16MHz_100kBPS_CFG3 (0x87)  
  
#define MCP_16MHz_95kBPS_CFG1 (0x03)  
#define MCP_16MHz_95kBPS_CFG2 (0xAD)  
#define MCP_16MHz_95kBPS_CFG3 (0x07)  
  
#define MCP_16MHz_83k3BPS_CFG1 (0x03)  
#define MCP_16MHz_83k3BPS_CFG2 (0xBE)  
#define MCP_16MHz_83k3BPS_CFG3 (0x07)  
  
#define MCP_16MHz_80kBPS_CFG1 (0x03)  
#define MCP_16MHz_80kBPS_CFG2 (0xFF)  
#define MCP_16MHz_80kBPS_CFG3 (0x87)  
  
#define MCP_16MHz_50kBPS_CFG1 (0x07)  
#define MCP_16MHz_50kBPS_CFG2 (0xFA)  
#define MCP_16MHz_50kBPS_CFG3 (0x87)  
  
#define MCP_16MHz_40kBPS_CFG1 (0x07)  
#define MCP_16MHz_40kBPS_CFG2 (0xFF)  
#define MCP_16MHz_40kBPS_CFG3 (0x87)  
  
#define MCP_16MHz_33k3BPS_CFG1 (0x4E)  
#define MCP_16MHz_33k3BPS_CFG2 (0xF1)  
#define MCP_16MHz_33k3BPS_CFG3 (0x85)  
  
#define MCP_16MHz_20kBPS_CFG1 (0x0F)  
#define MCP_16MHz_20kBPS_CFG2 (0xFF)  
#define MCP_16MHz_20kBPS_CFG3 (0x87)  
  
#define MCP_16MHz_10kBPS_CFG1 (0x1F)  
#define MCP_16MHz_10kBPS_CFG2 (0xFF)  
#define MCP_16MHz_10kBPS_CFG3 (0x87)  
  
#define MCP_16MHz_5kBPS_CFG1 (0x3F)  
#define MCP_16MHz_5kBPS_CFG2 (0xFF)  
#define MCP_16MHz_5kBPS_CFG3 (0x87)  
  
**20MHz**
#define MCP_20MHz_1000kBPS_CFG1 (0x00)  
#define MCP_20MHz_1000kBPS_CFG2 (0xD9)  
#define MCP_20MHz_1000kBPS_CFG3 (0x82)  
  
#define MCP_20MHz_500kBPS_CFG1 (0x00)  
#define MCP_20MHz_500kBPS_CFG2 (0xFA)  
#define MCP_20MHz_500kBPS_CFG3 (0x87)  
  
#define MCP_20MHz_250kBPS_CFG1 (0x41)  
#define MCP_20MHz_250kBPS_CFG2 (0xFB)  
#define MCP_20MHz_250kBPS_CFG3 (0x86)  
  
#define MCP_20MHz_200kBPS_CFG1 (0x01)  
#define MCP_20MHz_200kBPS_CFG2 (0xFF)  
#define MCP_20MHz_200kBPS_CFG3 (0x87)  
  
#define MCP_20MHz_125kBPS_CFG1 (0x03)  
#define MCP_20MHz_125kBPS_CFG2 (0xFA)  
#define MCP_20MHz_125kBPS_CFG3 (0x87)  
  
#define MCP_20MHz_100kBPS_CFG1 (0x04)  
#define MCP_20MHz_100kBPS_CFG2 (0xFA)  
#define MCP_20MHz_100kBPS_CFG3 (0x87)  
  
#define MCP_20MHz_83k3BPS_CFG1 (0x04)  
#define MCP_20MHz_83k3BPS_CFG2 (0xFE)  
#define MCP_20MHz_83k3BPS_CFG3 (0x87)  
  
#define MCP_20MHz_80kBPS_CFG1 (0x04)  
#define MCP_20MHz_80kBPS_CFG2 (0xFF)  
#define MCP_20MHz_80kBPS_CFG3 (0x87)  
  
#define MCP_20MHz_50kBPS_CFG1 (0x09)  
#define MCP_20MHz_50kBPS_CFG2 (0xFA)  
#define MCP_20MHz_50kBPS_CFG3 (0x87)  
  
#define MCP_20MHz_40kBPS_CFG1 (0x09)  
#define MCP_20MHz_40kBPS_CFG2 (0xFF)  
#define MCP_20MHz_40kBPS_CFG3 (0x87)  
  
#define MCP_20MHz_33k3BPS_CFG1 (0x0B)  
#define MCP_20MHz_33k3BPS_CFG2 (0xFF)  
#define MCP_20MHz_33k3BPS_CFG3 (0x87)  
