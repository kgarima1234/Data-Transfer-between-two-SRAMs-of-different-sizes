# Data-Transfer-between-two-SRAMs-of-different-sizes
Designed FSM for transferring the data from one SRAM of 8bit*32 locations to another SRAM of 16bit*16 locations making a data transfer bridge between two modules of different sizes.<br>
Module one processes data and as the result, inside the SRM eight bit by 32 locations, Module one signals that it's finished operating and data must be resized and stored in an SRM 16 bit by 16 locations to be processed further by module which is our design behaves as a data transfer bridge between two subsystems.

The FSM rearranges data in groups Byte Address Zero and Byte Address one from SRM in two word address zero in SRAMs out. The same process continues until all addresses from SRM and are processed. The FSM signals that it finished transferring and resizing data so Module two can start reading it from the SRAM.<br>


