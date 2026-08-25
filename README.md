# EVM-FPGA-project

## FPGA-Based Electronic Voting Machine
##1. Project Description
This project is a compact digital voting machine built entirely in hardware description language (like Verilog) and implemented on an FPGA. Every part of this machine runs as dedicated, always-on digital hardware, described as separate modules that operate simultaneously and communicate through clearly defined signals.
The machine performs four essential jobs: 
1) Confirms person trying to vote is eligible and hasn't already voted.
2) Lets the eligible voter cast exactly one vote.
3) Keeps the running tally completely hidden from view while polling is open.
4) Produces a timestamped, non-reversible record of what happened, so the results can be trusted and checked afterward.
The goal here is to design a system that is difficult to cheat, whether the person attempting to cheat is a voter (trying to vote twice, or without authorization) or the machine's own operator (trying to see results early, alter the count, or hide evidence of tampering).
##Core Features
•	Voter authentication using an UART-output barcode scanner
•	Exactly one permitted vote per authenticated voter - no re-use, no double count
•	Live vote counting that stays completely hidden from any display while polling is open
•	Result totals released only after an admin deliberately closes polling
•	A separate admin mode for election setup, live monitoring, and closing polling
•	Tamper detection through a case-open switch and unexpected-reset detection
•	A timestamped, identity-free audit log for post-election review


### Project Summary

### Core Features
