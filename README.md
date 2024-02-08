# MCP2515_CANBUS
Libreria per interfacciare schede Nucleo con CANBUS tramite MCP2515 e protocollo SPI

La velocità di comunicazione può essere impostata andando a modificare i valori dei registri **CNF1**, **CNF2**, **CNF3** all'interno del file *CAN_SPI.C* a partire dalla riga 112.

I possibili valori sono:  

Speed 8M \
#define MCP_8MHz_1000kBPS_CFG1 (0x00)  
#define MCP_8MHz_1000kBPS_CFG2 (0xC0)   /* Enabled SAM bit     */  
#define MCP_8MHz_1000kBPS_CFG3 (0x80)  /* Sample point at 75% */

#define MCP_8MHz_500kBPS_CFG1 (0x00)  
#define MCP_8MHz_500kBPS_CFG2 (0xD1)   /* Enabled SAM bit     */  
#define MCP_8MHz_500kBPS_CFG3 (0x81)   /* Sample point at 75% */  
  
#define MCP_8MHz_250kBPS_CFG1 (0x80)   /* Increased SJW       */  
#define MCP_8MHz_250kBPS_CFG2 (0xE5)   /* Enabled SAM bit     */  
#define MCP_8MHz_250kBPS_CFG3 (0x83)   /* Sample point at 75% */  

#define MCP_8MHz_200kBPS_CFG1 (0x80)   /* Increased SJW       */  
#define MCP_8MHz_200kBPS_CFG2 (0xF6)   /* Enabled SAM bit     */  
#define MCP_8MHz_200kBPS_CFG3 (0x84)   /* Sample point at 75% */  
  
#define MCP_8MHz_125kBPS_CFG1 (0x81)   /* Increased SJW       */  
#define MCP_8MHz_125kBPS_CFG2 (0xE5)   /* Enabled SAM bit     */  
#define MCP_8MHz_125kBPS_CFG3 (0x83)   /* Sample point at 75% */  
  
#define MCP_8MHz_100kBPS_CFG1 (0x81)   /* Increased SJW       */  
#define MCP_8MHz_100kBPS_CFG2 (0xF6)   /* Enabled SAM bit     */  
#define MCP_8MHz_100kBPS_CFG3 (0x84)   /* Sample point at 75% */  
  
#define MCP_8MHz_80kBPS_CFG1 (0x84)    /* Increased SJW       */  
#define MCP_8MHz_80kBPS_CFG2 (0xD3)    /* Enabled SAM bit     */  
#define MCP_8MHz_80kBPS_CFG3 (0x81)    /* Sample point at 75% */  
  
#define MCP_8MHz_50kBPS_CFG1 (0x84)    /* Increased SJW       */  
#define MCP_8MHz_50kBPS_CFG2 (0xE5)    /* Enabled SAM bit     */  
#define MCP_8MHz_50kBPS_CFG3 (0x83)    /* Sample point at 75% */  
  
#define MCP_8MHz_40kBPS_CFG1 (0x84)    /* Increased SJW       */  
#define MCP_8MHz_40kBPS_CFG2 (0xF6)    /* Enabled SAM bit     */  
#define MCP_8MHz_40kBPS_CFG3 (0x84)    /* Sample point at 75% */  
  
#define MCP_8MHz_33k3BPS_CFG1 (0x85)   /* Increased SJW       */  
#define MCP_8MHz_33k3BPS_CFG2 (0xF6)   /* Enabled SAM bit     */  
#define MCP_8MHz_33k3BPS_CFG3 (0x84)   /* Sample point at 75% */  
  
#define MCP_8MHz_31k25BPS_CFG1 (0x87)  /* Increased SJW       */  
#define MCP_8MHz_31k25BPS_CFG2 (0xE5)  /* Enabled SAM bit     */  
#define MCP_8MHz_31k25BPS_CFG3 (0x83)  /* Sample point at 75% */  
  
#define MCP_8MHz_20kBPS_CFG1 (0x89)    /* Increased SJW       */  
#define MCP_8MHz_20kBPS_CFG2 (0xF6)    /* Enabled SAM bit     */  
#define MCP_8MHz_20kBPS_CFG3 (0x84)    /* Sample point at 75% */  
  
#define MCP_8MHz_10kBPS_CFG1 (0x93)    /* Increased SJW       */  
#define MCP_8MHz_10kBPS_CFG2 (0xF6)    /* Enabled SAM bit     */  
#define MCP_8MHz_10kBPS_CFG3 (0x84)    /* Sample point at 75% */  
  
#define MCP_8MHz_5kBPS_CFG1 (0xA7)     /* Increased SJW       */  
#define MCP_8MHz_5kBPS_CFG2 (0xF6)     /* Enabled SAM bit     */  
#define MCP_8MHz_5kBPS_CFG3 (0x84)     /* Sample point at 75% */  
