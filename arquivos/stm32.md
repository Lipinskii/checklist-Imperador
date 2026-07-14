# Resumo Geral - STM32 - Apito

## Introdução

O STM32F411CEU6 é um microcontrolador de 32 bits baseado no núcleo Arm Cortex-M4 com unidade de processamento de ponto flutuante (FPU), operando em frequências de até 100MHz (gerando até 125 DMIPS). Ele se destaca pelo recurso BAM (Batch Acquisition Mode), desenvolvido para economizar energia ao transferir e processar dados de sensores em lote com a CPU desligada.

## Principais Funções

* Baseado no núcleo Arm Cortex-M4 equipado com FPU, operando em uma frequência de até 100MHz
* Oferece até 512 KB de memória Flash e 128 KB de SRAM
* Conta com até 11 temporizadores, incluindo seis de 16 bits e dois de 32 bits que chegam a 100MHz, além de dois watchdogs e um timer SysTick
* Possui acelerador de memória (ART Accelerator) para permitir execução sem estados de espera (0-wait state) a partir da memória flash
* Recurso de eficiência que otimiza e reduz consideravelmente o consumo de energia enquanto adquire dados em lote de sensores ou periféricos (Modo BAM)
* Possui 2 controladores DMA com 8 fluxos (streams) cada, suporte a FIFOs e transferências em rajada (burst)
* Possui um ADC de 12 bits e 2.4 MSPS capaz de realizar leitura em até 16 canais
* Possui conectividade avançada com até 3 interfaces I2C, 3 USARTs (chegando a até 12.5 Mbit/s), 5 interfaces SPI/I2S, 1 interface SDIO (para cartões SD/MMC) e um controlador USB 2.0 OTG full-speed com PHY integrado

## Características Elétricas

* Tensão de alimentação de 1.7V-3.6V
* Consumo típico de 100 µA/MHz em operação e 42 µA a 25°C com a Flash em modo Stop (e tempo de _wakeup_ rápido). O consumo cai para até 9 µA a 25°C com a Flash em modo "Deep power down"
* Consumo em Modo Standby de 1.8 µA a 25°C (sob tensão de 1.7V sem uso do RTC)
* Alimentação de Backup utilizada para o RTC, operando na faixa de 1.65V a 3.6V e consumindo tipicamente 1 µA a 25°C
* Oscilador interno RC de 16MHz, oscilador de cristal externo de 4 a 26MHz, e osciladores de 32kHz para o RTC
