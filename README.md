# Week-_0-Risc-v-_tapeout
This document outlines the environment setup, installation, and tool verification steps for digital design tapeout, incorporating your configuration and screenshots to demonstrate successful installation and usage.
## System Information
Gathered via:
<pre>neofetch</pre>
### Example output:

OS: Ubuntu 22.04.5 LTS x86_64

Kernel: 6.8.0-40-generic

CPU: Intel i7-11370H (11th Gen)

GPU: VMware SVGA II Adapter

Shell: bash 5.1.16

Memory: 7162MB

## References 
![references](https://github.com/praaveenharigs/Week-_0-Risc-v-_tapeout/blob/main/pictures/IMG-20250920-WA0011%20(7).jpg)

## Yosys Installation & Verification
Yosys is an open-source synthesis tool used for RTL-to-gate conversion.

### Installation
<pre>sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make               
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
 make config-gcc
git submodule update --init --recursive
make 
sudo make install</pre>
![yosys](https://github.com/praaveenharigs/Week-_0-Risc-v-_tapeout/blob/main/pictures/IMG-20250920-WA0011%20(6).jpg)

## Iverilog Installation & Verification
Iverilog is a popular Verilog simulation tool.

### Installation
<pre>sudo apt update
sudo apt-get install iverilog
</pre>
### Verification

Run:
<pre>iverilog</pre>
![iverilog](https://github.com/praaveenharigs/Week-_0-Risc-v-_tapeout/blob/main/pictures/IMG-20250920-WA0011%20(10).jpg)

## GTKWave Installation & Verification
GTKWave is a waveform analyzer for viewing .vcd simulation results.

### Installation
Recommended:
<pre>sudo apt update
sudo apt install gtkwave
</pre>
![gtk](https://github.com/praaveenharigs/Week-_0-Risc-v-_tapeout/blob/main/pictures/IMG-20250920-WA0011%20(9).jpg)

### Tools
|Tool|Command|Installed version|
|----|-------|-----------------|
|gftyf|vrd|dvrdrd5d|
