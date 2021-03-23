
Apb3Gpio
========

Introduction
------------

The Apb3Gpio component is used to connect a GPIO interface to an APB3 bus.

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
     - 0..31 bits
     - gpioRead
     - RO
     - Register to read the physical pin values

   * - 0x04
     - 0..31 bits
     - gpioWrite
     - RW 
     - Register to access the output values

   * - 0x08
     - 0..31 bits
     - gpioDirection
     - RW
     - Register to set the GPIO pin directions. When set, the corresponding pin is set as output

