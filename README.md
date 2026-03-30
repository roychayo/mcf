# Cache Configuration Parameters
## 505.mcf_r — gem5 Simulation (SPEC CPU2017)

---

## Single Level Cache (L1 Only)

| Parameter | iCache | dCache |
|---|---|---|
| Size | 64kB | 64kB |
| Associativity | 4-way | 4-way |
| Block Size | 64 bytes | 64 bytes |
| Replacement Policy | LRU | LRU |
| Tag Latency | 2 cycles | 2 cycles |
| Data Latency | 2 cycles | 2 cycles |
| Response Latency | 2 cycles | 2 cycles |
| MSHRs | 16 | 16 |

---

## Multi Level Cache (L1 + L2 + L3)

| Parameter | L1 (i+d) | L2 | L3 |
|---|---|---|---|
| Size | 64kB | 512kB | 2MB |
| Associativity | 4-way | 8-way | 16-way |
| Block Size | 64 bytes | 64 bytes | 64 bytes |
| Replacement Policy | LRU | LRU | LRU |
| Tag Latency | 2 cycles | 8 cycles | 20 cycles |
| Data Latency | 2 cycles | 8 cycles | 20 cycles |
| Response Latency | 2 cycles | 8 cycles | 20 cycles |
| MSHRs | 16 | 32 | 64 |

---

## System Configuration (Both)

| Parameter | Value |
|---|---|
| CPU Model | TimingSimpleCPU |
| Clock Speed | 2GHz |
| Memory | DDR4_2400_8x8 |
| Memory Size | 16GB |
| Simulation Mode | SE (Syscall Emulation) |
| gem5 Version | 25.1.0.0 |
| SPEC Version | CPU2017 v1.0.5 |
| Benchmark | 505.mcf_r |
| Input Size | Test + Train |
| Replacement Policy | LRU (gem5 default) |
