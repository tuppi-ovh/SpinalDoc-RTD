
Apb3UartCtrl
============

Introduction
------------

The Apb3UartCtrl component is used to connect an UART interface to a APB3 bus.

Memory Mapping
--------------

.. list-table::
   :header-rows: 1
   :widths: 1 1 1 1 2

   * - Address
     - Width 
     - Name
     - Read / Write
     - Description

   * - 0x00
     - 0..7 bits
     - TxData
     - WO
     - Register to send data on UART

   * - 0x06
     - 0..7 bits 
     - TxFifoFree
     - RO
     - Register to get free space in the TX FIFO (only for 16-bit bus)

Attention! The user must align the address offset regarding the bus width. For example, 
the register TxFifoFree (address 0x06) will be accessed as 16 MSB while reading the address 0x04.