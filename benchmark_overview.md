# Benchmark Database

This document provides an overview of all benchmarks in the database, according to category. Each benchmark is described with its key properties and a brief explanation of what it measures. We also include a table with summary statistics of the profiles we collected for each benchmark (sorted by median clock offset). For more detailed information, see the benchmark definition in the source code at `ptp_perf/registry/benchmark_db.py`.

### Benchmark: Baseline
_Id: `base`, 2 machines, 0:20:00 duration._

The base benchmark to compare other benchmarks against. It is the default benchmark for all new clusters. It is used to measure the performance of the cluster without any additional load or faults. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 37 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 15 µs | 63 µs| 0% | 98% | 0:00:10 | 12 µs | 1.2 µs |
| 30 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 14 µs | 64 µs| 0% | 99% | 0:00:10.032930 | 12 µs | 1.2 µs |
| 12 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.2 µs | 16 µs | 65 µs| 0% | 98% | 0:00:10 | 16 µs | 1.6 µs |
| 29 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.0 µs | 41 µs | 74 µs| 0% | 13% | 0:04:08.878127 | 109 µs | 438 ns |
| 11 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 15 µs | 66 µs| 0% | 99% | 0:00:16.998398 | 41 µs | 2.4 µs |
| 40 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 15 µs | 65 µs| 0% | 99% | 0:01:03.005037 | 37 µs | 588 ns |
| 24 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 24 µs | 57 µs | 87 µs| 0.3% | 4% | 0:02:32.968138 | 113 µs | 739 ns |
| 6 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 15 µs | 63 µs| 0% | 100% | 0:00:10 | 19 µs | 1.9 µs |
| 36 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.4 µs | 25 µs | 78 µs| 0% | 13% | 0:04:46.957401 | 125 µs | 435 ns |
| 28 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.8 µs | 15 µs | 66 µs| 0% | 99% | 0:00:14.959704 | 31 µs | 2.1 µs |
| 26 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.9 µs | 14 µs | 64 µs| 0% | 98% | 0:00:34.016421 | 24 µs | 702 ns |
| 41 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.6 µs | 49 µs | 81 µs| 0% | 9% | 0:03:50.975885 | 130 µs | 562 ns |
| 31 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 22 µs | 66 µs | 89 µs| 0% | 5% | 0:01:37.904371 | 104 µs | 1.1 µs |
| 42 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 16 µs | 64 µs| 0% | 99% | 0:00:45.000729 | 42 µs | 943 ns |
| 27 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.4 µs | 44 µs | 79 µs| 0.3% | 12% | 0:03:02.972835 | 114 µs | 626 ns |
| 137 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 4.5 µs | 122 µs| 0% | 98% | 0:00:16.144060 | 22 µs | 1.4 µs |
| 113 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 546 ns | 1.7 µs | 78 µs| 0% | 100% | 0:00:12.006429 | 20 µs | 1.7 µs |
| 102 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 8.7 µs | 74 µs| 0% | 100% | 0:00:12.994097 | 12 µs | 898 ns |
| 141 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 173 ns | 462 ns | 75 µs| 0% | 98% | 0:00:12.154086 | 46 µs | 3.8 µs |
| 139 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.2 µs | 3.6 µs | 116 µs| 0% | 10% | 0:04:31.955266 | 90 µs | 333 ns |
| 103 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.7 µs | 8.6 µs | 72 µs| 0% | 100% | 0:00:16.971006 | 42 µs | 2.5 µs |
| 135 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 498 ns | 1.5 µs | 78 µs| 0% | 100% | 0:00:12.005808 | 19 µs | 1.6 µs |
| 156 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 7.8 µs | 67 µs| 0% | 100% | 0:00:10.000509 | 17 µs | 1.7 µs |
| 161 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 207 ns | 667 ns | 75 µs| 0% | 86% | 0:00:17.205229 | 30 µs | 1.7 µs |
| 162 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.0 µs | 3.7 µs | 116 µs| 0% | 10% | 0:04:23.900415 | 95 µs | 358 ns |
| 172 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 491 ns | 1.6 µs | 78 µs| 0% | 100% | 0:00:14.009262 | 20 µs | 1.4 µs |
| 167 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 328 ns | 861 ns | 37 µs| 0% | 100% | 0:00:12.000333 | 848 ms | 71 ms |
| 153 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.8 µs | 67 µs| 0% | 100% | 0:00:12.002138 | 15 µs | 1.2 µs |
| 150 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.5 µs | 122 µs| 0% | 99% | 0:00:20.168337 | 23 µs | 1.1 µs |
| 140 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 4.6 µs | 120 µs| 0% | 99% | 0:00:17.173433 | 25 µs | 1.5 µs |
| 146 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.4 µs | 122 µs| 0% | 97% | 0:00:21.270632 | 15 µs | 707 ns |
| 133 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 4.3 µs | 122 µs| 0% | 98% | 0:00:14.174504 | 32 µs | 2.2 µs |
| 177 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 174 ns | 7.9 µs | 75 µs| 0% | 89% | 0:00:21.223052 | 37 µs | 1.7 µs |
| 173 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 158 ns | 440 ns | 75 µs| 0% | 97% | 0:00:17.181288 | 37 µs | 2.2 µs |
| 181 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 173 ns | 471 ns | 75 µs| 0% | 95% | 0:00:13.128299 | 44 µs | 3.3 µs |
| 176 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 498 ns | 1.7 µs | 78 µs| 0% | 100% | 0:00:14.004155 | 18 µs | 1.3 µs |
| 174 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.1 µs | 3.4 µs | 116 µs| 0% | 8% | 0:05:10.987683 | 94 µs | 302 ns |
| 158 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.2 µs | 4.2 µs | 116 µs| 0% | 8% | 0:04:38.991473 | 83 µs | 296 ns |
| 178 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.0 µs | 3.3 µs | 116 µs| 0% | 11% | 0:04:22.979012 | 91 µs | 347 ns |
| 155 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 7.4 µs | 68 µs| 0% | 100% | 0:00:10 | 6.8 µs | 683 ns |
| 175 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 309 ns | 875 ns | 37 µs| 0% | 100% | 0:00:10 | 406 ms | 41 ms |
| 170 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.1 µs | 3.5 µs | 116 µs| 0% | 11% | 0:04:48.989623 | 94 µs | 326 ns |
| 179 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 318 ns | 832 ns | 37 µs| 0% | 100% | 0:00:14.000561 | 559 ms | 40 ms |
| 185 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 170 ns | 456 ns | 75 µs| 0% | 96% | 0:00:13.129479 | 6.4 µs | 486 ns |
| 169 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 160 ns | 444 ns | 75 µs| 0% | 99% | 0:00:17.227650 | 44 µs | 2.6 µs |
| 165 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 188 ns | 494 ns | 75 µs| 0% | 94% | 0:00:17.202614 | 5.2 µs | 304 ns |
| 154 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 4.8 µs | 122 µs| 0% | 96% | 0:00:17.230200 | 36 µs | 2.1 µs |
| 152 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 4.8 µs | 121 µs| 0% | 98% | 0:00:16.184994 | 42 µs | 2.6 µs |
| 151 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 7.3 µs | 67 µs| 0% | 100% | 0:00:10 | 9.6 µs | 965 ns |
| 149 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.5 µs | 67 µs| 0% | 100% | 0:00:10 | 7.6 µs | 762 ns |
| 148 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.9 µs | 122 µs| 0% | 99% | 0:00:20.294178 | 22 µs | 1.1 µs |
| 145 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.6 µs | 67 µs| 0% | 100% | 0:00:13.000421 | 15 µs | 1.2 µs |
| 144 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 4.7 µs | 121 µs| 0% | 99% | 0:00:17.224445 | 21 µs | 1.2 µs |
| 143 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.6 µs | 67 µs| 0% | 100% | 0:00:10 | 5.4 µs | 538 ns |
| 142 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 4.9 µs | 123 µs| 0% | 98% | 0:00:14.157623 | 33 µs | 2.3 µs |
| 168 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 512 ns | 1.6 µs | 78 µs| 0% | 100% | 0:00:15.004443 | 19 µs | 1.3 µs |
| 160 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 478 ns | 1.5 µs | 78 µs| 0% | 100% | 0:00:15.006217 | 17 µs | 1.2 µs |
| 180 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 480 ns | 1.8 µs | 78 µs| 0% | 100% | 0:00:12.006187 | 18 µs | 1.5 µs |
| 184 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 486 ns | 1.6 µs | 78 µs| 0% | 100% | 0:00:14.001733 | 19 µs | 1.4 µs |
| 188 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 499 ns | 1.6 µs | 78 µs| 0% | 100% | 0:00:15.007376 | 4.9 µs | 324 ns |
| 189 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 190 ns | 639 ns | 75 µs| 0% | 93% | 0:00:12.151324 | 38 µs | 3.1 µs |
| 1939 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 18 µs | 63 µs| 0% | 7% | 0:08:29.036704 | 1.6 ms | 3.1 µs |
| 976 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.8 µs | 7.3 µs | 40 µs| 0% | 100% | 0:00:13.005611 | 6.8 µs | 525 ns |
| 1940 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.7 µs | 13 µs | 59 µs| 0% | 99% | 0:01:09.011719 | 73 µs | 1.1 µs |
| 1941 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 7.4 µs | 67 µs| 0% | 100% | 0:00:14.004067 | 56 µs | 4.0 µs |
| 994 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 2.5 µs | 9.5 µs | 45 µs| 0% | 11% | 0:00:29.926405 | 53 µs | 1.8 µs |
| 987 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 382 ns | 1.1 µs | 20 µs| 0% | 99% | 0:00:17.000663 | 2.6 µs | 154 ns |
| 1943 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.6 µs | 10 µs | 61 µs| 0% | 18% | 0:09:43.098803 | 1.6 ms | 2.7 µs |
| 1944 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 14 µs | 58 µs| 0% | 97% | 0:00:50.794971 | 65 µs | 1.3 µs |
| 1003 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 3.0 µs | 11 µs | 45 µs| 0% | 6% | 0:00:50.985863 | 52 µs | 1.0 µs |
| 996 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 2.9 µs | 11 µs | 46 µs| 0% | 8% | 0:01:30.981279 | 53 µs | 586 ns |
| 1935 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.7 µs | 16 µs | 66 µs| 0% | 12% | 0:08:33.076534 | 1.6 ms | 3.0 µs |
| 1937 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 8.7 µs | 67 µs| 0% | 100% | 0:00:11.000934 | 52 µs | 4.7 µs |
| 982 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 2.5 µs | 9.5 µs | 44 µs| 0% | 9% | 0:00:43.567797 | 63 µs | 1.5 µs |
| 983 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 394 ns | 1.2 µs | 20 µs| 0% | 99% | 0:00:11.000345 | 200 ms | 18 ms |
| 1938 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.7 µs | 120 µs| 0% | 97% | 0:00:11.949989 | 18 µs | 1.5 µs |
| 1006 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 353 ns | 1.1 µs | 42 µs| 0% | 72% | 0:00:16.214566 | 28 µs | 1.7 µs |
| 984 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.6 µs | 6.5 µs | 40 µs| 0% | 100% | 0:00:10 | 9.1 µs | 912 ns |
| 1945 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 8.1 µs | 67 µs| 0% | 100% | 0:00:14.007194 | 61 µs | 4.4 µs |
| 1018 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 377 ns | 1.2 µs | 42 µs| 0% | 76% | 0:00:14.152085 | 14 µs | 964 ns |
| 1021 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.9 µs | 6.9 µs | 40 µs| 0% | 100% | 0:00:11.005483 | 4.3 µs | 387 ns |
| 985 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 392 ns | 1.3 µs | 42 µs| 0% | 76% | 0:00:21.266011 | 17 µs | 813 ns |
| 1008 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 367 ns | 1.1 µs | 20 µs| 0% | 99% | 0:00:10.999804 | 139 ms | 13 ms |
| 1946 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.4 µs | 120 µs| 0% | 95% | 0:00:24.274429 | 20 µs | 827 ns |
| 1947 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 9.0 µs | 61 µs| 0% | 18% | 0:04:43.939251 | 111 µs | 393 ns |
| 1948 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.1 µs | 14 µs | 59 µs| 0% | 100% | 0:00:10.003339 | 11 µs | 1.1 µs |
| 989 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 366 ns | 1.2 µs | 42 µs| 0% | 86% | 0:00:23.253716 | 14 µs | 621 ns |
| 1950 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.0 µs | 4.1 µs | 118 µs| 0% | 96% | 0:00:14.162206 | 20 µs | 1.4 µs |
| 1951 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.5 µs | 14 µs | 61 µs| 0% | 12% | 0:03:38.981118 | 98 µs | 449 ns |
| 913 | Baseline | PTPd | None | petalinux02 | PRIMARY_SLAVE | 3.0 µs | 11 µs | 43 µs| 0% | 10% | 0:00:40.926629 | 49 µs | 1.2 µs |
| 1020 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 367 ns | 1.1 µs | 42 µs| 0% | 79% | 0:00:17.140083 | 26 µs | 1.5 µs |
| 990 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 3.0 µs | 10 µs | 46 µs| 0% | 11% | 0:00:42.977687 | 44 µs | 1.0 µs |
| 911 | Baseline | PTP4L | None | petalinux02 | PRIMARY_SLAVE | 7.3 µs | 21 µs | 37 µs| 0% | 99% | 0:00:13.999936 | 24 µs | 1.7 µs |
| 912 | Baseline | PTP4L | None | petalinux02 | PRIMARY_SLAVE | 7.6 µs | 20 µs | 38 µs| 0% | 98% | 0:00:10 | 17 µs | 1.7 µs |
| 914 | Baseline | PTPd | None | petalinux02 | PRIMARY_SLAVE | 3.0 µs | 10 µs | 43 µs| 0% | 11% | 0:01:08.893306 | 58 µs | 841 ns |
| 1953 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 7.9 µs | 67 µs| 0% | 100% | 0:00:10 | 7.4 µs | 740 ns |
| 991 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 387 ns | 1.1 µs | 20 µs| 0% | 100% | 0:00:15.000115 | 2.4 µs | 161 ns |
| 1954 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.6 µs | 118 µs| 0% | 99% | 0:00:18.191713 | 9.6 µs | 528 ns |
| 972 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 380 ns | 1.0 µs | 20 µs| 0% | 99% | 0:00:12.000413 | 757 ms | 63 ms |
| 1005 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.8 µs | 6.6 µs | 40 µs| 0% | 100% | 0:00:10 | 7.4 µs | 738 ns |
| 974 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.7 µs | 6.9 µs | 40 µs| 0% | 100% | 0:00:10 | 6.0 µs | 601 ns |
| 1013 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 2.0 µs | 7.2 µs | 40 µs| 0% | 100% | 0:00:11.004012 | 5.7 µs | 517 ns |
| 970 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 2.5 µs | 9.4 µs | 46 µs| 0% | 9% | 0:00:47.969051 | 47 µs | 982 ns |
| 1022 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 370 ns | 1.2 µs | 42 µs| 0% | 83% | 0:00:16.166723 | 72 µs | 4.5 µs |
| 1002 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 378 ns | 1.1 µs | 42 µs| 0% | 77% | 0:00:24.254410 | 13 µs | 556 ns |
| 971 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 367 ns | 1.1 µs | 42 µs| 0% | 75% | 0:00:18.189689 | 16 µs | 865 ns |
| 1001 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.5 µs | 6.2 µs | 40 µs| 0% | 100% | 0:00:12.003742 | 6.4 µs | 537 ns |
| 973 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.6 µs | 6.5 µs | 39 µs| 0% | 100% | 0:00:10 | 6.0 µs | 600 ns |
| 1004 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 380 ns | 1.1 µs | 20 µs| 0% | 100% | 0:00:23.000293 | 110 ms | 4.8 ms |
| 992 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 2.9 µs | 9.7 µs | 46 µs| 0% | 11% | 0:01:06.927251 | 49 µs | 732 ns |
| 1310 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.0 µs | 12 µs | 194 µs| 0% | 98% | 0:00:11.126457 | 90 µs | 8.1 µs |
| 1307 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.1 µs | 11 µs | 194 µs| 0% | 97% | 0:00:12.124015 | 61 µs | 5.0 µs |
| 1318 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 1.8 µs | 7.0 µs | 57 µs| 0% | 95% | 0:00:13.000874 | 64 µs | 4.9 µs |
| 1309 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 1.9 µs | 6.1 µs | 57 µs| 0% | 97% | 0:02:41.009543 | 42 µs | 263 ns |
| 1319 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.0 µs | 12 µs | 197 µs| 0% | 97% | 0:00:11.099667 | 76 µs | 6.8 µs |
| 1312 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 1.8 µs | 6.8 µs | 57 µs| 0% | 98% | 0:00:10 | 10 µs | 1.0 µs |
| 1315 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.0 µs | 7.8 µs | 57 µs| 0% | 92% | 0:00:14.000996 | 21 µs | 1.5 µs |
| 1306 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 1.9 µs | 7.2 µs | 57 µs| 0% | 92% | 0:01:10.004856 | 18 µs | 261 ns |
| 1316 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 1.8 µs | 12 µs | 196 µs| 0% | 97% | 0:00:12.159509 | 67 µs | 5.5 µs |
| 1348 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 202 ns | 586 ns | 37 µs| 0% | 100% | 0:00:34.792964 | 393 ms | 11 ms |
| 1351 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.8 µs | 9.5 µs | 64 µs| 0% | 7% | 0:00:48.973639 | 55 µs | 1.1 µs |
| 1347 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.4 µs | 8.3 µs | 62 µs| 0% | 15% | 0:00:55.043623 | 61 µs | 1.1 µs |
| 1371 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 208 ns | 591 ns | 37 µs| 0% | 100% | 0:00:33.908771 | 489 ms | 14 ms |
| 1373 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 214 ns | 602 ns | 37 µs| 0% | 100% | 0:00:30.914136 | 183 ms | 5.9 ms |
| 1370 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 314 ns | 861 ns | 20 µs| 0% | 96% | 0:00:14.003963 | 3.0 µs | 212 ns |
| 1361 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 287 ns | 812 ns | 20 µs| 0% | 99% | 0:00:16.005852 | 2.5 µs | 154 ns |
| 1357 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 297 ns | 827 ns | 20 µs| 0% | 99% | 0:00:15.007330 | 2.6 µs | 173 ns |
| 1354 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 206 ns | 593 ns | 37 µs| 0% | 100% | 0:00:35.960434 | 772 ms | 21 ms |
| 1360 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 202 ns | 574 ns | 37 µs| 0% | 100% | 0:00:36.963297 | 718 ms | 19 ms |
| 1372 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 288 ns | 813 ns | 20 µs| 0% | 97% | 0:00:18.008624 | 2.6 µs | 145 ns |
| 1384 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 197 ns | 590 ns | 37 µs| 0% | 100% | 0:00:23.988610 | 201 ms | 8.4 ms |
| 1385 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 293 ns | 834 ns | 20 µs| 0% | 99% | 0:00:19.009624 | 3.2 µs | 168 ns |
| 1380 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 218 ns | 592 ns | 37 µs| 0% | 100% | 0:00:32.972193 | 452 ms | 14 ms |
| 1383 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 310 ns | 875 ns | 20 µs| 0% | 98% | 0:00:18.013545 | 3.7 µs | 204 ns |
| 1375 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 212 ns | 605 ns | 37 µs| 0% | 100% | 0:00:28.981238 | 395 ms | 14 ms |
| 1381 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 304 ns | 872 ns | 20 µs| 0% | 98% | 0:00:26.012550 | 2.8 µs | 106 ns |
| 187 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 312 ns | 847 ns | 37 µs| 0% | 100% | 0:00:16.003992 | 77 ms | 4.8 ms |
| 111 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 333 ns | 835 ns | 37 µs| 0% | 100% | 0:00:12.997231 | 564 ms | 43 ms |
| 1369 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 210 ns | 577 ns | 37 µs| 0% | 100% | 0:00:33.916557 | 495 ms | 15 ms |
| 1352 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 206 ns | 602 ns | 37 µs| 0% | 100% | 0:00:27.900164 | 176 ms | 6.3 ms |
| 183 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 321 ns | 875 ns | 37 µs| 0% | 100% | 0:00:17.000191 | 27 ms | 1.6 ms |
| 171 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 332 ns | 849 ns | 37 µs| 0% | 100% | 0:00:15.999667 | 406 ms | 25 ms |
| 159 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 313 ns | 896 ns | 37 µs| 0% | 100% | 0:00:12.000786 | 191 ms | 16 ms |
| 1382 | Baseline | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 226 ns | 582 ns | 37 µs| 0% | 100% | 0:00:31.977796 | 60 ms | 1.9 ms |
| 981 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 378 ns | 1.1 µs | 20 µs| 0% | 99% | 0:00:11.000005 | 256 ms | 23 ms |
| 979 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 404 ns | 1.1 µs | 20 µs| 0% | 99% | 0:00:14.000009 | 430 ms | 31 ms |
| 1379 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 300 ns | 886 ns | 20 µs| 0% | 98% | 0:00:23.009755 | 2.1 µs | 92 ns |
| 997 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 380 ns | 1.1 µs | 20 µs| 0% | 100% | 0:00:13.000195 | 221 ms | 17 ms |
| 993 | Baseline | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 379 ns | 1.1 µs | 20 µs| 0% | 100% | 0:00:10.000169 | 751 ms | 75 ms |
| 25 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 35 µs | 75 µs| 0% | 12% | 0:04:10.968775 | 112 µs | 447 ns |
| 114 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 973 ns | 3.8 µs | 116 µs| 0% | 17% | 0:13:08.955002 | 28 ms | 35 µs |
| 22 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.8 µs | 22 µs | 74 µs| 0% | 16% | 0:03:51.982608 | 111 µs | 478 ns |
| 39 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 23 µs | 78 µs| 0% | 15% | 0:04:08.824369 | 111 µs | 446 ns |
| 980 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 3.0 µs | 10 µs | 43 µs| 0% | 8% | 0:00:58.918865 | 45 µs | 760 ns |
| 978 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 3.0 µs | 11 µs | 46 µs| 0% | 11% | 0:01:06.972782 | 49 µs | 730 ns |
| 1349 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.4 µs | 8.6 µs | 63 µs| 0% | 10% | 0:00:41.981530 | 49 µs | 1.2 µs |
| 986 | Baseline | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 3.4 µs | 13 µs | 46 µs| 0% | 9% | 0:00:42.927313 | 46 µs | 1.1 µs |
| 1019 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 2.0 µs | 7.1 µs | 40 µs| 0% | 99% | 0:00:16.007538 | 6.6 µs | 410 ns |
| 988 | Baseline | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.8 µs | 7.0 µs | 40 µs| 0% | 100% | 0:00:10 | 6.0 µs | 600 ns |
| 1374 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 298 ns | 871 ns | 20 µs| 0% | 96% | 0:00:14.006626 | 2.3 µs | 166 ns |
| 1313 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 2.0 µs | 12 µs | 195 µs| 0% | 97% | 0:00:10 | 27 µs | 2.7 µs |
| 977 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 376 ns | 1.1 µs | 42 µs| 0% | 76% | 0:00:23.282115 | 32 µs | 1.4 µs |
| 975 | Baseline | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 367 ns | 1.1 µs | 42 µs| 1% | 80% | 0:00:18.177229 | 16 µs | 891 ns |
| 163 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 332 ns | 909 ns | 37 µs| 0% | 100% | 0:00:12.001705 | 441 ms | 37 ms |
| 157 | Baseline | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 171 ns | 498 ns | 75 µs| 0% | 91% | 0:00:21.229092 | 5.6 µs | 262 ns |
| 1353 | Baseline | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 284 ns | 836 ns | 20 µs| 0% | 98% | 0:00:34.983769 | 700 ms | 20 ms |
| 147 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.6 µs | 7.3 µs | 67 µs| 0% | 100% | 0:00:12.000390 | 14 µs | 1.2 µs |
| 38 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.2 µs | 14 µs | 65 µs| 0% | 98% | 0:00:10 | 4.0 µs | 398 ns |
| 23 | Baseline | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.2 µs | 32 µs | 81 µs| 0% | 11% | 0:02:58.980162 | 113 µs | 632 ns |
| 164 | Baseline | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 506 ns | 1.7 µs | 78 µs| 0% | 100% | 0:00:15.008072 | 18 µs | 1.2 µs |
| 186 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.4 µs | 4.0 µs | 116 µs| 0% | 8% | 0:08:32.859443 | 462 µs | 902 ns |
| 182 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.2 µs | 3.6 µs | 116 µs| 0% | 7% | 0:04:15.949040 | 93 µs | 363 ns |
| 138 | Baseline | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 343 ns | 935 ns | 37 µs| 0% | 100% | 0:00:13.006646 | 49 ms | 3.8 ms |
| 166 | Baseline | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.1 µs | 3.8 µs | 116 µs| 0% | 7% | 0:04:13.938543 | 92 µs | 360 ns |
| 910 | Baseline | PTP4L | None | petalinux02 | PRIMARY_SLAVE | 7.5 µs | 21 µs | 38 µs| 0% | 99% | 0:00:52.000397 | 31 µs | 594 ns |
| 1520 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 3.6 µs | 15 µs | 62 µs| 0% | 98% | 0:00:11.000801 | 22 µs | 2.0 µs |
| 1521 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.7 µs | 21 µs | 238 µs| 0% | 96% | 0:00:10 | 59 µs | 5.9 µs |
| 1523 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 3.6 µs | 17 µs | 61 µs| 0% | 88% | 0:02:05.007737 | 44 µs | 352 ns |
| 1524 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.2 µs | 26 µs | 240 µs| 0% | 61% | 0:00:10.136730 | 100 µs | 9.9 µs |
| 1513 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.9 µs | 20 µs | 76 µs| 0% | 10% | 0:00:42.979076 | 64 µs | 1.5 µs |
| 1527 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 8.7 µs | 26 µs | 79 µs| 0% | 19% | 0:00:48.963136 | 81 µs | 1.7 µs |
| 1516 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 12 µs | 34 µs | 73 µs| 0% | 7% | 0:00:38.971990 | 66 µs | 1.7 µs |
| 1522 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 7.0 µs | 28 µs | 77 µs| 0% | 11% | 0:00:39.964005 | 70 µs | 1.8 µs |
| 1510 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 7.2 µs | 25 µs | 78 µs| 0% | 10% | 0:00:38.978068 | 66 µs | 1.7 µs |
| 1511 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 3.6 µs | 15 µs | 61 µs| 0% | 95% | 0:00:26.001763 | 33 µs | 1.3 µs |
| 1512 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.0 µs | 20 µs | 242 µs| 0% | 97% | 0:00:10 | 91 µs | 9.1 µs |
| 1525 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.9 µs | 20 µs | 76 µs| 0% | 9% | 0:01:02.938696 | 73 µs | 1.2 µs |
| 1526 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.5 µs | 16 µs | 63 µs| 0% | 98% | 0:00:10.000966 | 40 µs | 4.0 µs |
| 1514 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 3.5 µs | 15 µs | 61 µs| 0% | 98% | 0:00:10 | 28 µs | 2.8 µs |
| 1515 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.7 µs | 22 µs | 236 µs| 0% | 97% | 0:00:12.127169 | 31 µs | 2.5 µs |
| 1517 | Baseline | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 3.8 µs | 16 µs | 61 µs| 0% | 95% | 0:00:10 | 18 µs | 1.8 µs |
| 1518 | Baseline | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.1 µs | 21 µs | 242 µs| 0% | 98% | 0:00:14.143085 | 65 µs | 4.6 µs |
| 1519 | Baseline | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 7.0 µs | 22 µs | 77 µs| 0% | 15% | 0:00:38.971894 | 43 µs | 1.1 µs |
| 1949 | Baseline | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.6 µs | 67 µs| 0% | 100% | 0:00:10 | 14 µs | 1.4 µs |
| 1952 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 13 µs | 58 µs| 0% | 99% | 0:00:10.004007 | 26 µs | 2.6 µs |
| 1936 | Baseline | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.8 µs | 14 µs | 58 µs| 0% | 98% | 0:00:56.014406 | 66 µs | 1.2 µs |
| 1942 | Baseline | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.3 µs | 118 µs| 0% | 98% | 0:00:10.062374 | 19 µs | 1.9 µs |
### Benchmark: Test
_Id: `test/test`, 2 machines, 0:01:00 duration._

A test benchmark to quickly verify the cluster is working correctly. It is identical to the base benchmark but runs for a shorter duration.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Demo
_Id: `test/demo`, 2 machines, 0:05:00 duration._

A demo benchmark to quickly assess the capabilities of the cluster. It is identical to the base benchmark but runs for a shorter duration.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: 2 Nodes
_Id: `scalability/1_to_1`, 2 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 2 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1585 | 2 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.8 µs | 5.2 µs | 117 µs| 0% | 10% | 0:08:09.016092 | 312 µs | 638 ns |
| 1586 | 2 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 317 ns | 869 ns | 37 µs| 0% | 100% | 0:00:20.000788 | 572 ms | 29 ms |
| 1587 | 2 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 213 ns | 591 ns | 37 µs| 0% | 100% | 0:00:30.175627 | 41 ms | 1.4 ms |
| 1588 | 2 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 163 ns | 447 ns | 75 µs| 0% | 96% | 0:00:14.145742 | 4.8 µs | 341 ns |
### Benchmark: 3 Nodes
_Id: `scalability/1_to_2`, 3 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 3 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1582 | 3 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 341 ns | 870 ns | 37 µs| 0% | 100% | 0:00:10 | 174 ms | 17 ms |
| 1582 | 3 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 324 ns | 876 ns | 37 µs| 0% | 100% | 0:00:11.000764 | 693 ms | 63 ms |
| 1583 | 3 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 223 ns | 604 ns | 37 µs| 0% | 100% | 0:00:41.643478 | 806 ms | 19 ms |
| 1583 | 3 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 233 ns | 616 ns | 37 µs| 0% | 100% | 0:00:29.590440 | 343 ms | 12 ms |
| 1584 | 3 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 160 ns | 428 ns | 75 µs| 0% | 97% | 0:00:16.221399 | 12 µs | 750 ns |
| 1584 | 3 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 174 ns | 458 ns | 75 µs| 0% | 97% | 0:00:13.157336 | 55 µs | 4.2 µs |
| 1581 | 3 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.7 µs | 5.1 µs | 116 µs| 0% | 15% | 0:09:33.225867 | 1.3 ms | 2.3 µs |
| 1581 | 3 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 2.0 µs | 5.5 µs | 116 µs| 0% | 16% | 0:07:15.005611 | 314 µs | 723 ns |
### Benchmark: 12 Nodes
_Id: `scalability/1_to_11`, 12 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 12 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 337 ns | 849 ns | 37 µs| 0% | 99% | 0:00:10 | 400 ms | 40 ms |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 339 ns | 854 ns | 37 µs| 0% | 100% | 0:00:16.001224 | 697 ms | 44 ms |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 524 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:15.001132 | 5.2 µs | 344 ns |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 548 ns | 1.4 µs | 49 µs| 0% | 100% | 0:00:14.001054 | 5.0 µs | 360 ns |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 523 ns | 1.4 µs | 48 µs| 0% | 99% | 0:00:19.000729 | 18 µs | 939 ns |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 518 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:16.000785 | 16 µs | 1.0 µs |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 3.4 µs | 12 µs | 46 µs| 0% | 85% | 0:01:00.003577 | 22 µs | 370 ns |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 2.8 µs | 12 µs | 46 µs| 0% | 97% | 0:00:15.996082 | 7.4 µs | 465 ns |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.0 µs | 12 µs | 46 µs| 0% | 91% | 0:00:20.000038 | 11 µs | 567 ns |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 3.2 µs | 18 µs | 69 µs| 0% | 83% | 0:00:18.001179 | 25 µs | 1.4 µs |
| 1544 | 12 Nodes | PTP4L | Big Bad Cluster | bb-tk1-2 | TERTIARY_SLAVE | 3.6 µs | 18 µs | 69 µs| 0% | 78% | 0:01:01.002933 | 43 µs | 699 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 7.9 µs | 9.1 µs | 75 µs| 0% | 46% | 0:00:10 | 2.1 µs | 212 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 470 ns | 6.6 µs | 99 µs| 0% | 81% | 0:00:20.230517 | 1.7 µs | 83 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 911 ns | 3.9 µs | 93 µs| 0% | 78% | 0:00:13.165570 | 3.8 µs | 287 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 706 ns | 4.2 µs | 94 µs| 50% | 90% | 0:00:11.119562 | 4.4 µs | 400 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 432 ns | 1.4 µs | 99 µs| 0% | 78% | 0:00:10 | 1.5 µs | 148 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 550 ns | 8.7 µs | 99 µs| 0% | 63% | 0:00:10.107544 | 1.2 µs | 122 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 420 ns | 1.4 µs | 99 µs| 0% | 86% | 0:00:11.151382 | 1.3 µs | 116 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 742 ns | 3.9 µs | 94 µs| 0% | 88% | 0:00:14.098118 | 3.6 µs | 257 ns |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-2 | TERTIARY_SLAVE | 8.8 µs | 30 µs | 252 µs| 0% | 87% | 0:00:22.241992 | 52 µs | 2.4 µs |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 29 µs | 45 µs | 253 µs| 0% | 4% | 0:00:20.211066 | 83 µs | 4.1 µs |
| 1598 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 167 ns | 457 ns | 75 µs| 0% | 96% | 0:00:15.145002 | 987 ns | 65 ns |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 796 ns | 8.7 µs | 75 µs| 0.6% | 38% | 0:00:16.196026 | 45 µs | 2.8 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 486 ns | 8.2 µs | 99 µs| 0.6% | 69% | 0:00:21.236262 | 31 µs | 1.5 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 478 ns | 2.7 µs | 99 µs| 0% | 68% | 0:00:14.165622 | 18 µs | 1.3 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 450 ns | 7.0 µs | 99 µs| 0.6% | 78% | 0:00:22.194818 | 31 µs | 1.4 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.1 µs | 4.1 µs | 99 µs| 0.3% | 89% | 0:00:12.122333 | 23 µs | 1.9 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.2 µs | 4.5 µs | 95 µs| 0.8% | 76% | 0:00:16.200927 | 20 µs | 1.3 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 1.3 µs | 5.6 µs | 94 µs| 51% | 70% | 0:00:30.335064 | 19 µs | 615 ns |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 30 µs | 48 µs | 254 µs| 0.6% | 1.0% | 0:00:10 | 81 µs | 8.1 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 490 ns | 8.6 µs | 75 µs| 0% | 50% | 0:00:15.161147 | 1.1 µs | 71 ns |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 390 ns | 1.6 µs | 99 µs| 0.3% | 85% | 0:00:12.142731 | 31 µs | 2.6 µs |
| 1540 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-2 | TERTIARY_SLAVE | 4.4 µs | 41 µs | 184 µs| 0% | 25% | 0:00:10 | 82 µs | 8.2 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.4 µs | 4.4 µs | 113 µs| 0% | 15% | 0:08:29.917378 | 314 µs | 615 ns |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.2 µs | 4.0 µs | 113 µs| 0% | 14% | 0:08:54.011241 | 461 µs | 862 ns |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 5.3 µs | 17 µs | 99 µs| 0% | 11% | 0:06:37.000682 | 477 µs | 1.2 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 5.1 µs | 17 µs | 98 µs| 0% | 6% | 0:07:12.994771 | 467 µs | 1.1 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 5.3 µs | 17 µs | 98 µs| 0% | 6% | 0:07:04.994265 | 476 µs | 1.1 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 4.8 µs | 17 µs | 98 µs| 0% | 7% | 0:06:25.983864 | 483 µs | 1.3 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 4.2 µs | 13 µs | 86 µs| 0% | 15% | 0:07:12.004730 | 479 µs | 1.1 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.9 µs | 12 µs | 105 µs| 0% | 23% | 0:07:13.049626 | 572 µs | 1.3 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-tk1-2 | TERTIARY_SLAVE | 9.8 µs | 48 µs | 119 µs| 0% | 5% | 0:05:40.997646 | 508 µs | 1.5 µs |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 3.6 µs | 12 µs | 86 µs| 0% | 12% | 0:06:26.947325 | 282 µs | 728 ns |
| 1545 | 12 Nodes | PTPd | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 11 µs | 44 µs | 121 µs| 0% | 9% | 0:05:58.998181 | 541 µs | 1.5 µs |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 444 ns | 5.4 µs | 99 µs| 0% | 78% | 0:00:15.133128 | 29 µs | 1.9 µs |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.1 µs | 4.0 µs | 94 µs| 0% | 73% | 0:00:13.153441 | 20 µs | 1.6 µs |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-2 | TERTIARY_SLAVE | 31 µs | 46 µs | 257 µs| 0% | 1% | 0:01:43.255721 | 93 µs | 899 ns |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 7.6 µs | 8.9 µs | 75 µs| 0% | 47% | 0:00:12.132229 | 35 µs | 2.9 µs |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 841 ns | 4.8 µs | 94 µs| 0% | 78% | 0:00:21.304878 | 22 µs | 1.0 µs |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 497 ns | 8.4 µs | 99 µs| 0% | 66% | 0:00:20.261129 | 11 µs | 566 ns |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 468 ns | 2.3 µs | 99 µs| 0% | 73% | 0:00:25.288292 | 29 µs | 1.2 µs |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 446 ns | 8.7 µs | 75 µs| 0% | 51% | 0:00:10 | 2.9 µs | 288 ns |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 462 ns | 7.1 µs | 99 µs| 0% | 73% | 0:00:21.210115 | 31 µs | 1.4 µs |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.2 µs | 5.0 µs | 100 µs| 50% | 26% | 0:00:20.260375 | 20 µs | 964 ns |
| 2001 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 28 µs | 45 µs | 253 µs| 0% | 0% | 0:05:05.622927 | 114 µs | 374 ns |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 1.2 µs | 4.6 µs | 99 µs| 50% | 69% | 0:00:21.204450 | 22 µs | 1.0 µs |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 216 ns | 3.8 µs | 75 µs| 0% | 79% | 0:00:14.177339 | 33 µs | 2.3 µs |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 454 ns | 16 µs | 99 µs| 0% | 76% | 0:00:16.237852 | 10 µs | 642 ns |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 486 ns | 8.6 µs | 99 µs| 0% | 67% | 0:00:15.197230 | 12 µs | 805 ns |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 511 ns | 9.8 µs | 99 µs| 0% | 68% | 0:00:12.105608 | 30 µs | 2.5 µs |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.9 µs | 4.8 µs | 99 µs| 0% | 43% | 0:00:19.203674 | 23 µs | 1.2 µs |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 953 ns | 3.8 µs | 96 µs| 0% | 86% | 0:00:22.253596 | 22 µs | 992 ns |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 34 µs | 55 µs | 255 µs| 0% | 1% | 0:03:08.135477 | 86 µs | 457 ns |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-2 | TERTIARY_SLAVE | 27 µs | 43 µs | 253 µs| 0% | 0% | 0:18:24.944068 | 111 µs | 101 ns |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 250 ns | 9.1 µs | 75 µs| 0% | 70% | 0:00:14.182390 | 47 µs | 3.3 µs |
| 2003 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 476 ns | 15 µs | 99 µs| 0% | 78% | 0:00:19.190976 | 29 µs | 1.5 µs |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 398 ns | 1.4 µs | 99 µs| 0% | 81% | 0:00:18.180820 | 12 µs | 660 ns |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 410 ns | 7.0 µs | 99 µs| 0% | 81% | 0:00:22.244141 | 20 µs | 882 ns |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 477 ns | 10 µs | 99 µs| 0% | 75% | 0:00:15.152030 | 30 µs | 2.0 µs |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.5 µs | 6.1 µs | 100 µs| 50% | 42% | 0:00:19.250774 | 22 µs | 1.1 µs |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 251 ns | 9.2 µs | 75 µs| 0% | 66% | 0:00:14.151672 | 13 µs | 945 ns |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 4.9 µs | 8.6 µs | 75 µs| 0% | 45% | 0:00:17.190444 | 5.7 µs | 329 ns |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.8 µs | 5.6 µs | 98 µs| 0% | 50% | 0:00:27.393599 | 16 µs | 594 ns |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 2.2 µs | 6.9 µs | 99 µs| 0% | 32% | 0:00:18.199732 | 20 µs | 1.1 µs |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 6.9 µs | 44 µs | 187 µs| 0% | 12% | 0:03:00.175348 | 98 µs | 544 ns |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-tk1-2 | TERTIARY_SLAVE | 28 µs | 46 µs | 254 µs| 0% | 0% | 0:01:36.103101 | 96 µs | 1.0 µs |
| 2005 | 12 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 479 ns | 3.0 µs | 99 µs| 0% | 70% | 0:00:24.243514 | 10 µs | 429 ns |
### Benchmark: 4 Nodes
_Id: `scalability/1_to_3`, 4 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 4 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1577 | 4 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.8 µs | 5.1 µs | 115 µs| 0% | 12% | 0:07:42.995992 | 314 µs | 677 ns |
| 1577 | 4 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.9 µs | 5.3 µs | 115 µs| 0% | 7% | 0:08:28.011961 | 464 µs | 913 ns |
| 1577 | 4 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 6.4 µs | 18 µs | 103 µs| 0% | 16% | 0:05:55.103621 | 485 µs | 1.4 µs |
| 1600 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 161 ns | 417 ns | 75 µs| 0% | 94% | 0:00:13.117559 | 913 ns | 70 ns |
| 1600 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 160 ns | 440 ns | 75 µs| 0% | 96% | 0:00:11.136850 | 1.4 µs | 126 ns |
| 1600 | 4 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 366 ns | 1.2 µs | 99 µs| 0% | 84% | 0:00:11.123494 | 1.2 µs | 109 ns |
| 1611 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 149 ns | 406 ns | 75 µs| 0% | 97% | 0:00:19.213314 | 5.3 µs | 276 ns |
| 1611 | 4 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 382 ns | 1.1 µs | 99 µs| 0% | 83% | 0:00:20.240921 | 31 µs | 1.5 µs |
| 1611 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 170 ns | 501 ns | 75 µs| 9% | 89% | 0:01:08.756658 | 1.3 ms | 19 µs |
| 1578 | 4 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 340 ns | 927 ns | 37 µs| 0% | 100% | 0:00:13.003926 | 153 ms | 12 ms |
| 1578 | 4 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 339 ns | 921 ns | 37 µs| 0% | 100% | 0:00:14.000069 | 475 ms | 34 ms |
| 1578 | 4 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 516 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:12.000911 | 17 µs | 1.4 µs |
| 1579 | 4 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 221 ns | 618 ns | 37 µs| 0% | 100% | 0:00:27.978431 | 13 ms | 451 µs |
| 1579 | 4 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 332 ns | 902 ns | 49 µs| 0% | 100% | 0:00:12.003407 | 15 µs | 1.2 µs |
| 1579 | 4 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 201 ns | 590 ns | 37 µs| 0% | 100% | 0:00:24.905633 | 44 ms | 1.8 ms |
| 1870 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 150 ns | 434 ns | 75 µs| 0% | 99% | 0:00:17.179624 | 36 µs | 2.1 µs |
| 1870 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 160 ns | 436 ns | 75 µs| 0% | 99% | 0:00:21.226832 | 5.7 µs | 267 ns |
| 1870 | 4 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 397 ns | 1.1 µs | 99 µs| 0% | 83% | 0:00:15.163462 | 32 µs | 2.1 µs |
| 1871 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 162 ns | 426 ns | 75 µs| 0% | 97% | 0:00:22.251545 | 35 µs | 1.6 µs |
| 1871 | 4 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 416 ns | 1.3 µs | 99 µs| 0% | 82% | 0:00:24.314945 | 18 µs | 739 ns |
| 1871 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 152 ns | 426 ns | 75 µs| 0% | 97% | 0:00:13.184746 | 5.0 µs | 381 ns |
| 1875 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 302 ns | 8.5 µs | 75 µs| 0% | 64% | 0:00:19.218997 | 39 µs | 2.0 µs |
| 1875 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 313 ns | 8.6 µs | 75 µs| 0% | 61% | 0:00:18.163387 | 4.0 µs | 222 ns |
| 1875 | 4 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 415 ns | 1.2 µs | 99 µs| 0% | 82% | 0:00:20.180359 | 28 µs | 1.4 µs |
| 1874 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 162 ns | 452 ns | 75 µs| 0% | 97% | 0:00:19.225252 | 38 µs | 2.0 µs |
| 1874 | 4 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 395 ns | 1.2 µs | 99 µs| 0% | 86% | 0:00:13.138002 | 13 µs | 972 ns |
| 1874 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 160 ns | 440 ns | 75 µs| 0% | 97% | 0:00:29.340239 | 14 µs | 471 ns |
| 1876 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 156 ns | 458 ns | 75 µs| 0% | 96% | 0:00:16.221368 | 40 µs | 2.5 µs |
| 1876 | 4 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 172 ns | 501 ns | 75 µs| 0% | 96% | 0:00:11.106599 | 32 µs | 2.9 µs |
| 1876 | 4 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 377 ns | 1.1 µs | 99 µs| 0% | 86% | 0:00:12.122802 | 11 µs | 895 ns |
### Benchmark: 5 Nodes
_Id: `scalability/1_to_4`, 5 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 5 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1573 | 5 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.8 µs | 4.9 µs | 115 µs| 0% | 14% | 0:08:53.018534 | 463 µs | 870 ns |
| 1573 | 5 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.9 µs | 4.9 µs | 115 µs| 0% | 9% | 0:07:57.006471 | 547 µs | 1.1 µs |
| 1573 | 5 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 6.7 µs | 17 µs | 102 µs| 0% | 16% | 0:06:49.001321 | 479 µs | 1.2 µs |
| 1573 | 5 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 6.9 µs | 16 µs | 102 µs| 0% | 11% | 0:05:59.999179 | 266 µs | 740 ns |
| 1617 | 5 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 231 ns | 8.5 µs | 75 µs| 0% | 75% | 0:00:13.102140 | 929 ns | 71 ns |
| 1617 | 5 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 171 ns | 471 ns | 75 µs| 0% | 97% | 0:00:20.207013 | 1.2 µs | 61 ns |
| 1617 | 5 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 376 ns | 1.2 µs | 99 µs| 0% | 84% | 0:00:23.268278 | 36 µs | 1.6 µs |
| 1617 | 5 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 400 ns | 1.1 µs | 99 µs| 0% | 79% | 0:00:10 | 1.2 µs | 119 ns |
| 1574 | 5 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 334 ns | 933 ns | 37 µs| 0% | 100% | 0:00:13.000121 | 59 ms | 4.5 ms |
| 1574 | 5 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 334 ns | 947 ns | 37 µs| 0% | 100% | 0:00:10.999722 | 516 ms | 47 ms |
| 1574 | 5 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 517 ns | 1.5 µs | 49 µs| 0% | 100% | 0:00:17.001368 | 3.1 µs | 180 ns |
| 1574 | 5 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 530 ns | 1.5 µs | 49 µs| 0% | 100% | 0:00:13.001010 | 12 µs | 905 ns |
| 1575 | 5 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 208 ns | 609 ns | 37 µs| 0% | 100% | 0:00:34.946346 | 366 ms | 10 ms |
| 1575 | 5 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 354 ns | 975 ns | 49 µs| 0% | 100% | 0:00:13.004373 | 8.8 µs | 675 ns |
| 1575 | 5 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 213 ns | 608 ns | 37 µs| 0% | 100% | 0:00:20.919624 | 400 µs | 19 µs |
| 1575 | 5 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 342 ns | 975 ns | 49 µs| 0% | 100% | 0:00:12.002843 | 9.0 µs | 750 ns |
| 1576 | 5 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 166 ns | 450 ns | 75 µs| 0% | 94% | 0:00:13.138369 | 28 µs | 2.1 µs |
| 1576 | 5 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 377 ns | 1.1 µs | 99 µs| 0% | 82% | 0:00:11.119923 | 14 µs | 1.3 µs |
| 1576 | 5 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 168 ns | 460 ns | 75 µs| 0% | 97% | 0:00:11.084804 | 40 µs | 3.6 µs |
| 1576 | 5 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 372 ns | 1.1 µs | 99 µs| 0% | 86% | 0:00:12.124459 | 33 µs | 2.7 µs |
| 1877 | 5 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 170 ns | 549 ns | 75 µs| 0% | 95% | 0:00:14.175671 | 30 µs | 2.1 µs |
| 1877 | 5 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 422 ns | 1.6 µs | 99 µs| 0% | 82% | 0:00:13.149868 | 14 µs | 1.1 µs |
| 1877 | 5 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 407 ns | 1.6 µs | 99 µs| 0% | 78% | 0:00:15.133946 | 12 µs | 802 ns |
| 1877 | 5 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 290 ns | 8.8 µs | 75 µs| 0% | 63% | 0:00:14.166255 | 510 ns | 36 ns |
### Benchmark: 6 Nodes
_Id: `scalability/1_to_5`, 6 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 6 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1570 | 6 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 320 ns | 978 ns | 37 µs| 0% | 100% | 0:00:18.002051 | 43 ms | 2.4 ms |
| 1570 | 6 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 480 ns | 1.6 µs | 48 µs| 0% | 100% | 0:00:14.982080 | 36 µs | 2.4 µs |
| 1570 | 6 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 490 ns | 1.7 µs | 48 µs| 0% | 100% | 0:00:16.008963 | 40 µs | 2.5 µs |
| 1570 | 6 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 313 ns | 984 ns | 37 µs| 0% | 100% | 0:00:12.000942 | 243 ms | 20 ms |
| 1570 | 6 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 480 ns | 1.6 µs | 48 µs| 0% | 100% | 0:00:13.001322 | 32 µs | 2.5 µs |
| 1571 | 6 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 366 ns | 1.0 µs | 49 µs| 0% | 100% | 0:00:13.005974 | 12 µs | 960 ns |
| 1571 | 6 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 207 ns | 641 ns | 37 µs| 0% | 100% | 0:00:31.999393 | 403 ms | 13 ms |
| 1571 | 6 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 366 ns | 919 ns | 49 µs| 0% | 100% | 0:00:13.003897 | 15 µs | 1.1 µs |
| 1571 | 6 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 360 ns | 1.0 µs | 49 µs| 0% | 99% | 0:00:17.004342 | 13 µs | 772 ns |
| 1571 | 6 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 219 ns | 569 ns | 37 µs| 0% | 100% | 0:00:26.924760 | 50 ms | 1.9 ms |
| 1569 | 6 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 6.7 µs | 18 µs | 100 µs| 0% | 12% | 0:05:29.953710 | 268 µs | 811 ns |
| 1569 | 6 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.6 µs | 5.1 µs | 114 µs| 0% | 16% | 0:07:54.950665 | 311 µs | 656 ns |
| 1569 | 6 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.7 µs | 5.0 µs | 114 µs| 0% | 13% | 0:08:50.009226 | 461 µs | 871 ns |
| 1569 | 6 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 6.7 µs | 17 µs | 101 µs| 0% | 10% | 0:06:41.999778 | 481 µs | 1.2 µs |
| 1569 | 6 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 6.3 µs | 18 µs | 101 µs| 0% | 14% | 0:06:22.998501 | 464 µs | 1.2 µs |
| 1572 | 6 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 212 ns | 8.7 µs | 75 µs| 0% | 80% | 0:00:16.151724 | 4.8 µs | 294 ns |
| 1572 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 430 ns | 1.5 µs | 99 µs| 0% | 77% | 0:00:17.200396 | 30 µs | 1.7 µs |
| 1572 | 6 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 197 ns | 8.6 µs | 75 µs| 0% | 81% | 0:00:11.130993 | 38 µs | 3.4 µs |
| 1572 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 404 ns | 1.2 µs | 99 µs| 0% | 80% | 0:00:18.221317 | 18 µs | 998 ns |
| 1572 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 408 ns | 1.3 µs | 99 µs| 0% | 77% | 0:00:33.333139 | 28 µs | 854 ns |
| 1878 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 493 ns | 8.3 µs | 99 µs| 0% | 72% | 0:00:20.239028 | 37 µs | 1.8 µs |
| 1878 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 384 ns | 1.5 µs | 99 µs| 0% | 81% | 0:00:10 | 813 ns | 81 ns |
| 1878 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 462 ns | 9.0 µs | 99 µs| 0% | 73% | 0:00:28.374745 | 35 µs | 1.2 µs |
| 1878 | 6 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 219 ns | 8.5 µs | 75 µs| 0% | 75% | 0:00:22.245305 | 2.5 µs | 113 ns |
| 1878 | 6 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 155 ns | 442 ns | 75 µs| 0% | 97% | 0:00:14.170490 | 1.1 µs | 75 ns |
| 1880 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 420 ns | 2.2 µs | 99 µs| 0% | 78% | 0:00:14.190966 | 13 µs | 949 ns |
| 1880 | 6 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 173 ns | 487 ns | 75 µs| 0% | 94% | 0:00:14.178562 | 3.6 µs | 254 ns |
| 1880 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 389 ns | 1.2 µs | 99 µs| 0% | 80% | 0:01:29.961738 | 29 µs | 321 ns |
| 1880 | 6 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 392 ns | 1.2 µs | 99 µs| 0% | 75% | 0:00:16.209186 | 13 µs | 810 ns |
| 1880 | 6 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 215 ns | 8.6 µs | 75 µs| 0% | 78% | 0:00:10.129053 | 39 µs | 3.8 µs |
### Benchmark: 7 Nodes
_Id: `scalability/1_to_6`, 7 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 7 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1565 | 7 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 6.0 µs | 17 µs | 100 µs| 0% | 14% | 0:06:15.000441 | 389 µs | 1.0 µs |
| 1565 | 7 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.7 µs | 5.2 µs | 114 µs| 0% | 11% | 0:08:17.010917 | 461 µs | 927 ns |
| 1565 | 7 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 6.4 µs | 17 µs | 100 µs| 0% | 11% | 0:06:44.001576 | 463 µs | 1.1 µs |
| 1565 | 7 Nodes | PTPd | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 6.4 µs | 15 µs | 100 µs| 0% | 9% | 0:06:28.000760 | 492 µs | 1.3 µs |
| 1565 | 7 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.6 µs | 4.5 µs | 114 µs| 0% | 14% | 0:09:35.973181 | 1.2 ms | 2.0 µs |
| 1565 | 7 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 6.6 µs | 17 µs | 100 µs| 0% | 10% | 0:06:27.001385 | 484 µs | 1.3 µs |
| 1567 | 7 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 223 ns | 618 ns | 37 µs| 0% | 100% | 0:00:35.933027 | 897 ms | 25 ms |
| 1567 | 7 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 319 ns | 888 ns | 49 µs| 0% | 100% | 0:00:13.002747 | 14 µs | 1.1 µs |
| 1567 | 7 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 324 ns | 936 ns | 49 µs| 0% | 100% | 0:00:16.006216 | 11 µs | 713 ns |
| 1567 | 7 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 332 ns | 910 ns | 49 µs| 0% | 100% | 0:00:16.004705 | 13 µs | 808 ns |
| 1567 | 7 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 340 ns | 962 ns | 49 µs| 0% | 100% | 0:00:17.005606 | 14 µs | 810 ns |
| 1567 | 7 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 213 ns | 604 ns | 37 µs| 0% | 100% | 0:00:34.949646 | 449 ms | 13 ms |
| 1568 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 383 ns | 1.3 µs | 99 µs| 0% | 85% | 0:00:20.231083 | 1.5 µs | 72 ns |
| 1568 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 370 ns | 1.1 µs | 99 µs| 0% | 85% | 0:00:10 | 1.8 µs | 180 ns |
| 1568 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 416 ns | 8.0 µs | 99 µs| 0% | 84% | 0:00:12.169697 | 1.0 µs | 83 ns |
| 1568 | 7 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 184 ns | 8.4 µs | 75 µs| 0% | 85% | 0:00:13.135537 | 1.6 µs | 122 ns |
| 1568 | 7 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 267 ns | 8.3 µs | 75 µs| 0% | 68% | 0:00:10.099029 | 33 µs | 3.3 µs |
| 1568 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 412 ns | 1.6 µs | 99 µs| 0% | 84% | 0:00:12.160605 | 688 ns | 57 ns |
| 1566 | 7 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 465 ns | 1.6 µs | 48 µs| 0% | 100% | 0:00:17.001425 | 9.1 µs | 533 ns |
| 1566 | 7 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 474 ns | 1.6 µs | 48 µs| 0% | 100% | 0:00:16.001336 | 5.0 µs | 310 ns |
| 1566 | 7 Nodes | PTP4L | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 481 ns | 1.6 µs | 48 µs| 0% | 100% | 0:00:12.000969 | 3.4 µs | 281 ns |
| 1566 | 7 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 327 ns | 938 ns | 37 µs| 0% | 100% | 0:00:13.000919 | 664 ms | 51 ms |
| 1566 | 7 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 324 ns | 964 ns | 37 µs| 0% | 100% | 0:00:10.997672 | 409 µs | 37 µs |
| 1566 | 7 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 453 ns | 1.6 µs | 48 µs| 0% | 100% | 0:00:19.001334 | 9.6 µs | 504 ns |
| 1879 | 7 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 165 ns | 448 ns | 75 µs| 0% | 97% | 0:00:10 | 8.0 µs | 798 ns |
| 1879 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 444 ns | 8.5 µs | 99 µs| 0% | 77% | 0:00:15.179399 | 32 µs | 2.1 µs |
| 1879 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 454 ns | 2.9 µs | 99 µs| 0% | 76% | 0:00:27.346082 | 18 µs | 642 ns |
| 1879 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 604 ns | 7.5 µs | 99 µs| 0% | 61% | 0:00:44.532069 | 20 µs | 441 ns |
| 1879 | 7 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 198 ns | 8.5 µs | 75 µs| 0% | 83% | 0:00:12.108574 | 21 µs | 1.7 µs |
| 1879 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 442 ns | 1.6 µs | 99 µs| 0% | 78% | 0:00:21.271182 | 20 µs | 917 ns |
| 1881 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 424 ns | 1.7 µs | 99 µs| 0% | 75% | 0:00:21.235746 | 14 µs | 643 ns |
| 1881 | 7 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 205 ns | 8.9 µs | 75 µs| 0% | 82% | 0:00:16.156921 | 42 µs | 2.6 µs |
| 1881 | 7 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 161 ns | 445 ns | 75 µs| 0% | 94% | 0:00:17.183004 | 6.0 µs | 346 ns |
| 1881 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 418 ns | 7.8 µs | 99 µs| 0% | 77% | 0:00:16.203879 | 22 µs | 1.4 µs |
| 1881 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 401 ns | 1.2 µs | 99 µs| 0% | 85% | 0:00:12.165470 | 14 µs | 1.2 µs |
| 1881 | 7 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 396 ns | 1.2 µs | 99 µs| 0% | 81% | 0:00:21.247462 | 30 µs | 1.4 µs |
### Benchmark: 8 Nodes
_Id: `scalability/1_to_7`, 8 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 8 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1618 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 410 ns | 1.3 µs | 99 µs| 0% | 87% | 0:00:15.162119 | 16 µs | 1.1 µs |
| 1618 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 426 ns | 8.3 µs | 99 µs| 0% | 73% | 0:00:13.151532 | 30 µs | 2.2 µs |
| 1618 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 239 ns | 8.5 µs | 75 µs| 0% | 70% | 0:00:14.176086 | 42 µs | 3.0 µs |
| 1618 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 2.0 µs | 5.0 µs | 95 µs| 0% | 22% | 0:00:23.278438 | 22 µs | 945 ns |
| 1618 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 382 ns | 1.1 µs | 99 µs| 0% | 87% | 0:00:25.313436 | 30 µs | 1.2 µs |
| 1618 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 467 ns | 7.7 µs | 99 µs| 0% | 73% | 0:00:17.165052 | 17 µs | 991 ns |
| 1618 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 177 ns | 489 ns | 75 µs| 0% | 93% | 0:00:17.203843 | 4.7 µs | 271 ns |
| 1619 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 459 ns | 8.1 µs | 99 µs| 0% | 79% | 0:00:15.175111 | 30 µs | 2.0 µs |
| 1619 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 431 ns | 2.0 µs | 99 µs| 0% | 79% | 0:00:11.123771 | 12 µs | 1.1 µs |
| 1619 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 453 ns | 5.3 µs | 99 µs| 0% | 81% | 0:00:27.304065 | 16 µs | 574 ns |
| 1619 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.4 µs | 4.4 µs | 94 µs| 0% | 41% | 0:00:29.369701 | 22 µs | 758 ns |
| 1619 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 586 ns | 9.3 µs | 99 µs| 0% | 65% | 0:01:32.897980 | 18 µs | 196 ns |
| 1619 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 154 ns | 448 ns | 75 µs| 0% | 97% | 0:00:10.117198 | 33 µs | 3.3 µs |
| 1619 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 213 ns | 8.6 µs | 75 µs| 0% | 79% | 0:00:26.319071 | 5.5 µs | 209 ns |
| 1561 | 8 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.5 µs | 4.8 µs | 114 µs| 0% | 10% | 0:08:40.031500 | 311 µs | 597 ns |
| 1561 | 8 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 6.2 µs | 17 µs | 100 µs| 0% | 7% | 0:06:47.003296 | 476 µs | 1.2 µs |
| 1561 | 8 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 5.7 µs | 17 µs | 100 µs| 0% | 14% | 0:06:40.953489 | 483 µs | 1.2 µs |
| 1561 | 8 Nodes | PTPd | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 6.0 µs | 15 µs | 100 µs| 0% | 10% | 0:06:44.954098 | 495 µs | 1.2 µs |
| 1561 | 8 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.5 µs | 5.6 µs | 114 µs| 0% | 10% | 0:08:03.010017 | 460 µs | 953 ns |
| 1561 | 8 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 5.5 µs | 15 µs | 100 µs| 0% | 9% | 0:07:21.947729 | 457 µs | 1.0 µs |
| 1561 | 8 Nodes | PTPd | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 4.4 µs | 14 µs | 88 µs| 0% | 12% | 0:07:05.998042 | 479 µs | 1.1 µs |
| 1562 | 8 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 347 ns | 1.1 µs | 37 µs| 0% | 100% | 0:00:15.001238 | 474 ms | 32 ms |
| 1562 | 8 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 483 ns | 1.9 µs | 48 µs| 0% | 100% | 0:00:22.001078 | 12 µs | 531 ns |
| 1562 | 8 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 506 ns | 2.0 µs | 48 µs| 0% | 99% | 0:00:19.001123 | 8.1 µs | 424 ns |
| 1562 | 8 Nodes | PTP4L | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 3.0 µs | 16 µs | 46 µs| 0% | 97% | 0:00:17.066791 | 13 µs | 738 ns |
| 1562 | 8 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 363 ns | 1.0 µs | 37 µs| 0% | 99% | 0:00:10 | 341 ms | 34 ms |
| 1562 | 8 Nodes | PTP4L | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 492 ns | 1.8 µs | 48 µs| 0% | 98% | 0:00:13.001076 | 5.2 µs | 399 ns |
| 1562 | 8 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 492 ns | 2.0 µs | 48 µs| 0% | 99% | 0:00:17.001768 | 5.5 µs | 323 ns |
| 1564 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 206 ns | 8.3 µs | 75 µs| 0% | 82% | 0:00:19.213203 | 10 µs | 524 ns |
| 1564 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 166 ns | 477 ns | 75 µs| 0% | 95% | 0:00:15.213993 | 4.0 µs | 266 ns |
| 1564 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 384 ns | 1.3 µs | 99 µs| 0% | 87% | 0:00:18.222068 | 17 µs | 953 ns |
| 1564 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 390 ns | 1.3 µs | 99 µs| 0% | 86% | 0:00:27.339420 | 30 µs | 1.1 µs |
| 1564 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 548 ns | 15 µs | 99 µs| 0% | 69% | 0:00:22.292282 | 17 µs | 769 ns |
| 1564 | 8 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 2.1 µs | 5.2 µs | 99 µs| 0% | 43% | 0:00:23.259138 | 23 µs | 989 ns |
| 1564 | 8 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 400 ns | 1.2 µs | 99 µs| 0% | 82% | 0:00:17.203243 | 14 µs | 794 ns |
| 1563 | 8 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.6 µs | 6.2 µs | 55 µs| 0% | 100% | 0:00:13.005203 | 27 µs | 2.1 µs |
| 1563 | 8 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 207 ns | 596 ns | 37 µs| 0% | 100% | 0:00:36.944671 | 771 ms | 21 ms |
| 1563 | 8 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 344 ns | 991 ns | 49 µs| 0% | 100% | 0:00:17.003724 | 9.1 µs | 533 ns |
| 1563 | 8 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 216 ns | 583 ns | 37 µs| 0% | 100% | 0:00:31.968513 | 103 ms | 3.2 ms |
| 1563 | 8 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 330 ns | 924 ns | 49 µs| 0% | 100% | 0:00:14.002840 | 14 µs | 1.0 µs |
| 1563 | 8 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 339 ns | 937 ns | 49 µs| 0% | 100% | 0:00:14.003340 | 13 µs | 910 ns |
| 1563 | 8 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 351 ns | 996 ns | 49 µs| 0% | 100% | 0:00:14.003449 | 11 µs | 777 ns |
### Benchmark: 9 Nodes
_Id: `scalability/1_to_8`, 9 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 9 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 413 ns | 1.7 µs | 99 µs| 0% | 85% | 0:00:16.183434 | 13 µs | 797 ns |
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 438 ns | 4.0 µs | 99 µs| 0% | 80% | 0:00:20.212788 | 29 µs | 1.4 µs |
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.5 µs | 4.7 µs | 93 µs| 0% | 24% | 0:00:16.176152 | 22 µs | 1.4 µs |
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 2.0 µs | 5.3 µs | 100 µs| 0% | 44% | 0:00:21.253378 | 21 µs | 969 ns |
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 193 ns | 7.9 µs | 75 µs| 0% | 87% | 0:00:13.142280 | 22 µs | 1.7 µs |
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 403 ns | 1.2 µs | 99 µs| 0% | 86% | 0:00:17.206038 | 31 µs | 1.8 µs |
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 201 ns | 8.5 µs | 75 µs| 0% | 83% | 0:00:24.213192 | 7.1 µs | 292 ns |
| 1620 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 418 ns | 2.8 µs | 99 µs| 0% | 80% | 0:00:20.185144 | 32 µs | 1.6 µs |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.4 µs | 4.0 µs | 114 µs| 0% | 11% | 0:08:28.998298 | 313 µs | 615 ns |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.4 µs | 4.0 µs | 114 µs| 0% | 9% | 0:08:34.929651 | 465 µs | 903 ns |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 5.4 µs | 16 µs | 100 µs| 0% | 10% | 0:06:38.948967 | 481 µs | 1.2 µs |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 5.7 µs | 17 µs | 99 µs| 0% | 9% | 0:06:44.965860 | 481 µs | 1.2 µs |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 5.6 µs | 16 µs | 100 µs| 0% | 10% | 0:07:21.951491 | 467 µs | 1.1 µs |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 5.3 µs | 16 µs | 100 µs| 0% | 6% | 0:06:36.948958 | 477 µs | 1.2 µs |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 4.8 µs | 13 µs | 88 µs| 0% | 12% | 0:06:59.997186 | 478 µs | 1.1 µs |
| 1557 | 9 Nodes | PTPd | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 4.3 µs | 12 µs | 88 µs| 0% | 12% | 0:06:27.991438 | 279 µs | 718 ns |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 326 ns | 884 ns | 37 µs| 0% | 100% | 0:00:10.000827 | 135 ms | 13 ms |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 323 ns | 893 ns | 37 µs| 0% | 100% | 0:00:16.001156 | 389 ms | 24 ms |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 442 ns | 1.3 µs | 48 µs| 0% | 98% | 0:00:10.000832 | 2.2 µs | 222 ns |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 414 ns | 1.3 µs | 48 µs| 0% | 100% | 0:00:18.001371 | 6.7 µs | 371 ns |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 433 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:12.000460 | 6.4 µs | 537 ns |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 418 ns | 1.3 µs | 48 µs| 0% | 100% | 0:00:14.000760 | 3.0 µs | 215 ns |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 3.7 µs | 15 µs | 47 µs| 0% | 94% | 0:00:10 | 13 µs | 1.3 µs |
| 1558 | 9 Nodes | PTP4L | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 3.1 µs | 13 µs | 47 µs| 0% | 96% | 0:00:21.003111 | 21 µs | 1.0 µs |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 448 ns | 7.4 µs | 99 µs| 0% | 74% | 0:00:13.152222 | 18 µs | 1.4 µs |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 420 ns | 7.7 µs | 99 µs| 0% | 81% | 0:00:14.188408 | 27 µs | 1.9 µs |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 932 ns | 3.7 µs | 97 µs| 0% | 82% | 0:00:20.239612 | 21 µs | 1.0 µs |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 236 ns | 8.5 µs | 75 µs| 0% | 79% | 0:00:19.207395 | 1.4 µs | 73 ns |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 306 ns | 8.7 µs | 75 µs| 0% | 61% | 0:00:10 | 13 µs | 1.3 µs |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 508 ns | 8.8 µs | 99 µs| 0% | 65% | 0:00:27.373750 | 28 µs | 1.0 µs |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.7 µs | 5.1 µs | 93 µs| 0% | 34% | 0:00:18.210979 | 19 µs | 1.0 µs |
| 1560 | 9 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 460 ns | 3.0 µs | 99 µs| 0% | 74% | 0:00:20.234073 | 17 µs | 859 ns |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 202 ns | 575 ns | 37 µs| 0% | 100% | 0:00:28.912441 | 268 ms | 9.3 ms |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 222 ns | 581 ns | 37 µs| 0% | 100% | 0:00:33.999467 | 491 ms | 14 ms |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 308 ns | 873 ns | 49 µs| 0% | 100% | 0:00:16.004851 | 13 µs | 836 ns |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 303 ns | 941 ns | 49 µs| 0% | 100% | 0:00:16.004286 | 13 µs | 802 ns |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 311 ns | 901 ns | 49 µs| 0% | 98% | 0:00:16.005589 | 14 µs | 904 ns |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 341 ns | 930 ns | 49 µs| 0% | 98% | 0:00:23.007877 | 12 µs | 532 ns |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.7 µs | 7.8 µs | 55 µs| 0% | 100% | 0:00:16.007075 | 21 µs | 1.3 µs |
| 1559 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.7 µs | 8.2 µs | 55 µs| 0% | 100% | 0:00:12.055867 | 11 µs | 931 ns |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 343 ns | 982 ns | 49 µs| 0% | 100% | 0:00:16.007829 | 13 µs | 797 ns |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.3 µs | 6.9 µs | 55 µs| 0% | 100% | 0:00:11.006065 | 44 µs | 4.0 µs |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.5 µs | 7.8 µs | 55 µs| 0% | 100% | 0:00:12.009237 | 22 µs | 1.8 µs |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 211 ns | 587 ns | 37 µs| 0% | 100% | 0:00:26.995430 | 25 ms | 929 µs |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 356 ns | 979 ns | 49 µs| 0% | 100% | 0:00:13.005774 | 14 µs | 1.1 µs |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 333 ns | 966 ns | 49 µs| 0% | 100% | 0:00:18.004388 | 9.6 µs | 534 ns |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 355 ns | 1.0 µs | 49 µs| 0% | 99% | 0:00:13.006877 | 11 µs | 832 ns |
| 1929 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 212 ns | 593 ns | 37 µs| 0% | 100% | 0:00:27.974875 | 46 ms | 1.7 ms |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.4 µs | 8.1 µs | 55 µs| 0% | 100% | 0:00:13.005624 | 14 µs | 1.1 µs |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 338 ns | 929 ns | 49 µs| 0% | 100% | 0:00:12.027139 | 8.2 µs | 679 ns |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 213 ns | 589 ns | 37 µs| 0% | 100% | 0:00:26.998314 | 385 ms | 14 ms |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 224 ns | 619 ns | 37 µs| 0% | 100% | 0:00:25.936432 | 76 ms | 2.9 ms |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 345 ns | 996 ns | 49 µs| 0% | 100% | 0:00:15.004164 | 13 µs | 848 ns |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 334 ns | 943 ns | 49 µs| 0% | 100% | 0:00:13.002864 | 14 µs | 1.0 µs |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.4 µs | 6.7 µs | 55 µs| 0% | 100% | 0:00:19.010729 | 42 µs | 2.2 µs |
| 1930 | 9 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 330 ns | 953 ns | 49 µs| 0% | 99% | 0:00:13.004705 | 15 µs | 1.1 µs |
### Benchmark: 10 Nodes
_Id: `scalability/1_to_9`, 10 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 10 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 204 ns | 575 ns | 37 µs| 0% | 100% | 0:00:29.907977 | 274 ms | 9.1 ms |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 341 ns | 1.0 µs | 49 µs| 0% | 99% | 0:00:13.003705 | 14 µs | 1.1 µs |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 351 ns | 997 ns | 49 µs| 0% | 100% | 0:00:20.005361 | 12 µs | 611 ns |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.3 µs | 6.6 µs | 55 µs| 0% | 100% | 0:00:17.023545 | 12 µs | 700 ns |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 345 ns | 1.0 µs | 49 µs| 0% | 100% | 0:00:19.005128 | 13 µs | 662 ns |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 345 ns | 1.0 µs | 49 µs| 0% | 100% | 0:00:17.006259 | 8.1 µs | 478 ns |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.3 µs | 18 ms | 55 µs| 50% | 71% | 0:00:17.007243 | 27 µs | 1.6 µs |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 211 ns | 634 ns | 37 µs| 0% | 100% | 0:00:28.973956 | 148 ms | 5.1 ms |
| 1610 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.4 µs | 7.4 µs | 55 µs| 0% | 100% | 0:00:14.010454 | 13 µs | 949 ns |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 350 ns | 953 ns | 49 µs| 0% | 100% | 0:00:15.002325 | 13 µs | 876 ns |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 346 ns | 1.0 µs | 49 µs| 0% | 100% | 0:00:15.007622 | 14 µs | 910 ns |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 206 ns | 597 ns | 37 µs| 0% | 100% | 0:00:33.915342 | 418 ms | 12 ms |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 344 ns | 973 ns | 49 µs| 0% | 100% | 0:00:13.004984 | 15 µs | 1.2 µs |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 357 ns | 958 ns | 49 µs| 0% | 100% | 0:00:19.005967 | 12 µs | 628 ns |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.6 µs | 7.2 µs | 55 µs| 0% | 100% | 0:00:13.978564 | 22 µs | 1.5 µs |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.5 µs | 7.3 µs | 55 µs| 0% | 100% | 0:00:14.064336 | 12 µs | 859 ns |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 215 ns | 629 ns | 37 µs| 0% | 100% | 0:00:41.966700 | 955 ms | 23 ms |
| 1601 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.1 µs | 18 ms | 55 µs| 50% | 74% | 0:00:20.011538 | 20 µs | 987 ns |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 207 ns | 590 ns | 37 µs| 0% | 100% | 0:00:43.918876 | 922 ms | 21 ms |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 214 ns | 611 ns | 37 µs| 0% | 100% | 0:00:34.976269 | 436 ms | 12 ms |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 335 ns | 906 ns | 49 µs| 0% | 100% | 0:00:17.003536 | 8.6 µs | 504 ns |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 323 ns | 932 ns | 49 µs| 0% | 100% | 0:00:21.006879 | 13 µs | 597 ns |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 332 ns | 947 ns | 49 µs| 0% | 100% | 0:00:17.008533 | 9.0 µs | 527 ns |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 339 ns | 926 ns | 49 µs| 0% | 100% | 0:00:15.000758 | 11 µs | 730 ns |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.5 µs | 7.7 µs | 55 µs| 0% | 100% | 0:00:13.009467 | 22 µs | 1.7 µs |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.5 µs | 7.4 µs | 55 µs| 0% | 100% | 0:00:11.008805 | 13 µs | 1.2 µs |
| 1555 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.3 µs | 18 ms | 54 µs| 50% | 77% | 0:00:13.005939 | 19 µs | 1.5 µs |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 5.0 µs | 17 µs | 99 µs| 0% | 10% | 0:07:22.926676 | 479 µs | 1.1 µs |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 5.8 µs | 17 µs | 99 µs| 0% | 11% | 0:07:12.926243 | 466 µs | 1.1 µs |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 5.1 µs | 17 µs | 99 µs| 0% | 11% | 0:07:23.684018 | 490 µs | 1.1 µs |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 4.2 µs | 12 µs | 87 µs| 0% | 13% | 0:07:05.121426 | 477 µs | 1.1 µs |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 3.8 µs | 12 µs | 86 µs| 0% | 11% | 0:06:47.191031 | 278 µs | 682 ns |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.5 µs | 5.4 µs | 113 µs| 0% | 11% | 0:08:29.213242 | 314 µs | 617 ns |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.6 µs | 5.8 µs | 113 µs| 0% | 8% | 0:08:45.617354 | 465 µs | 885 ns |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 5.0 µs | 16 µs | 98 µs| 0% | 8% | 0:06:46.681609 | 461 µs | 1.1 µs |
| 1553 | 10 Nodes | PTPd | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.6 µs | 12 µs | 105 µs| 0% | 29% | 0:08:17.818953 | 1.1 ms | 2.3 µs |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 284 ns | 8.6 µs | 75 µs| 0% | 65% | 0:00:17.177132 | 6.5 µs | 381 ns |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 502 ns | 16 µs | 99 µs| 0% | 74% | 0:00:16.150748 | 11 µs | 701 ns |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 394 ns | 3.5 µs | 99 µs| 0% | 82% | 0:00:28.296011 | 31 µs | 1.1 µs |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 2.6 µs | 5.4 µs | 100 µs| 0% | 8% | 0:01:28.963688 | 16 µs | 183 ns |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 750 ns | 4.9 µs | 93 µs| 50% | 86% | 0:00:14.148790 | 19 µs | 1.4 µs |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 193 ns | 1.2 µs | 75 µs| 0% | 82% | 0:00:14.196854 | 38 µs | 2.7 µs |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 406 ns | 1.9 µs | 99 µs| 0% | 83% | 0:00:21.184716 | 31 µs | 1.5 µs |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 386 ns | 3.0 µs | 99 µs| 0% | 83% | 0:00:39.396949 | 31 µs | 794 ns |
| 1556 | 10 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.0 µs | 3.9 µs | 95 µs| 0% | 82% | 0:00:16.200864 | 23 µs | 1.4 µs |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 451 ns | 1.3 µs | 48 µs| 0% | 100% | 0:00:15.001533 | 11 µs | 751 ns |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 444 ns | 1.4 µs | 49 µs| 0% | 100% | 0:00:12.000434 | 3.9 µs | 326 ns |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 454 ns | 1.4 µs | 49 µs| 0% | 100% | 0:00:13.000773 | 14 µs | 1.1 µs |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 3.5 µs | 15 µs | 47 µs| 0% | 92% | 0:00:49.004700 | 34 µs | 702 ns |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.4 µs | 13 µs | 47 µs| 0% | 89% | 0:00:15.997825 | 16 µs | 1.0 µs |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 304 ns | 841 ns | 37 µs| 0% | 100% | 0:00:14.001454 | 46 ms | 3.3 ms |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 297 ns | 849 ns | 37 µs| 0% | 99% | 0:00:10.998957 | 497 ms | 45 ms |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 455 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:17.001515 | 5.7 µs | 336 ns |
| 1554 | 10 Nodes | PTP4L | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 2.8 µs | 14 µs | 46 µs| 0% | 89% | 0:00:12.203715 | 15 µs | 1.2 µs |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 346 ns | 999 ns | 49 µs| 0% | 99% | 0:00:11.001444 | 9.0 µs | 814 ns |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 203 ns | 592 ns | 37 µs| 0% | 100% | 0:00:40.944479 | 872 ms | 21 ms |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 343 ns | 1.2 µs | 49 µs| 0% | 98% | 0:00:13.004265 | 14 µs | 1.1 µs |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 351 ns | 986 ns | 49 µs| 0% | 100% | 0:00:20.006066 | 15 µs | 736 ns |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 350 ns | 977 ns | 49 µs| 0% | 100% | 0:00:18.006564 | 8.9 µs | 492 ns |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.4 µs | 6.5 µs | 55 µs| 0% | 100% | 0:00:15.011613 | 16 µs | 1.1 µs |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.6 µs | 18 ms | 55 µs| 50% | 72% | 0:00:15.003783 | 21 µs | 1.4 µs |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 218 ns | 609 ns | 37 µs| 0% | 100% | 0:00:25.991469 | 139 ms | 5.4 ms |
| 1872 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.5 µs | 7.2 µs | 55 µs| 0% | 100% | 0:00:12.007640 | 13 µs | 1.1 µs |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.4 µs | 7.4 µs | 54 µs| 0% | 100% | 0:00:12.991890 | 30 µs | 2.3 µs |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 214 ns | 608 ns | 37 µs| 0% | 100% | 0:00:41.006226 | 854 ms | 21 ms |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 226 ns | 620 ns | 37 µs| 0% | 100% | 0:00:29.987681 | 309 ms | 10 ms |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 336 ns | 933 ns | 49 µs| 0% | 100% | 0:00:20.005294 | 14 µs | 713 ns |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 344 ns | 990 ns | 49 µs| 0% | 100% | 0:00:16.006130 | 14 µs | 872 ns |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 355 ns | 929 ns | 49 µs| 0% | 100% | 0:00:13.005462 | 13 µs | 969 ns |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.4 µs | 7.8 µs | 55 µs| 0% | 100% | 0:00:17.010252 | 21 µs | 1.2 µs |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 4.0 µs | 18 ms | 55 µs| 50% | 71% | 0:00:17.962567 | 18 µs | 975 ns |
| 1873 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 348 ns | 981 ns | 49 µs| 0% | 100% | 0:00:21.007894 | 13 µs | 614 ns |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.4 µs | 7.4 µs | 55 µs| 0% | 100% | 0:00:17.006814 | 44 µs | 2.6 µs |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 214 ns | 589 ns | 37 µs| 0% | 100% | 0:00:41.992031 | 885 ms | 21 ms |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 225 ns | 605 ns | 37 µs| 0% | 100% | 0:00:30.990976 | 381 ms | 12 ms |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 338 ns | 959 ns | 49 µs| 0% | 100% | 0:00:17.005172 | 14 µs | 835 ns |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 320 ns | 977 ns | 49 µs| 0% | 100% | 0:00:14.005326 | 12 µs | 847 ns |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.5 µs | 7.9 µs | 55 µs| 0% | 100% | 0:00:21.866179 | 16 µs | 725 ns |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.8 µs | 18 ms | 55 µs| 50% | 76% | 0:00:13.987945 | 23 µs | 1.6 µs |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 322 ns | 952 ns | 49 µs| 0% | 100% | 0:00:16.005190 | 14 µs | 901 ns |
| 1931 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 321 ns | 941 ns | 49 µs| 0% | 100% | 0:00:22.009878 | 13 µs | 608 ns |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.6 µs | 18 ms | 55 µs| 50% | 74% | 0:00:13.014741 | 24 µs | 1.9 µs |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 220 ns | 611 ns | 37 µs| 0% | 100% | 0:00:33.924774 | 582 ms | 17 ms |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 204 ns | 585 ns | 37 µs| 0% | 100% | 0:00:35.118517 | 307 ms | 8.7 ms |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 324 ns | 903 ns | 49 µs| 0% | 100% | 0:00:14.006494 | 12 µs | 852 ns |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 355 ns | 1.0 µs | 49 µs| 0% | 100% | 0:00:22.007737 | 14 µs | 639 ns |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.3 µs | 7.5 µs | 55 µs| 0% | 100% | 0:00:11.004634 | 54 µs | 4.9 µs |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.5 µs | 7.3 µs | 55 µs| 0% | 100% | 0:00:17.007290 | 13 µs | 747 ns |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 346 ns | 959 ns | 49 µs| 0% | 99% | 0:00:18.005536 | 14 µs | 758 ns |
| 1932 | 10 Nodes | SPTP | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 321 ns | 990 ns | 49 µs| 0% | 100% | 0:00:14.002422 | 11 µs | 820 ns |
### Benchmark: 11 Nodes
_Id: `scalability/1_to_10`, 11 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 11 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 386 ns | 8.7 µs | 75 µs| 0% | 56% | 0:00:16.173049 | 1.3 µs | 82 ns |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 412 ns | 1.3 µs | 99 µs| 0% | 81% | 0:00:10.098760 | 32 µs | 3.2 µs |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 552 ns | 7.8 µs | 99 µs| 0% | 63% | 0:00:17.229642 | 19 µs | 1.1 µs |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 493 ns | 17 µs | 99 µs| 0% | 71% | 0:00:18.171938 | 22 µs | 1.2 µs |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 861 ns | 4.7 µs | 93 µs| 0% | 78% | 0:00:15.198191 | 5.3 µs | 352 ns |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 798 ns | 4.1 µs | 100 µs| 50% | 94% | 0:00:16.205439 | 2.5 µs | 152 ns |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 317 ns | 9.1 µs | 75 µs| 0% | 63% | 0:00:10 | 791 ns | 79 ns |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 2.4 µs | 5.4 µs | 101 µs| 0% | 19% | 0:00:11.086567 | 2.1 µs | 187 ns |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 9.3 µs | 37 µs | 254 µs| 0% | 76% | 0:00:14.163308 | 82 µs | 5.8 µs |
| 1599 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 408 ns | 1.4 µs | 99 µs| 0% | 74% | 0:00:12.140352 | 36 µs | 3.0 µs |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 268 ns | 8.6 µs | 75 µs| 0% | 68% | 0:00:11.131847 | 879 ns | 79 ns |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 2.3 µs | 5.7 µs | 100 µs| 0% | 35% | 0:00:17.194203 | 4.8 µs | 278 ns |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 470 ns | 7.8 µs | 99 µs| 0% | 72% | 0:00:10 | 20 µs | 2.0 µs |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 418 ns | 1.6 µs | 99 µs| 0% | 79% | 0:00:11.132083 | 1.6 µs | 143 ns |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 431 ns | 4.0 µs | 99 µs| 0% | 76% | 0:00:13.113498 | 1.3 µs | 95 ns |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.0 µs | 4.2 µs | 94 µs| 0% | 62% | 0:00:10.101686 | 1.6 µs | 156 ns |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 779 ns | 4.7 µs | 94 µs| 50% | 91% | 0:00:12.138766 | 3.9 µs | 317 ns |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 3.2 µs | 37 µs | 183 µs| 0% | 48% | 0:00:59.741418 | 86 µs | 1.4 µs |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 214 ns | 8.6 µs | 75 µs| 0% | 75% | 0:00:14.180839 | 1.5 µs | 108 ns |
| 1552 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 423 ns | 1.3 µs | 99 µs| 0% | 79% | 0:00:16.155134 | 1.3 µs | 78 ns |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.6 µs | 5.3 µs | 113 µs| 0% | 10% | 0:08:00.999280 | 312 µs | 649 ns |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.4 µs | 4.9 µs | 114 µs| 0% | 7% | 0:08:55.106925 | 465 µs | 869 ns |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 4.7 µs | 16 µs | 99 µs| 0% | 11% | 0:06:36.949382 | 483 µs | 1.2 µs |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 6.0 µs | 17 µs | 99 µs| 0% | 10% | 0:06:27.999136 | 482 µs | 1.2 µs |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 5.1 µs | 16 µs | 98 µs| 0% | 9% | 0:07:20.001677 | 460 µs | 1.0 µs |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 5.3 µs | 17 µs | 100 µs| 0% | 10% | 0:07:19.001832 | 484 µs | 1.1 µs |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 4.4 µs | 13 µs | 87 µs| 0% | 14% | 0:07:30.978994 | 471 µs | 1.0 µs |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 3.7 µs | 12 µs | 86 µs| 0% | 16% | 0:06:33.984432 | 276 µs | 701 ns |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.4 µs | 14 µs | 107 µs| 0% | 27% | 0:06:44.979848 | 302 µs | 746 ns |
| 1547 | 11 Nodes | PTPd | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 13 µs | 43 µs | 121 µs| 0% | 6% | 0:05:39.012263 | 494 µs | 1.5 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 164 ns | 467 ns | 75 µs| 0% | 96% | 0:00:15.155770 | 39 µs | 2.6 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 175 ns | 458 ns | 75 µs| 0% | 97% | 0:00:10 | 6.7 µs | 672 ns |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 407 ns | 8.8 µs | 99 µs| 0% | 76% | 0:00:14.169814 | 31 µs | 2.2 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 479 ns | 2.5 µs | 99 µs| 0% | 65% | 0:00:15.182101 | 19 µs | 1.2 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 446 ns | 3.2 µs | 99 µs| 0% | 77% | 0:00:21.250922 | 18 µs | 849 ns |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 470 ns | 9.5 µs | 99 µs| 0% | 71% | 0:00:14.201958 | 30 µs | 2.1 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.2 µs | 4.7 µs | 94 µs| 0% | 48% | 0:00:19.242321 | 21 µs | 1.1 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 979 ns | 4.6 µs | 94 µs| 0% | 66% | 0:00:20.231568 | 25 µs | 1.3 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 2.0 µs | 5.6 µs | 100 µs| 50% | 34% | 0:00:20.235379 | 21 µs | 1.0 µs |
| 1549 | 11 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 29 µs | 45 µs | 254 µs| 0% | 3% | 0:04:20.977677 | 89 µs | 340 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 333 ns | 902 ns | 37 µs| 0% | 100% | 0:00:11.000194 | 807 ms | 73 ms |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 3.3 µs | 14 µs | 46 µs| 0% | 96% | 0:00:14.002307 | 22 µs | 1.6 µs |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 496 ns | 1.5 µs | 48 µs| 0% | 100% | 0:00:16.001154 | 3.4 µs | 213 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 530 ns | 1.5 µs | 48 µs| 0% | 100% | 0:00:17.001197 | 11 µs | 651 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 2.7 µs | 13 µs | 46 µs| 0% | 93% | 0:00:22.001785 | 19 µs | 879 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 2.8 µs | 19 µs | 69 µs| 0% | 77% | 0:00:22.999078 | 22 µs | 954 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 521 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:18.001706 | 15 µs | 843 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 526 ns | 1.4 µs | 49 µs| 0% | 100% | 0:00:18.001424 | 6.6 µs | 365 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.0 µs | 13 µs | 46 µs| 0% | 96% | 0:00:44.004159 | 20 µs | 461 ns |
| 1551 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 331 ns | 907 ns | 37 µs| 0% | 100% | 0:00:15.000049 | 148 ms | 9.9 ms |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 328 ns | 880 ns | 37 µs| 0% | 100% | 0:00:13.997432 | 488 ms | 35 ms |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 333 ns | 878 ns | 37 µs| 0% | 100% | 0:00:13.999451 | 195 ms | 14 ms |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 547 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:19.001587 | 19 µs | 1.0 µs |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 549 ns | 1.4 µs | 49 µs| 0% | 100% | 0:00:20.001700 | 13 µs | 671 ns |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 559 ns | 1.4 µs | 48 µs| 0% | 100% | 0:00:10.000544 | 6.1 µs | 606 ns |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 519 ns | 1.4 µs | 49 µs| 0% | 100% | 0:00:16.000881 | 5.4 µs | 335 ns |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 4.1 µs | 15 µs | 46 µs| 0% | 96% | 0:00:19.649446 | 10 µs | 527 ns |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 3.6 µs | 15 µs | 46 µs| 0% | 96% | 0:00:37.651571 | 44 µs | 1.2 µs |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.3 µs | 14 µs | 46 µs| 0% | 93% | 0:01:12.002256 | 42 µs | 579 ns |
| 1548 | 11 Nodes | PTP4L | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 3.0 µs | 20 µs | 69 µs| 0% | 80% | 0:00:19.000807 | 41 µs | 2.2 µs |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 1.4 µs | 4.6 µs | 114 µs| 0% | 12% | 0:08:44.009766 | 465 µs | 888 ns |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 4.4 µs | 13 µs | 86 µs| 0% | 14% | 0:06:26.996714 | 280 µs | 725 ns |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 5.1 µs | 16 µs | 99 µs| 0% | 7% | 0:06:52.003709 | 475 µs | 1.2 µs |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 5.1 µs | 16 µs | 98 µs| 0% | 9% | 0:07:13.002713 | 484 µs | 1.1 µs |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 4.9 µs | 16 µs | 99 µs| 0% | 10% | 0:06:36.003016 | 489 µs | 1.2 µs |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 4.5 µs | 14 µs | 86 µs| 0% | 13% | 0:07:18.994983 | 469 µs | 1.1 µs |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 3.4 µs | 12 µs | 106 µs| 0% | 28% | 0:06:29.988803 | 312 µs | 801 ns |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 11 µs | 46 µs | 121 µs| 0% | 9% | 0:05:55.993473 | 576 µs | 1.6 µs |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 1.5 µs | 4.8 µs | 113 µs| 0% | 13% | 0:08:01.999168 | 311 µs | 646 ns |
| 1550 | 11 Nodes | PTPd | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 5.2 µs | 15 µs | 99 µs| 0% | 11% | 0:07:25.993919 | 492 µs | 1.1 µs |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 210 ns | 8.3 µs | 75 µs| 0% | 78% | 0:00:15.192094 | 35 µs | 2.3 µs |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 385 ns | 1.1 µs | 99 µs| 0% | 85% | 0:00:28.316322 | 19 µs | 685 ns |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 1.2 µs | 6.0 µs | 93 µs| 50% | 73% | 0:00:28.293122 | 22 µs | 767 ns |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 23 µs | 45 µs | 236 µs| 0% | 12% | 0:00:17.204137 | 89 µs | 5.1 µs |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 188 ns | 8.4 µs | 75 µs| 0% | 87% | 0:00:13.116590 | 46 µs | 3.5 µs |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 1.2 µs | 5.3 µs | 93 µs| 0% | 53% | 0:00:17.189080 | 24 µs | 1.4 µs |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.3 µs | 4.8 µs | 94 µs| 0% | 44% | 0:00:29.337354 | 24 µs | 832 ns |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 433 ns | 2.3 µs | 99 µs| 0% | 80% | 0:00:15.172316 | 17 µs | 1.1 µs |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 468 ns | 7.7 µs | 99 µs| 0% | 71% | 0:00:25.291267 | 32 µs | 1.2 µs |
| 2002 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 455 ns | 8.6 µs | 99 µs| 0% | 72% | 0:00:11.154384 | 11 µs | 968 ns |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi57 | SECONDARY_SLAVE | 241 ns | 8.8 µs | 75 µs| 0% | 73% | 0:00:15.158891 | 39 µs | 2.6 µs |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux01 | TERTIARY_SLAVE | 368 ns | 1.1 µs | 99 µs| 0% | 83% | 0:00:15.187213 | 11 µs | 728 ns |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux03 | TERTIARY_SLAVE | 418 ns | 1.2 µs | 99 µs| 0% | 79% | 0:00:12.089394 | 18 µs | 1.5 µs |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux04 | TERTIARY_SLAVE | 416 ns | 1.3 µs | 99 µs| 0% | 85% | 0:00:13.136948 | 30 µs | 2.3 µs |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi08 | TERTIARY_SLAVE | 1.4 µs | 5.0 µs | 100 µs| 0% | 58% | 0:00:17.230718 | 25 µs | 1.4 µs |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-tk1-1 | TERTIARY_SLAVE | 8.1 µs | 44 µs | 191 µs| 0% | 12% | 0:01:59.318044 | 130 µs | 1.1 µs |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi58 | PRIMARY_SLAVE | 218 ns | 8.7 µs | 75 µs| 0% | 74% | 0:00:15.150920 | 36 µs | 2.4 µs |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi06 | TERTIARY_SLAVE | 2.7 µs | 5.8 µs | 100 µs| 0% | 18% | 0:00:26.282326 | 21 µs | 817 ns |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-petalinux02 | TERTIARY_SLAVE | 391 ns | 1.1 µs | 99 µs| 0% | 82% | 0:00:12.176602 | 13 µs | 1.1 µs |
| 2004 | 11 Nodes | Chrony | Big Bad Cluster | bb-rpi07 | TERTIARY_SLAVE | 994 ns | 3.9 µs | 96 µs| 50% | 85% | 0:00:26.352880 | 21 µs | 809 ns |
### Benchmark: Software Fault (Slave)
_Id: `fault/software/slave`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a software fault on a slave. The software fault is created by killing and restarting the PTP daemon on the slave machine. A second slave is used as a control node to check whether it is affected by the fault. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 816 | Software Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 502 ns | 1.8 µs | 78 µs| 0% | 100% | 0:00:12.999204 | 18 µs | 1.4 µs |
| 808 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.2 µs | 9.6 µs | 57 µs| 0% | 97% | 0:00:22.219496 | 22 µs | 996 ns |
| 761 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.6 µs | 16 µs | 77 µs| 0% | 55% | 0:04:23.973291 | 134 µs | 509 ns |
| 816 | Software Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 483 ns | 1.6 µs | 78 µs| 7% | 100% | 0:00:18.001825 | 10 µs | 582 ns |
| 762 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 14 µs | 56 µs| 7% | 82% | 0:00:33.004564 | 19 µs | 583 ns |
| 762 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.9 µs | 12 µs | 57 µs| 0% | 91% | 0:00:15.005647 | 9.5 µs | 632 ns |
| 763 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 925 ns | 4.2 µs | 118 µs| 7% | 97% | 0:01:35.965131 | 25 µs | 261 ns |
| 763 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.5 µs | 6.0 µs | 116 µs| 33% | 92% | 0:00:12.127004 | 37 µs | 3.1 µs |
| 818 | Software Fault (Slave) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 188 ns | 512 ns | 75 µs| 0% | 94% | 0:00:30.326268 | 36 µs | 1.2 µs |
| 818 | Software Fault (Slave) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 202 ns | 8.5 µs | 75 µs| 7% | 81% | 0:00:12.133938 | 34 µs | 2.8 µs |
| 810 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 µs | 5.5 µs | 110 µs| 33% | 93% | 0:00:16.183228 | 20 µs | 1.2 µs |
| 810 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.5 µs | 118 µs| 7% | 97% | 0:00:16.188140 | 36 µs | 2.2 µs |
| 812 | Software Fault (Slave) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.5 µs | 4.8 µs | 114 µs| 7% | 16% | 0:07:22.948941 | 269 µs | 608 ns |
| 813 | Software Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 316 ns | 898 ns | 37 µs| 8% | 100% | 0:00:19.000872 | 464 ms | 24 ms |
| 813 | Software Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 318 ns | 892 ns | 37 µs| 0% | 100% | 0:00:14.002190 | 18 ms | 1.3 ms |
| 814 | Software Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 311 ns | 894 ns | 37 µs| 0% | 100% | 0:00:12.009233 | 355 ms | 30 ms |
| 812 | Software Fault (Slave) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 1.1 µs | 3.1 µs | 114 µs| 0% | 21% | 0:04:44.851944 | 122 µs | 429 ns |
| 814 | Software Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 328 ns | 898 ns | 37 µs| 7% | 100% | 0:00:13.998859 | 583 ms | 42 ms |
| 807 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.8 µs | 20 µs | 89 µs| 0% | 41% | 0:07:23.920983 | 760 µs | 1.7 µs |
| 811 | Software Fault (Slave) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 1.2 µs | 3.6 µs | 114 µs| 0% | 17% | 0:04:44.975281 | 119 µs | 418 ns |
| 811 | Software Fault (Slave) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.4 µs | 4.8 µs | 114 µs| 7% | 18% | 0:06:47.977068 | 251 µs | 615 ns |
| 817 | Software Fault (Slave) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 173 ns | 466 ns | 75 µs| 7% | 98% | 0:00:18.230117 | 1.4 µs | 79 ns |
| 815 | Software Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 503 ns | 1.7 µs | 78 µs| 7% | 100% | 0:00:19.968908 | 11 µs | 545 ns |
| 817 | Software Fault (Slave) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 276 ns | 8.1 µs | 75 µs| 0% | 72% | 0:00:18.237071 | 34 µs | 1.9 µs |
| 1025 | Software Fault (Slave) | SPTP (Software Timestamping) | Xilinx | petalinux03 | SECONDARY_SLAVE | 1.8 µs | 6.6 µs | 40 µs| 0% | 100% | 0:00:10.004607 | 7.5 µs | 746 ns |
| 1026 | Software Fault (Slave) | Chrony | Xilinx | petalinux03 | SECONDARY_SLAVE | 380 ns | 7.4 µs | 42 µs| 0% | 73% | 0:00:28.321256 | 23 µs | 829 ns |
| 1024 | Software Fault (Slave) | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 387 ns | 1.1 µs | 20 µs| 8% | 100% | 0:00:14.000114 | 787 ms | 56 ms |
| 1030 | Software Fault (Slave) | Chrony | Xilinx | petalinux03 | SECONDARY_SLAVE | 525 ns | 8.8 µs | 42 µs| 0% | 67% | 0:00:24.280933 | 19 µs | 786 ns |
| 1028 | Software Fault (Slave) | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 353 ns | 1.0 µs | 20 µs| 8% | 97% | 0:00:14.000169 | 323 ms | 23 ms |
| 1028 | Software Fault (Slave) | PTP4L | Xilinx | petalinux03 | SECONDARY_SLAVE | 385 ns | 979 ns | 20 µs| 0% | 99% | 0:00:13.000087 | 37 ms | 2.8 ms |
| 1026 | Software Fault (Slave) | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 418 ns | 7.0 µs | 43 µs| 7% | 76% | 0:00:16.150423 | 8.8 µs | 547 ns |
| 1027 | Software Fault (Slave) | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 5.5 µs | 18 µs | 38 µs| 7% | 19% | 0:03:53.929216 | 103 µs | 441 ns |
| 1027 | Software Fault (Slave) | PTPd | Xilinx | petalinux03 | SECONDARY_SLAVE | 5.5 µs | 16 µs | 38 µs| 0% | 13% | 0:03:23.963757 | 104 µs | 508 ns |
| 1023 | Software Fault (Slave) | PTPd | Xilinx | petalinux03 | SECONDARY_SLAVE | 5.4 µs | 16 µs | 40 µs| 0% | 20% | 0:03:31.978698 | 99 µs | 467 ns |
| 1023 | Software Fault (Slave) | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 7.1 µs | 18 µs | 38 µs| 7% | 14% | 0:03:12.979018 | 102 µs | 530 ns |
| 1030 | Software Fault (Slave) | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 686 ns | 9.8 µs | 42 µs| 7% | 55% | 0:00:14.133245 | 16 µs | 1.1 µs |
| 1025 | Software Fault (Slave) | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 1.7 µs | 7.1 µs | 39 µs| 7% | 99% | 0:00:10 | 7.8 µs | 785 ns |
| 868 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.8 µs | 26 ms | 66 µs| 33% | 72% | 0:00:10.227372 | 37 µs | 3.6 µs |
| 868 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 7.9 µs | 67 µs| 7% | 100% | 0:00:13.002375 | 3.0 µs | 231 ns |
| 869 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 7.7 µs | 66 µs| 7% | 100% | 0:00:11.002285 | 7.0 µs | 640 ns |
| 869 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.1 µs | 27 ms | 66 µs| 33% | 77% | 0:00:15.002822 | 28 µs | 1.9 µs |
| 1397 | Software Fault (Slave) | SPTP | Xilinx | petalinux03 | SECONDARY_SLAVE | 295 ns | 837 ns | 20 µs| 0% | 98% | 0:00:17.008843 | 2.0 µs | 115 ns |
| 1398 | Software Fault (Slave) | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.2 µs | 21 µs | 73 µs| 7% | 12% | 0:00:45.972286 | 75 µs | 1.6 µs |
| 1389 | Software Fault (Slave) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 226 ns | 632 ns | 37 µs| 7% | 100% | 0:00:35.973826 | 761 ms | 21 ms |
| 1389 | Software Fault (Slave) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 212 ns | 597 ns | 37 µs| 0% | 100% | 0:00:15.007234 | 4.0 µs | 266 ns |
| 1397 | Software Fault (Slave) | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 301 ns | 903 ns | 20 µs| 7% | 97% | 0:00:13.009484 | 3.4 µs | 258 ns |
| 1401 | Software Fault (Slave) | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.6 µs | 21 µs | 237 µs| 7% | 98% | 0:00:18.180718 | 31 µs | 1.7 µs |
| 1399 | Software Fault (Slave) | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.1 µs | 17 µs | 63 µs| 7% | 98% | 0:00:10.000268 | 41 µs | 4.1 µs |
| 808 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.8 µs | 11 µs | 56 µs| 8% | 91% | 0:00:34.002081 | 14 µs | 421 ns |
| 807 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.5 µs | 16 µs | 65 µs| 7% | 15% | 0:01:15.925899 | 73 µs | 961 ns |
| 761 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 17 µs | 60 µs| 7% | 12% | 0:00:55.073749 | 72 µs | 1.3 µs |
| 1024 | Software Fault (Slave) | PTP4L | Xilinx | petalinux03 | SECONDARY_SLAVE | 367 ns | 1.0 µs | 20 µs| 0% | 99% | 0:00:13.000214 | 676 ms | 52 ms |
| 815 | Software Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 502 ns | 1.6 µs | 78 µs| 0% | 100% | 0:00:16.006889 | 18 µs | 1.1 µs |
| 1621 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.6 µs | 17 µs | 85 µs| 0% | 37% | 0:04:48.910652 | 192 µs | 665 ns |
| 1621 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.0 µs | 20 µs | 66 µs| 7% | 16% | 0:05:12.966885 | 212 µs | 679 ns |
| 1626 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 11 µs | 57 µs| 8% | 96% | 0:00:15.001585 | 17 µs | 1.1 µs |
| 1630 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 14 µs | 57 µs| 8% | 98% | 0:00:10.000476 | 15 µs | 1.5 µs |
| 1632 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 µs | 4.4 µs | 112 µs| 33% | 91% | 0:00:34.388013 | 22 µs | 633 ns |
| 1624 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 938 ns | 4.4 µs | 118 µs| 7% | 94% | 0:00:20.258250 | 27 µs | 1.4 µs |
| 1624 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.2 µs | 5.1 µs | 114 µs| 33% | 99% | 0:00:15.133601 | 39 µs | 2.6 µs |
| 1623 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 7.5 µs | 67 µs| 7% | 100% | 0:00:12.222119 | 36 µs | 3.0 µs |
| 1623 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.2 µs | 36 ms | 64 µs| 33% | 62% | 0:00:18.001192 | 39 µs | 2.2 µs |
| 1622 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.7 µs | 12 µs | 56 µs| 7% | 80% | 0:01:18.055242 | 20 µs | 257 ns |
| 1622 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.4 µs | 10 µs | 57 µs| 0% | 92% | 0:02:00.006480 | 55 µs | 455 ns |
| 1625 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.2 µs | 16 µs | 60 µs| 7% | 10% | 0:05:55.075403 | 222 µs | 626 ns |
| 1625 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 7.4 µs | 22 µs | 83 µs| 0% | 30% | 0:07:18.974908 | 1.0 ms | 2.4 µs |
| 1626 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.6 µs | 19 µs | 57 µs| 0% | 80% | 0:00:12.000526 | 13 µs | 1.1 µs |
| 1627 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 µs | 7.6 µs | 67 µs| 7% | 100% | 0:00:10.998269 | 8.7 µs | 793 ns |
| 1627 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 16 ms | 37 ms | 67 µs| 33% | 46% | 0:00:14.000065 | 39 µs | 2.8 µs |
| 1628 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.6 µs | 119 µs| 7% | 93% | 0:00:29.275535 | 19 µs | 642 ns |
| 1628 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.3 µs | 5.0 µs | 112 µs| 33% | 97% | 0:00:27.289519 | 40 µs | 1.5 µs |
| 1629 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.6 µs | 20 µs | 61 µs| 7% | 11% | 0:05:14.941152 | 211 µs | 669 ns |
| 1629 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.6 µs | 18 µs | 82 µs| 0% | 41% | 0:05:26.943354 | 205 µs | 628 ns |
| 1630 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.8 µs | 12 µs | 57 µs| 0% | 96% | 0:00:26.003512 | 32 µs | 1.2 µs |
| 1631 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 7.9 µs | 67 µs| 7% | 100% | 0:00:13.003104 | 8.3 µs | 636 ns |
| 1631 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 5.2 µs | 37 ms | 65 µs| 33% | 61% | 0:00:16.004239 | 41 µs | 2.5 µs |
| 1632 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.3 µs | 119 µs| 7% | 90% | 0:00:22.220312 | 13 µs | 589 ns |
| 1797 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.0 µs | 12 µs | 58 µs| 0% | 99% | 0:00:31.994465 | 41 µs | 1.3 µs |
| 1795 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 887 ns | 5.1 µs | 109 µs| 33% | 88% | 0:00:23.229797 | 19 µs | 806 ns |
| 1804 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 8.8 µs | 24 µs | 95 µs| 0% | 35% | 0:07:32.906579 | 1.1 ms | 2.3 µs |
| 1798 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 7.8 µs | 67 µs| 7% | 100% | 0:00:15.008502 | 14 µs | 940 ns |
| 1798 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.1 ms | 37 ms | 66 µs| 33% | 48% | 0:00:12.004309 | 46 µs | 3.9 µs |
| 1792 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.7 µs | 15 µs | 66 µs| 7% | 15% | 0:06:13.938052 | 232 µs | 620 ns |
| 1792 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.4 µs | 20 µs | 89 µs| 0% | 36% | 0:07:47.925904 | 1.1 ms | 2.3 µs |
| 1796 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.2 µs | 20 µs | 62 µs| 7% | 12% | 0:05:02.960326 | 231 µs | 764 ns |
| 1796 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 8.5 µs | 24 µs | 86 µs| 0% | 37% | 0:07:03.909630 | 1.1 ms | 2.5 µs |
| 1800 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.6 µs | 24 µs | 63 µs| 7% | 6% | 0:04:29.953154 | 226 µs | 837 ns |
| 1800 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.5 µs | 19 µs | 79 µs| 0% | 45% | 0:04:50.918535 | 223 µs | 765 ns |
| 1793 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 12 µs | 57 µs| 7% | 87% | 0:00:13.000725 | 11 µs | 831 ns |
| 1793 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.0 µs | 12 µs | 56 µs| 0% | 90% | 0:00:17.003182 | 27 µs | 1.6 µs |
| 1797 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 13 µs | 58 µs| 8% | 97% | 0:00:17.000615 | 18 µs | 1.1 µs |
| 1801 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.0 µs | 9.3 µs | 57 µs| 0% | 93% | 0:02:35.012988 | 58 µs | 373 ns |
| 1801 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 14 µs | 57 µs| 7% | 79% | 0:00:21.001858 | 37 µs | 1.7 µs |
| 1803 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.5 µs | 118 µs| 7% | 92% | 0:00:15.202601 | 35 µs | 2.3 µs |
| 1803 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.6 µs | 5.3 µs | 115 µs| 33% | 96% | 0:00:22.254145 | 33 µs | 1.5 µs |
| 1794 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 7.3 µs | 67 µs| 7% | 100% | 0:00:10.000845 | 7.8 µs | 778 ns |
| 1794 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 5.1 µs | 37 ms | 67 µs| 33% | 62% | 0:00:14.000452 | 46 µs | 3.3 µs |
| 1795 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 982 ns | 4.5 µs | 118 µs| 7% | 96% | 0:00:18.216356 | 20 µs | 1.1 µs |
| 1799 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 µs | 5.3 µs | 113 µs| 33% | 96% | 0:00:22.239054 | 8.3 µs | 372 ns |
| 1799 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 962 ns | 4.3 µs | 119 µs| 7% | 93% | 0:00:24.360046 | 31 µs | 1.3 µs |
| 1802 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 7.8 µs | 66 µs| 7% | 100% | 0:00:15.003476 | 11 µs | 749 ns |
| 1802 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.2 ms | 37 ms | 67 µs| 33% | 48% | 0:00:19.003334 | 41 µs | 2.2 µs |
| 1804 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.1 µs | 17 µs | 62 µs| 7% | 10% | 0:06:08.923361 | 241 µs | 652 ns |
| 1805 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.5 µs | 11 µs | 57 µs| 0% | 99% | 0:00:22.001799 | 15 µs | 677 ns |
| 1809 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.9 µs | 37 ms | 65 µs| 33% | 60% | 0:00:18.006290 | 43 µs | 2.4 µs |
| 1809 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 7.9 µs | 67 µs| 7% | 100% | 0:00:16.003820 | 18 µs | 1.1 µs |
| 1810 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.6 µs | 121 µs| 7% | 97% | 0:00:26.286530 | 24 µs | 929 ns |
| 1805 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.7 µs | 11 µs | 57 µs| 7% | 95% | 0:00:27.001283 | 7.9 µs | 292 ns |
| 1810 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 µs | 4.6 µs | 115 µs| 33% | 98% | 0:00:34.370887 | 22 µs | 637 ns |
| 1818 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 4.4 µs | 120 µs| 7% | 95% | 0:00:18.160209 | 18 µs | 1.0 µs |
| 1815 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.4 µs | 20 µs | 89 µs| 1% | 37% | 0:07:33.909975 | 1.1 ms | 2.3 µs |
| 1815 | Software Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.1 µs | 24 µs | 66 µs| 8% | 9% | 0:06:07.908224 | 231 µs | 628 ns |
| 1816 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 14 µs | 57 µs| 8% | 95% | 0:00:14.002199 | 13 µs | 929 ns |
| 1816 | Software Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.9 µs | 12 µs | 57 µs| 0% | 99% | 0:00:35.003845 | 38 µs | 1.1 µs |
| 1817 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 ms | 37 ms | 65 µs| 33% | 47% | 0:00:13.004820 | 44 µs | 3.4 µs |
| 1817 | Software Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.8 µs | 67 µs| 7% | 100% | 0:00:16.025015 | 8.9 µs | 554 ns |
| 1818 | Software Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.2 µs | 5.0 µs | 111 µs| 33% | 100% | 0:00:16.181278 | 32 µs | 2.0 µs |
### Benchmark: Hardware Fault (Switch)
_Id: `fault/hardware/switch`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on the network switch. The hardware fault is created by turning off the power to the network switch using a smart PDU (check the documentation on how to register it with PTP-Perf). It is expected that both the primary and the secondary slave are affected by the network outage. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 775 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 161 µs | 874 µs | 63 µs| 10% | 3% | 0:07:14.943247 | 753 µs | 1.7 µs |
| 782 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 166 ns | 483 ns | 75 µs| 7% | 94% | 0:00:19.186923 | 5.7 µs | 295 ns |
| 777 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.9 µs | 26 ms | 67 µs| 41% | 75% | 0:00:14.002694 | 45 µs | 3.2 µs |
| 778 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 4.9 µs | 117 µs| 7% | 97% | 0:00:49.552782 | 38 µs | 765 ns |
| 779 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 3.1 µs | 45 µs | 114 µs| 9% | 12% | 0:04:44.934451 | 124 µs | 436 ns |
| 779 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 41 µs | 243 µs | 114 µs| 9% | 6% | 0:07:11.933814 | 252 µs | 584 ns |
| 781 | Hardware Fault (Switch) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 512 ns | 1.7 µs | 78 µs| 7% | 100% | 0:00:15.003038 | 13 µs | 889 ns |
| 1390 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 206 ns | 617 ns | 37 µs| 7% | 100% | 0:00:36.818908 | 364 ms | 9.9 ms |
| 780 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 336 ns | 893 ns | 37 µs| 9% | 100% | 0:00:14.000820 | 355 ms | 25 ms |
| 777 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 7.6 µs | 66 µs| 7% | 100% | 0:00:10.001584 | 7.6 µs | 760 ns |
| 776 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 14 µs | 57 µs| 9% | 92% | 0:00:11.993868 | 21 µs | 1.8 µs |
| 778 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.1 µs | 6.1 µs | 108 µs| 41% | 79% | 0:00:28.328693 | 22 µs | 762 ns |
| 782 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 169 ns | 500 ns | 75 µs| 7% | 93% | 0:00:10 | 44 µs | 4.4 µs |
| 1390 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 211 ns | 637 ns | 37 µs| 7% | 100% | 0:00:32.968274 | 373 ms | 11 ms |
| 775 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.6 µs | 21 µs | 60 µs| 10% | 11% | 0:01:22.960413 | 55 µs | 668 ns |
| 781 | Hardware Fault (Switch) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 467 ns | 1.8 µs | 78 µs| 7% | 100% | 0:00:15.003443 | 18 µs | 1.2 µs |
| 776 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.8 µs | 15 µs | 56 µs| 9% | 98% | 0:02:09.007796 | 46 µs | 358 ns |
| 780 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 352 ns | 894 ns | 37 µs| 9% | 99% | 0:00:10 | 17 ms | 1.7 ms |
| 1465 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux03 | SECONDARY_SLAVE | 384 ns | 1.7 µs | 42 µs| 7% | 80% | 0:00:31.360664 | 12 µs | 389 ns |
| 1465 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 381 ns | 1.3 µs | 42 µs| 7% | 80% | 0:00:20.188276 | 18 µs | 898 ns |
| 1457 | Hardware Fault (Switch) | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.0 µs | 19 µs | 73 µs| 9% | 9% | 0:00:24.977894 | 71 µs | 2.9 µs |
| 1458 | Hardware Fault (Switch) | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.7 µs | 15 µs | 61 µs| 9% | 97% | 0:00:10 | 32 µs | 3.2 µs |
| 1460 | Hardware Fault (Switch) | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.5 µs | 21 µs | 237 µs| 7% | 95% | 0:00:11.135103 | 48 µs | 4.3 µs |
| 1462 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux03 | SECONDARY_SLAVE | 6.9 µs | 19 µs | 41 µs| 7% | 13% | 0:01:08.904734 | 55 µs | 797 ns |
| 1462 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 7.4 µs | 23 µs | 40 µs| 7% | 16% | 0:00:57.980205 | 45 µs | 784 ns |
| 1463 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux03 | SECONDARY_SLAVE | 386 ns | 1.1 µs | 20 µs| 9% | 100% | 0:00:20.000293 | 297 ms | 15 ms |
| 1463 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 385 ns | 1.1 µs | 20 µs| 9% | 100% | 0:00:14.000251 | 790 ms | 56 ms |
| 1464 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux03 | SECONDARY_SLAVE | 291 ns | 809 ns | 20 µs| 7% | 100% | 0:00:17.009103 | 1.7 µs | 100 ns |
| 1464 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 293 ns | 894 ns | 20 µs| 7% | 99% | 0:00:19.010433 | 3.3 µs | 175 ns |
| 1637 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 151 µs | 532 µs | 115 µs| 9% | 2% | 0:08:44.957272 | 464 µs | 883 ns |
| 1638 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 374 ns | 907 ns | 37 µs| 9% | 99% | 0:00:17.001177 | 92 ms | 5.4 ms |
| 1640 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 175 ns | 463 ns | 75 µs| 8% | 94% | 0:00:18.212103 | 36 µs | 2.0 µs |
| 1657 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux03 | SECONDARY_SLAVE | 7.5 µs | 29 µs | 38 µs| 8% | 13% | 0:01:50.971343 | 79 µs | 711 ns |
| 1643 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 312 ns | 841 ns | 20 µs| 8% | 99% | 0:00:22.010810 | 3.3 µs | 150 ns |
| 1644 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux03 | SECONDARY_SLAVE | 410 ns | 1.5 µs | 42 µs| 7% | 72% | 0:00:23.224378 | 17 µs | 734 ns |
| 1649 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 23 µs | 211 µs | 63 µs| 10% | 4% | 0:06:01.978430 | 221 µs | 609 ns |
| 1651 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 7.0 µs | 36 ms | 64 µs| 41% | 54% | 0:00:16.000304 | 38 µs | 2.4 µs |
| 1668 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.5 µs | 115 µs| 7% | 89% | 0:00:18.185730 | 37 µs | 2.0 µs |
| 1669 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 142 µs | 504 µs | 115 µs| 9% | 2% | 0:08:29.009961 | 463 µs | 909 ns |
| 1686 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux03 | SECONDARY_SLAVE | 8.3 µs | 31 µs | 38 µs| 7% | 12% | 0:01:48.932205 | 69 µs | 632 ns |
| 1674 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux03 | SECONDARY_SLAVE | 407 ns | 1.1 µs | 20 µs| 9% | 100% | 0:00:17.000681 | 1.4 µs | 83 ns |
| 1676 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux03 | SECONDARY_SLAVE | 405 ns | 1.3 µs | 42 µs| 7% | 78% | 0:00:16.179196 | 4.0 µs | 247 ns |
| 1680 | Hardware Fault (Switch) | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.9 µs | 23 µs | 238 µs| 7% | 95% | 0:00:11.130836 | 79 µs | 7.1 µs |
| 1639 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 206 ns | 602 ns | 37 µs| 7% | 100% | 0:00:26.976721 | 107 ms | 4.0 ms |
| 1639 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 198 ns | 581 ns | 37 µs| 7% | 100% | 0:00:19.927402 | 64 ms | 3.2 ms |
| 1655 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 203 ns | 611 ns | 37 µs| 7% | 100% | 0:00:13.995066 | 2.3 µs | 167 ns |
| 1655 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 220 ns | 621 ns | 37 µs| 7% | 100% | 0:00:29.922537 | 265 ms | 8.9 ms |
| 1671 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 214 ns | 592 ns | 37 µs| 7% | 100% | 0:00:37.905450 | 804 ms | 21 ms |
| 1671 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 208 ns | 595 ns | 37 µs| 7% | 100% | 0:00:40.952896 | 748 ms | 18 ms |
| 1640 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 165 ns | 494 ns | 75 µs| 8% | 94% | 0:00:11.133312 | 41 µs | 3.7 µs |
| 1656 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 167 ns | 480 ns | 75 µs| 7% | 95% | 0:00:10.112775 | 33 µs | 3.3 µs |
| 1656 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 196 ns | 7.6 µs | 75 µs| 7% | 82% | 0:00:12.092561 | 35 µs | 2.9 µs |
| 1672 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 204 ns | 8.3 µs | 75 µs| 8% | 85% | 0:00:10.113816 | 39 µs | 3.8 µs |
| 1672 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 198 ns | 8.6 µs | 75 µs| 8% | 87% | 0:00:12.123530 | 8.1 µs | 666 ns |
| 1686 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 6.5 µs | 34 µs | 38 µs| 7% | 16% | 0:02:19.982435 | 51 µs | 367 ns |
| 1641 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 7.7 µs | 30 µs | 41 µs| 7% | 15% | 0:01:47.921040 | 73 µs | 675 ns |
| 1641 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux03 | SECONDARY_SLAVE | 7.8 µs | 30 µs | 41 µs| 7% | 19% | 0:02:07.971064 | 67 µs | 520 ns |
| 1657 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 7.7 µs | 31 µs | 39 µs| 7% | 15% | 0:01:53.971107 | 78 µs | 685 ns |
| 1673 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 7.4 µs | 27 µs | 40 µs| 7% | 17% | 0:01:48.914059 | 71 µs | 649 ns |
| 1673 | Hardware Fault (Switch) | PTPd | Xilinx | petalinux03 | SECONDARY_SLAVE | 7.2 µs | 30 µs | 40 µs| 7% | 15% | 0:02:40.914328 | 69 µs | 427 ns |
| 1687 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 371 ns | 1.1 µs | 20 µs| 9% | 100% | 0:00:16.000667 | 243 ms | 15 ms |
| 1687 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux03 | SECONDARY_SLAVE | 363 ns | 1.0 µs | 20 µs| 9% | 99% | 0:00:14.000190 | 732 ms | 52 ms |
| 1642 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 380 ns | 1.1 µs | 20 µs| 9% | 100% | 0:00:14.000087 | 873 ms | 62 ms |
| 1642 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux03 | SECONDARY_SLAVE | 418 ns | 1.2 µs | 20 µs| 9% | 99% | 0:00:10 | 367 ms | 37 ms |
| 1658 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 376 ns | 1.1 µs | 20 µs| 9% | 100% | 0:00:15.000481 | 786 ms | 52 ms |
| 1658 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux03 | SECONDARY_SLAVE | 371 ns | 1.2 µs | 20 µs| 9% | 100% | 0:00:15.000142 | 1.8 µs | 123 ns |
| 1674 | Hardware Fault (Switch) | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 385 ns | 1.1 µs | 20 µs| 9% | 99% | 0:00:16.000214 | 68 ms | 4.3 ms |
| 1688 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 320 ns | 840 ns | 20 µs| 7% | 98% | 0:00:12.006165 | 3.5 µs | 292 ns |
| 1688 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux03 | SECONDARY_SLAVE | 294 ns | 898 ns | 20 µs| 7% | 97% | 0:00:17.008559 | 1.7 µs | 99 ns |
| 1643 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux03 | SECONDARY_SLAVE | 310 ns | 839 ns | 20 µs| 8% | 97% | 0:00:18.009631 | 1.7 µs | 94 ns |
| 1659 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 284 ns | 886 ns | 20 µs| 7% | 98% | 0:00:12.006365 | 3.4 µs | 279 ns |
| 1659 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux03 | SECONDARY_SLAVE | 288 ns | 839 ns | 20 µs| 7% | 98% | 0:00:16.005889 | 2.5 µs | 159 ns |
| 1689 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 371 ns | 1.1 µs | 42 µs| 7% | 75% | 0:00:21.218895 | 17 µs | 809 ns |
| 1689 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux03 | SECONDARY_SLAVE | 373 ns | 6.1 µs | 42 µs| 7% | 69% | 0:00:26.307788 | 23 µs | 864 ns |
| 1675 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 305 ns | 833 ns | 20 µs| 7% | 98% | 0:00:17.012003 | 2.7 µs | 156 ns |
| 1675 | Hardware Fault (Switch) | SPTP | Xilinx | petalinux03 | SECONDARY_SLAVE | 285 ns | 912 ns | 20 µs| 7% | 98% | 0:00:11.005671 | 1.2 µs | 113 ns |
| 1660 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 375 ns | 1.1 µs | 42 µs| 7% | 86% | 0:00:19.198643 | 4.2 µs | 221 ns |
| 1660 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux03 | SECONDARY_SLAVE | 388 ns | 1.5 µs | 42 µs| 7% | 71% | 0:00:16.162732 | 12 µs | 719 ns |
| 1644 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 358 ns | 1.1 µs | 42 µs| 7% | 76% | 0:00:18.156326 | 3.2 µs | 178 ns |
| 1676 | Hardware Fault (Switch) | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 358 ns | 1.1 µs | 42 µs| 7% | 82% | 0:00:15.158365 | 22 µs | 1.4 µs |
| 1690 | Hardware Fault (Switch) | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 8.7 µs | 30 µs | 72 µs| 9% | 4% | 0:01:37.980219 | 75 µs | 769 ns |
| 1645 | Hardware Fault (Switch) | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.6 µs | 21 µs | 73 µs| 9% | 16% | 0:00:30.974087 | 61 µs | 2.0 µs |
| 1661 | Hardware Fault (Switch) | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.7 µs | 25 µs | 73 µs| 9% | 9% | 0:00:18.971426 | 61 µs | 3.2 µs |
| 1677 | Hardware Fault (Switch) | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 9.5 µs | 50 µs | 77 µs| 9% | 5% | 0:00:17.966157 | 54 µs | 3.0 µs |
| 1691 | Hardware Fault (Switch) | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.5 µs | 14 µs | 61 µs| 9% | 99% | 0:00:11.000834 | 25 µs | 2.2 µs |
| 1646 | Hardware Fault (Switch) | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.3 µs | 15 µs | 61 µs| 9% | 96% | 0:00:18.000875 | 25 µs | 1.4 µs |
| 1662 | Hardware Fault (Switch) | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 3.6 µs | 15 µs | 61 µs| 9% | 96% | 0:00:10.000936 | 79 µs | 7.9 µs |
| 1678 | Hardware Fault (Switch) | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.6 µs | 15 µs | 64 µs| 9% | 99% | 0:00:10 | 32 µs | 3.2 µs |
| 1693 | Hardware Fault (Switch) | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.8 µs | 19 µs | 234 µs| 7% | 94% | 0:00:14.160540 | 79 µs | 5.6 µs |
| 1648 | Hardware Fault (Switch) | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.6 µs | 22 µs | 236 µs| 7% | 93% | 0:00:11.099832 | 40 µs | 3.6 µs |
| 1664 | Hardware Fault (Switch) | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.6 µs | 22 µs | 235 µs| 7% | 96% | 0:00:12.147953 | 101 µs | 8.3 µs |
| 1633 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 214 µs | 58 µs| 9% | 7% | 0:05:56.969857 | 212 µs | 593 ns |
| 1633 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 16 µs | 181 µs | 59 µs| 9% | 14% | 0:04:20.971599 | 195 µs | 749 ns |
| 1649 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 20 µs | 182 µs | 76 µs| 10% | 16% | 0:05:15.900848 | 207 µs | 656 ns |
| 1665 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 190 µs | 60 µs| 10% | 5% | 0:04:18.976979 | 214 µs | 826 ns |
| 1665 | Hardware Fault (Switch) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 18 µs | 188 µs | 60 µs| 10% | 20% | 0:04:20.976429 | 210 µs | 806 ns |
| 1634 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 13 µs | 56 µs| 9% | 93% | 0:00:33.002141 | 20 µs | 594 ns |
| 1634 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.3 µs | 11 µs | 56 µs| 9% | 99% | 0:00:49.009008 | 37 µs | 759 ns |
| 1650 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.6 µs | 13 µs | 56 µs| 9% | 98% | 0:00:19.005517 | 23 µs | 1.2 µs |
| 1650 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.7 µs | 17 µs | 56 µs| 9% | 83% | 0:00:12.001141 | 21 µs | 1.8 µs |
| 1666 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.4 µs | 13 µs | 58 µs| 9% | 96% | 0:00:11.000494 | 12 µs | 1.1 µs |
| 1666 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.8 µs | 13 µs | 57 µs| 9% | 97% | 0:01:44.007167 | 43 µs | 410 ns |
| 1635 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 8.9 µs | 67 µs| 8% | 98% | 0:00:11.002864 | 7.4 µs | 673 ns |
| 1635 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 9.3 µs | 36 ms | 64 µs| 41% | 54% | 0:00:14.004090 | 39 µs | 2.8 µs |
| 1651 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 8.5 µs | 66 µs| 7% | 99% | 0:00:15.972258 | 26 µs | 1.6 µs |
| 1667 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 9.1 µs | 67 µs| 7% | 98% | 0:00:18.005017 | 9.8 µs | 546 ns |
| 1667 | Hardware Fault (Switch) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 7.2 µs | 36 ms | 65 µs| 41% | 54% | 0:00:18.006660 | 44 µs | 2.4 µs |
| 1683 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 323 ns | 882 ns | 37 µs| 9% | 99% | 0:00:10 | 546 ms | 55 ms |
| 1683 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 334 ns | 890 ns | 37 µs| 9% | 100% | 0:00:13.996759 | 549 ms | 39 ms |
| 1636 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.6 µs | 117 µs| 7% | 95% | 0:00:16.161646 | 16 µs | 1.0 µs |
| 1636 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.3 µs | 4.6 µs | 112 µs| 41% | 98% | 0:00:15.108183 | 35 µs | 2.3 µs |
| 1652 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 3.8 µs | 118 µs| 8% | 88% | 0:00:18.207458 | 43 µs | 2.3 µs |
| 1652 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.2 µs | 4.8 µs | 113 µs| 41% | 95% | 0:00:32.369012 | 29 µs | 885 ns |
| 1668 | Hardware Fault (Switch) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 µs | 7.2 µs | 109 µs| 41% | 85% | 0:00:18.214048 | 12 µs | 640 ns |
| 1684 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 218 ns | 640 ns | 37 µs| 7% | 100% | 0:00:31.908454 | 383 ms | 12 ms |
| 1684 | Hardware Fault (Switch) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 218 ns | 605 ns | 37 µs| 7% | 100% | 0:00:30.895322 | 185 ms | 6.0 ms |
| 1637 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 90 µs | 344 µs | 115 µs| 9% | 0.9% | 0:08:14.007550 | 311 µs | 629 ns |
| 1653 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 69 µs | 335 µs | 115 µs| 9% | 3% | 0:07:27.001607 | 311 µs | 697 ns |
| 1653 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 150 µs | 533 µs | 115 µs| 9% | 5% | 0:08:44.006157 | 461 µs | 880 ns |
| 1669 | Hardware Fault (Switch) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 89 µs | 333 µs | 115 µs| 9% | 2% | 0:08:13.950372 | 313 µs | 633 ns |
| 1654 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 346 ns | 870 ns | 37 µs| 9% | 100% | 0:00:11.000737 | 97 ms | 8.9 ms |
| 1654 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 341 ns | 849 ns | 37 µs| 9% | 100% | 0:00:11.002832 | 810 ms | 74 ms |
| 1638 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 361 ns | 881 ns | 37 µs| 9% | 99% | 0:00:12.001909 | 910 ms | 76 ms |
| 1670 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 333 ns | 872 ns | 37 µs| 9% | 100% | 0:00:15.997982 | 566 ms | 35 ms |
| 1670 | Hardware Fault (Switch) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 330 ns | 844 ns | 37 µs| 9% | 100% | 0:00:12.985257 | 674 ms | 52 ms |
| 1685 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 166 ns | 469 ns | 75 µs| 7% | 98% | 0:00:13.143229 | 37 µs | 2.8 µs |
| 1685 | Hardware Fault (Switch) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 167 ns | 539 ns | 75 µs| 7% | 87% | 0:00:10 | 32 µs | 3.2 µs |
### Benchmark: Hardware Fault (Slave)
_Id: `fault/hardware/slave`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on a slave. The hardware fault is created by turning off the power to the slave machine using a smart PDU (check the documentation on how to register it with PTP-Perf). A second slave is used as a control node to check whether it is affected by the fault. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 800 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.6 µs | 6.6 µs | 112 µs| 33% | 77% | 0:00:14.125170 | 27 µs | 1.9 µs |
| 839 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 172 ns | 455 ns | 75 µs| 0% | 97% | 0:00:15.186356 | 5.2 µs | 342 ns |
| 800 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 9.9 µs | 118 µs| 11% | 86% | 0:00:14.152147 | 32 µs | 2.3 µs |
| 801 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.5 µs | 4.6 µs | 113 µs| 33% | 97% | 0:00:35.404892 | 17 µs | 477 ns |
| 768 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.9 µs | 14 µs | 81 µs| 0% | 34% | 0:07:23.951237 | 757 µs | 1.7 µs |
| 768 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 25 µs | 60 µs| 11% | 13% | 0:01:51.948193 | 76 µs | 675 ns |
| 796 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 5.9 µs | 19 µs | 90 µs| 0% | 40% | 0:07:16.915585 | 769 µs | 1.8 µs |
| 796 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.8 µs | 25 µs | 66 µs| 11% | 12% | 0:01:10.969256 | 77 µs | 1.1 µs |
| 837 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 336 ns | 826 ns | 37 µs| 0% | 100% | 0:00:13.995114 | 462 ms | 33 ms |
| 771 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 8.5 µs | 118 µs| 11% | 80% | 0:00:16.181699 | 19 µs | 1.2 µs |
| 837 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 326 ns | 864 ns | 37 µs| 11% | 99% | 0:00:10.002793 | 89 ms | 8.9 ms |
| 797 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.7 µs | 11 µs | 57 µs| 0% | 99% | 0:00:33.004640 | 34 µs | 1.0 µs |
| 769 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 14 µs | 56 µs| 11% | 96% | 0:00:12.994680 | 10 µs | 787 ns |
| 797 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 16 µs | 57 µs| 11% | 86% | 0:00:10 | 18 µs | 1.8 µs |
| 769 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.5 µs | 13 µs | 56 µs| 0% | 92% | 0:00:14.997518 | 11 µs | 752 ns |
| 770 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.5 µs | 26 ms | 64 µs| 33% | 65% | 0:00:11.997380 | 37 µs | 3.1 µs |
| 798 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 8.0 µs | 67 µs| 10% | 100% | 0:00:17.004696 | 10 µs | 599 ns |
| 771 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.2 µs | 4.4 µs | 112 µs| 33% | 90% | 0:00:24.255457 | 34 µs | 1.4 µs |
| 799 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.7 µs | 27 ms | 65 µs| 33% | 76% | 0:00:23.004973 | 23 µs | 996 ns |
| 866 | Hardware Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 827 ns | 259 ms | 78 µs| 10% | 74% | 0:00:19.006724 | 12 µs | 641 ns |
| 838 | Hardware Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 782 ns | 346 ms | 78 µs| 10% | 74% | 0:00:17.004798 | 11 µs | 668 ns |
| 866 | Hardware Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 497 ns | 1.5 µs | 78 µs| 0% | 100% | 0:00:19.004276 | 19 µs | 982 ns |
| 867 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 1.2 µs | 3.4 µs | 115 µs| 0% | 17% | 0:04:38.911469 | 121 µs | 434 ns |
| 1391 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 201 ns | 622 ns | 37 µs| 0% | 100% | 0:00:33.929196 | 592 ms | 17 ms |
| 1391 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 231 ns | 715 ns | 37 µs| 10% | 96% | 0:00:29.969967 | 54 ms | 1.8 ms |
| 838 | Hardware Fault (Slave) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 491 ns | 1.5 µs | 78 µs| 0% | 100% | 0:00:14.992657 | 19 µs | 1.2 µs |
| 839 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 162 ns | 480 ns | 75 µs| 10% | 99% | 0:00:15.164778 | 4.1 µs | 272 ns |
| 801 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 11 µs | 120 µs| 11% | 89% | 0:00:18.209921 | 31 µs | 1.7 µs |
| 799 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.8 µs | 66 µs| 11% | 99% | 0:00:10.004723 | 7.0 µs | 699 ns |
| 798 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.5 µs | 27 ms | 65 µs| 33% | 65% | 0:00:11.999547 | 30 µs | 2.5 µs |
| 770 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 7.6 µs | 67 µs| 10% | 99% | 0:00:10.001614 | 4.5 µs | 452 ns |
| 1696 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 15 µs | 56 µs| 11% | 78% | 0:00:40.998972 | 22 µs | 534 ns |
| 1698 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.3 µs | 4.3 µs | 114 µs| 33% | 87% | 0:00:18.170356 | 10 µs | 564 ns |
| 1700 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 299 ns | 860 ns | 37 µs| 11% | 99% | 0:00:10 | 52 ms | 5.2 ms |
| 1700 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 311 ns | 876 ns | 37 µs| 0% | 100% | 0:00:12.001187 | 243 ms | 20 ms |
| 1701 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 234 ns | 742 ns | 37 µs| 10% | 96% | 0:00:36.922992 | 658 ms | 18 ms |
| 1701 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 209 ns | 603 ns | 37 µs| 0% | 100% | 0:00:25.937563 | 136 ms | 5.2 ms |
| 1721 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.0 µs | 11 µs | 57 µs| 0% | 99% | 0:00:34.001810 | 36 µs | 1.1 µs |
| 1722 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.2 ms | 37 ms | 64 µs| 33% | 49% | 0:00:16.010327 | 47 µs | 2.9 µs |
| 1723 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.3 µs | 5.4 µs | 112 µs| 33% | 89% | 0:00:16.152077 | 43 µs | 2.7 µs |
| 1745 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.4 µs | 14 µs | 56 µs| 11% | 80% | 0:00:16.000785 | 21 µs | 1.3 µs |
| 1758 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 237 ns | 9.1 µs | 75 µs| 0% | 67% | 0:00:14.151078 | 6.3 µs | 442 ns |
| 1744 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.8 µs | 27 µs | 60 µs| 11% | 6% | 0:05:42.978168 | 215 µs | 628 ns |
| 1744 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.6 µs | 17 µs | 77 µs| 0% | 36% | 0:04:45.977034 | 221 µs | 772 ns |
| 1703 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 168 ns | 443 ns | 75 µs| 10% | 96% | 0:00:10.132870 | 42 µs | 4.1 µs |
| 1703 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 174 ns | 465 ns | 75 µs| 0% | 97% | 0:00:15.160323 | 5.6 µs | 372 ns |
| 1745 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.4 µs | 12 µs | 57 µs| 0% | 89% | 0:00:25.004146 | 26 µs | 1.0 µs |
| 1720 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 32 µs | 65 µs| 11% | 6% | 0:06:13.913436 | 219 µs | 586 ns |
| 1720 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.0 µs | 18 µs | 83 µs| 0% | 36% | 0:04:34.903906 | 208 µs | 755 ns |
| 1746 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 64 ms | 106 ms | 217 µs| 10% | 0% | 0:09:26.000711 | 912 µs | 1.6 µs |
| 1746 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 1.5 µs | 4.1 µs | 114 µs| 0% | 17% | 0:08:22.993220 | 464 µs | 922 ns |
| 1758 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 192 ns | 8.5 µs | 75 µs| 10% | 89% | 0:00:15.162805 | 40 µs | 2.6 µs |
| 1721 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.8 µs | 13 µs | 57 µs| 11% | 85% | 0:01:30.005005 | 22 µs | 248 ns |
| 1747 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 307 ns | 860 ns | 37 µs| 11% | 100% | 0:00:10.999608 | 590 ms | 54 ms |
| 1747 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 295 ns | 834 ns | 37 µs| 0% | 100% | 0:00:10.025108 | 119 ms | 12 ms |
| 1722 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 7.6 µs | 67 µs| 11% | 100% | 0:00:12.005142 | 18 µs | 1.5 µs |
| 1748 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 235 ns | 693 ns | 37 µs| 10% | 97% | 0:00:32.001316 | 381 ms | 12 ms |
| 1748 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 206 ns | 566 ns | 37 µs| 0% | 100% | 0:00:30.935282 | 268 ms | 8.7 ms |
| 1723 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 8.2 µs | 119 µs| 11% | 83% | 0:00:22.313564 | 24 µs | 1.1 µs |
| 1749 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 167 ns | 502 ns | 75 µs| 10% | 95% | 0:00:10 | 29 µs | 2.9 µs |
| 1749 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 166 ns | 464 ns | 75 µs| 0% | 94% | 0:00:13.147886 | 44 µs | 3.3 µs |
| 1725 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 337 ns | 865 ns | 37 µs| 11% | 100% | 0:00:12.000858 | 177 ms | 15 ms |
| 1725 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 339 ns | 843 ns | 37 µs| 0% | 100% | 0:00:12.002087 | 97 ms | 8.1 ms |
| 1695 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.5 µs | 32 µs | 61 µs| 11% | 6% | 0:04:44.969822 | 216 µs | 758 ns |
| 1695 | Hardware Fault (Slave) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 5.7 µs | 17 µs | 84 µs| 0% | 42% | 0:07:25.909418 | 1.0 ms | 2.3 µs |
| 1726 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 220 ns | 657 ns | 37 µs| 10% | 97% | 0:00:26.982635 | 134 ms | 5.0 ms |
| 1726 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 218 ns | 600 ns | 37 µs| 0% | 100% | 0:00:29.934623 | 200 ms | 6.7 ms |
| 1696 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 2.8 µs | 14 µs | 57 µs| 0% | 100% | 0:00:55.004646 | 50 µs | 915 ns |
| 1727 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 172 ns | 487 ns | 75 µs| 10% | 94% | 0:00:16.162226 | 38 µs | 2.3 µs |
| 1727 | Hardware Fault (Slave) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 163 ns | 469 ns | 75 µs| 0% | 96% | 0:00:17.229939 | 5.8 µs | 334 ns |
| 1697 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.7 µs | 67 µs| 11% | 100% | 0:00:17.003325 | 23 µs | 1.3 µs |
| 1697 | Hardware Fault (Slave) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 686 µs | 36 ms | 66 µs| 33% | 49% | 0:00:14.992733 | 48 µs | 3.2 µs |
| 1698 | Hardware Fault (Slave) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.7 µs | 119 µs| 11% | 96% | 0:00:24.306833 | 24 µs | 1.0 µs |
| 1699 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 164 µs | 531 µs | 115 µs| 10% | 6% | 0:08:08.001258 | 315 µs | 646 ns |
| 1699 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 1.3 µs | 3.4 µs | 114 µs| 0% | 13% | 0:08:37.956588 | 465 µs | 898 ns |
| 1756 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 303 ns | 914 ns | 37 µs| 11% | 99% | 0:00:10 | 1.1 µs | 108 ns |
| 1756 | Hardware Fault (Slave) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 326 ns | 878 ns | 37 µs| 0% | 100% | 0:00:16.001123 | 69 ms | 4.3 ms |
| 867 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 390 ms | 465 ms | 226 µs| 10% | 3% | 0:07:12.918003 | 252 µs | 583 ns |
| 1807 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 210 ns | 666 ns | 37 µs| 10% | 97% | 0:00:27.932551 | 224 ms | 8.0 ms |
| 1807 | Hardware Fault (Slave) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 210 ns | 583 ns | 37 µs| 0% | 100% | 0:00:24.941569 | 13 ms | 508 µs |
| 1808 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 307 ms | 351 ms | 217 µs| 10% | 0% | 0:09:13.013546 | 914 µs | 1.7 µs |
| 1808 | Hardware Fault (Slave) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 1.4 µs | 4.5 µs | 114 µs| 0% | 15% | 0:08:21.012471 | 465 µs | 928 ns |
### Benchmark: Hardware Fault (Master)
_Id: `fault/hardware/master`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on the master. The hardware fault is created by turning off the power to the master machine using a smart PDU (check the documentation on how to register it with PTP-Perf). A second slave is used as a control node, it is expected to also be affected by the fault. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 827 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.7 µs | 16 m | 57 µs| 12% | 71% | 0:01:15.004618 | 23 µs | 301 ns |
| 831 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.0 µs | 4.2 µs | 112 µs| 33% | 89% | 0:00:18.212393 | 8.6 µs | 472 ns |
| 783 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 9.2 µs | 22 µs | 75 µs| 0% | 9% | 0:06:40.977733 | 768 µs | 1.9 µs |
| 825 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.9 µs | 23 µs | 67 µs| 12% | 6% | 0:03:34.963657 | 116 µs | 537 ns |
| 784 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.7 µs | 24 m | 57 µs| 12% | 74% | 0:00:35.002236 | 35 µs | 993 ns |
| 785 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.0 µs | 27 ms | 65 µs| 33% | 72% | 0:00:16.001354 | 38 µs | 2.4 µs |
| 786 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.6 µs | 5.4 µs | 115 µs| 33% | 94% | 0:00:12.137542 | 19 µs | 1.6 µs |
| 825 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 8.9 µs | 18 µs | 89 µs| 0% | 10% | 0:07:45.962320 | 957 µs | 2.1 µs |
| 826 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 8.0 µs | 21 µs | 82 µs| 0% | 21% | 0:07:13.918505 | 755 µs | 1.7 µs |
| 828 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.7 µs | 26 ms | 67 µs| 33% | 70% | 0:00:17.003975 | 27 µs | 1.6 µs |
| 828 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 8.2 µs | 67 µs| 11% | 98% | 0:00:11.002354 | 5.7 µs | 520 ns |
| 826 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 19 µs | 63 µs| 12% | 5% | 0:03:56.969831 | 114 µs | 481 ns |
| 829 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.6 µs | 27 ms | 64 µs| 33% | 72% | 0:00:15.001748 | 30 µs | 2.0 µs |
| 786 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 5.0 µs | 118 µs| 10% | 99% | 0:00:33.278092 | 18 µs | 553 ns |
| 830 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.2 µs | 5.2 µs | 109 µs| 33% | 93% | 0:00:22.272355 | 10 µs | 453 ns |
| 830 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 µs | 8.3 µs | 121 µs| 11% | 86% | 0:00:27.390885 | 28 µs | 1.0 µs |
| 827 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.1 µs | 16 m | 57 µs| 12% | 71% | 0:00:34.002568 | 20 µs | 594 ns |
| 871 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 248 ms | 321 ms | 222 µs| 11% | 7% | 0:07:10.967817 | 255 µs | 592 ns |
| 870 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 2.7 µs | 434 ms | 115 µs| 12% | 13% | 0:04:11.935445 | 119 µs | 471 ns |
| 870 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 360 ms | 436 ms | 220 µs| 12% | 10% | 0:06:57.849871 | 246 µs | 590 ns |
| 879 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 184 ns | 493 ns | 75 µs| 10% | 89% | 0:00:26.351852 | 40 µs | 1.5 µs |
| 879 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 164 ns | 492 ns | 75 µs| 10% | 90% | 0:00:14.154972 | 36 µs | 2.6 µs |
| 877 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 358 ns | 13 µs | 37 µs| 11% | 98% | 0:00:13.999893 | 341 ms | 24 ms |
| 877 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 358 ns | 11 µs | 37 µs| 11% | 99% | 0:00:11.999149 | 180 ms | 15 ms |
| 878 | Hardware Fault (Master) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 753 ns | 187 ms | 78 µs| 10% | 75% | 0:00:14.002570 | 12 µs | 875 ns |
| 878 | Hardware Fault (Master) | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 701 ns | 187 ms | 78 µs| 10% | 74% | 0:00:20.210523 | 18 µs | 906 ns |
| 1392 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 224 ns | 2.2 µs | 37 µs| 10% | 95% | 0:00:34.928905 | 517 ms | 15 ms |
| 831 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 6.0 µs | 119 µs| 10% | 93% | 0:00:24.285282 | 30 µs | 1.3 µs |
| 784 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 24 m | 57 µs| 12% | 72% | 0:00:11.007507 | 11 µs | 973 ns |
| 871 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 3.0 µs | 319 ms | 115 µs| 11% | 11% | 0:04:21.137366 | 124 µs | 477 ns |
| 1392 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 217 ns | 1.2 µs | 37 µs| 10% | 95% | 0:00:11.985698 | 2.9 µs | 242 ns |
| 829 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 9.5 µs | 67 µs| 11% | 97% | 0:00:12.002461 | 20 µs | 1.7 µs |
| 785 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 8.9 µs | 67 µs| 11% | 98% | 0:00:14.004564 | 4.0 µs | 283 ns |
| 783 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 110 µs | 61 µs| 12% | 9% | 0:00:55.976956 | 75 µs | 1.3 µs |
| 1485 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 333 ns | 2.1 µs | 37 µs| 12% | 96% | 0:00:14.002773 | 375 ms | 27 ms |
| 1483 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.8 µs | 12 m | 57 µs| 12% | 72% | 0:00:28.997250 | 16 µs | 562 ns |
| 1483 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 3.4 µs | 12 m | 57 µs| 12% | 71% | 0:00:32.002590 | 41 µs | 1.3 µs |
| 1484 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.2 ms | 35 ms | 99 µs| 12% | 5% | 0:08:20.993646 | 311 µs | 620 ns |
| 1484 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 3.5 ms | 35 ms | 78 µs| 12% | 3% | 0:08:43.997829 | 459 µs | 877 ns |
| 1485 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 326 ns | 1.1 µs | 37 µs| 12% | 97% | 0:00:12.000117 | 347 ms | 29 ms |
| 1486 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 227 ns | 830 ns | 37 µs| 10% | 96% | 0:00:30.937320 | 152 ms | 4.9 ms |
| 1486 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 204 ns | 1.2 µs | 37 µs| 10% | 96% | 0:00:29.965687 | 328 ms | 11 ms |
| 1487 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 262 ns | 8.7 µs | 75 µs| 10% | 73% | 0:00:17.196610 | 46 µs | 2.7 µs |
| 1487 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 178 ns | 484 ns | 75 µs| 10% | 96% | 0:00:14.168007 | 36 µs | 2.5 µs |
| 1488 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 336 ns | 1.0 µs | 37 µs| 12% | 97% | 0:00:10 | 560 ms | 56 ms |
| 1488 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 328 ns | 1.0 µs | 37 µs| 12% | 99% | 0:00:10.000893 | 494 ms | 49 ms |
| 1489 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 215 ns | 1.2 µs | 37 µs| 10% | 95% | 0:00:23.970435 | 15 ms | 626 µs |
| 1489 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 216 ns | 1.3 µs | 37 µs| 10% | 95% | 0:00:26.855992 | 8.4 ms | 311 µs |
| 1490 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 188 ns | 563 ns | 75 µs| 10% | 90% | 0:00:15.215552 | 6.2 µs | 408 ns |
| 1490 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 196 ns | 529 ns | 75 µs| 10% | 86% | 0:00:11.130615 | 35 µs | 3.1 µs |
| 1707 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.5 µs | 4.5 µs | 113 µs| 33% | 91% | 0:00:10 | 22 µs | 2.2 µs |
| 1705 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 5.0 µs | 24 m | 58 µs| 12% | 72% | 0:00:18.002053 | 25 µs | 1.4 µs |
| 1710 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 198 ns | 810 ns | 37 µs| 10% | 96% | 0:00:28.975217 | 110 ms | 3.8 ms |
| 1728 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 289 µs | 61 µs| 12% | 4% | 0:05:14.969300 | 216 µs | 686 ns |
| 1729 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.4 µs | 23 m | 57 µs| 12% | 71% | 0:01:27.005843 | 53 µs | 610 ns |
| 1731 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 µs | 6.3 µs | 118 µs| 11% | 75% | 0:00:21.270647 | 16 µs | 760 ns |
| 1731 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.8 µs | 5.1 µs | 109 µs| 33% | 56% | 0:00:33.410524 | 37 µs | 1.1 µs |
| 1704 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 284 µs | 63 µs| 12% | 4% | 0:04:32.977550 | 212 µs | 776 ns |
| 1704 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 12 µs | 24 µs | 81 µs| 0% | 8% | 0:07:03.902462 | 1.0 ms | 2.4 µs |
| 1705 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.8 µs | 24 m | 58 µs| 12% | 75% | 0:00:14.000599 | 23 µs | 1.6 µs |
| 1706 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 9.1 µs | 67 µs| 11% | 97% | 0:00:10.002561 | 21 µs | 2.1 µs |
| 1706 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 7.2 µs | 37 ms | 65 µs| 33% | 55% | 0:00:20.004588 | 41 µs | 2.1 µs |
| 1707 | Hardware Fault (Master) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 6.8 µs | 120 µs| 11% | 81% | 0:00:21.208912 | 25 µs | 1.2 µs |
| 1733 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 350 ns | 1.0 µs | 37 µs| 11% | 97% | 0:00:12.997792 | 14 ms | 1.1 ms |
| 1733 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 334 ns | 1.0 µs | 37 µs| 11% | 98% | 0:00:12.999913 | 601 ms | 46 ms |
| 1708 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 292 ms | 350 ms | 231 µs| 11% | 4% | 0:08:23.006596 | 313 µs | 622 ns |
| 1708 | Hardware Fault (Master) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 299 ms | 351 ms | 232 µs| 11% | 1% | 0:08:44.026665 | 463 µs | 883 ns |
| 1734 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 219 ns | 884 ns | 37 µs| 10% | 96% | 0:00:28.982494 | 59 ms | 2.0 ms |
| 1734 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 218 ns | 880 ns | 37 µs| 10% | 96% | 0:00:30.933866 | 225 ms | 7.3 ms |
| 1709 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 338 ns | 1.0 µs | 37 µs| 11% | 98% | 0:00:15.001378 | 586 ms | 39 ms |
| 1709 | Hardware Fault (Master) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 324 ns | 1.0 µs | 37 µs| 11% | 98% | 0:00:10 | 114 ms | 11 ms |
| 1735 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 167 ns | 8.1 µs | 75 µs| 10% | 86% | 0:00:11.121413 | 6.1 µs | 545 ns |
| 1735 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 180 ns | 511 ns | 75 µs| 10% | 89% | 0:00:13.124064 | 1.7 µs | 133 ns |
| 1710 | Hardware Fault (Master) | SPTP | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 232 ns | 905 ns | 37 µs| 10% | 95% | 0:00:31.942945 | 293 ms | 9.2 ms |
| 1711 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 207 ns | 664 ns | 75 µs| 10% | 82% | 0:00:21.230883 | 5.2 µs | 243 ns |
| 1711 | Hardware Fault (Master) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 177 ns | 573 ns | 75 µs| 10% | 93% | 0:00:14.118939 | 42 µs | 2.9 µs |
| 1728 | Hardware Fault (Master) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 8.2 µs | 20 µs | 65 µs| 0% | 39% | 0:04:38.969542 | 211 µs | 755 ns |
| 1729 | Hardware Fault (Master) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.2 µs | 23 m | 57 µs| 12% | 73% | 0:00:19.001469 | 17 µs | 911 ns |
| 1730 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 9.0 µs | 67 µs| 11% | 97% | 0:00:17.008612 | 15 µs | 885 ns |
| 1730 | Hardware Fault (Master) | SPTP | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 7.2 µs | 37 ms | 65 µs| 33% | 57% | 0:00:12.999679 | 42 µs | 3.3 µs |
### Benchmark: Hardware Fault (Failover)
_Id: `fault/hardware/master_failover`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on the master but with a failover master on the secondary slave that will take over once the primary master fails. The fault occurs 10 minutes into the benchmark and lasts for 1 minute. After the fault is resolved, the failover master will be demoted back to a slave, allowing the primary master to take over again. The benchmark is expected to show a seamless transition between the primary and failover masters. The hardware fault is created by turning off the power to the master machine using a smart PDU (check the documentation on how to register it with PTP-Perf). 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 821 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 8.0 µs | 119 µs| 4% | 89% | 0:00:10 | 1 m | 6 s |
| 819 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.2 µs | 18 µs | 73 µs| 0% | 10% | 0:07:22.968231 | 773 µs | 1.7 µs |
| 820 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.7 µs | 23 m | 57 µs| 2% | 67% | 0:00:22.001776 | 21 µs | 977 ns |
| 790 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 108 µs | 62 µs| 12% | 10% | 0:01:04.979709 | 80 µs | 1.2 µs |
| 821 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.2 µs | 4.4 µs | 114 µs| 33% | 100% | 0:00:19.160027 | 18 µs | 913 ns |
| 790 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.8 µs | 18 µs | 72 µs| 0% | 14% | 0:06:47.937627 | 757 µs | 1.9 µs |
| 791 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.7 µs | 38 m | 57 µs| 3% | 73% | 0:00:19.001432 | 13 µs | 666 ns |
| 820 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.0 µs | 23 m | 57 µs| 12% | 67% | 0:01:31.005156 | 24 µs | 261 ns |
| 791 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.9 µs | 38 m | 57 µs| 12% | 63% | 0:00:12.000932 | 26 µs | 2.2 µs |
| 792 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 9.7 µs | 121 µs| 4% | 85% | 0:00:10 | 1 m | 6 s |
| 792 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 µs | 4.4 µs | 116 µs| 33% | 94% | 0:00:16.156617 | 16 µs | 991 ns |
| 880 | Hardware Fault (Failover) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 2.3 µs | 41 ms | 114 µs| 12% | 17% | 0:04:55.700061 | 121 µs | 410 ns |
| 883 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 190 ns | 516 ns | 75 µs| 10% | 92% | 0:00:13.370425 | 28 µs | 2.1 µs |
| 883 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 180 ns | 522 ns | 75 µs| 0% | 94% | 0:00:10 | 1 m | 6 s |
| 881 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 322 ns | 1.0 µs | 37 µs| 1% | 97% | 0:00:15.000248 | 140 ms | 9.3 ms |
| 880 | Hardware Fault (Failover) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.1 ms | 45 ms | 96 µs| 12% | 4% | 0:07:30.922509 | 251 µs | 557 ns |
| 1393 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 11 µs | 24 µs | 81 µs| 0% | 5% | 0:06:45.909861 | 766 µs | 1.9 µs |
| 1393 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 286 µs | 61 µs| 12% | 7% | 0:05:03.936755 | 210 µs | 692 ns |
| 1395 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.6 µs | 5.6 µs | 118 µs| 33% | 99% | 0:00:14.171091 | 28 µs | 2.0 µs |
| 1395 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.6 µs | 8.6 µs | 121 µs| 4% | 87% | 0:00:10 | 1 m | 6 s |
| 819 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 107 µs | 61 µs| 12% | 8% | 0:00:52.967428 | 74 µs | 1.4 µs |
| 1712 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 8.9 µs | 19 µs | 69 µs| 0% | 29% | 0:04:50.133583 | 210 µs | 725 ns |
| 1715 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.4 µs | 6.0 µs | 112 µs| 33% | 85% | 0:00:26.307403 | 27 µs | 1.0 µs |
| 1737 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 5.0 µs | 26 m | 58 µs| 12% | 73% | 0:00:31.003543 | 48 µs | 1.6 µs |
| 1739 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 1.6 µs | 6.6 µs | 115 µs| 33% | 76% | 0:00:12.151427 | 39 µs | 3.2 µs |
| 1750 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 12 m | 58 µs| 3% | 75% | 0:00:13.001257 | 16 µs | 1.2 µs |
| 1719 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 183 ns | 577 ns | 75 µs| 10% | 94% | 0:00:11.121677 | 7.1 µs | 635 ns |
| 1719 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 190 ns | 3.6 µs | 75 µs| 0% | 88% | 0:00:10.948575 | 44 µs | 4.0 µs |
| 1736 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 291 µs | 63 µs| 12% | 7% | 0:04:37.900499 | 212 µs | 761 ns |
| 1736 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 6.7 µs | 19 µs | 67 µs| 0% | 42% | 0:04:41.975542 | 209 µs | 743 ns |
| 1737 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.0 µs | 26 m | 58 µs| 3% | 74% | 0:00:40.002774 | 21 µs | 521 ns |
| 1750 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 4.2 µs | 12 m | 57 µs| 12% | 69% | 0:02:02.010091 | 42 µs | 343 ns |
| 1712 | Hardware Fault (Failover) | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 287 µs | 63 µs| 12% | 4% | 0:04:22.977795 | 224 µs | 853 ns |
| 1761 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 349 ns | 1.0 µs | 37 µs| 11% | 96% | 0:00:10 | 164 ms | 16 ms |
| 1713 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.8 µs | 1 h | 57 µs| 3% | 76% | 0:00:10 | 14 µs | 1.4 µs |
| 1713 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 4 | rpi07 | SECONDARY_SLAVE | 5.2 µs | 1 h | 57 µs| 12% | 58% | 0:00:18.001175 | 36 µs | 2.0 µs |
| 1739 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.7 µs | 8.9 µs | 122 µs| 5% | 81% | 0:00:10 | 1 m | 6 s |
| 1752 | Hardware Fault (Failover) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.8 µs | 8.9 ms | 115 µs| 12% | 9% | 0:06:10.993827 | 74 µs | 198 ns |
| 1752 | Hardware Fault (Failover) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 2.2 ms | 15 ms | 151 µs| 12% | 1% | 0:08:44.002486 | 463 µs | 883 ns |
| 1763 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 219 ns | 5.6 µs | 75 µs| 0% | 92% | 0:00:11.142788 | 1 m | 5 s |
| 1763 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 220 ns | 7.9 µs | 75 µs| 10% | 81% | 0:00:13.115769 | 38 µs | 2.9 µs |
| 1715 | Hardware Fault (Failover) | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 µs | 8.3 µs | 123 µs| 5% | 92% | 0:00:10 | 1 m | 6 s |
| 1741 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 379 ns | 12 µs | 37 µs| 11% | 98% | 0:00:11.000981 | 309 ms | 28 ms |
| 1741 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 362 ns | 5.2 µs | 37 µs| 1% | 98% | 0:00:10.001876 | 730 ms | 73 ms |
| 1753 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 354 ns | 992 ns | 37 µs| 11% | 100% | 0:00:13.998840 | 578 ms | 41 ms |
| 1743 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 227 ns | 3.0 µs | 75 µs| 0% | 77% | 0:00:10 | 1 m | 6 s |
| 1743 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 175 ns | 500 ns | 75 µs| 10% | 96% | 0:00:12.112432 | 38 µs | 3.1 µs |
| 1811 | Hardware Fault (Failover) | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 870 µs | 8.9 ms | 141 µs| 12% | 0% | 0:09:25.012058 | 913 µs | 1.6 µs |
| 1761 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 333 ns | 1.0 µs | 37 µs| 1% | 98% | 0:00:14.001614 | 328 ms | 23 ms |
| 1811 | Hardware Fault (Failover) | PTPd | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 707 µs | 6.3 ms | 134 µs| 12% | 0.6% | 0:08:39.006369 | 464 µs | 893 ns |
| 1753 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 328 ns | 1.0 µs | 37 µs| 1% | 98% | 0:00:10.000526 | 72 ms | 7.2 ms |
| 881 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 338 ns | 1.0 µs | 37 µs| 11% | 96% | 0:00:12.999999 | 265 ms | 20 ms |
| 1717 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 364 ns | 2.5 µs | 37 µs| 11% | 97% | 0:00:10 | 34 ms | 3.4 ms |
| 1717 | Hardware Fault (Failover) | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 352 ns | 1.3 µs | 37 µs| 1% | 97% | 0:00:12.000814 | 738 ms | 62 ms |
| 1812 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 236 ns | 6.0 µs | 75 µs| 0% | 94% | 0:00:10 | 1 m | 6 s |
| 1812 | Hardware Fault (Failover) | Chrony | Raspberry Pi 5 | rpi57 | SECONDARY_SLAVE | 234 ns | 8.7 µs | 75 µs| 10% | 75% | 0:00:20.270427 | 5.5 µs | 269 ns |
### Benchmark: No Switch
_Id: `configuration/no_switch`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster without a network switch. The configuration is identical to the baseline, the user is expected to rewire the cluster appropriately before running this benchmark. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Resource Consumption
_Id: `resource_consumption`, 2 machines, 0:20:00 duration._

A benchmark to measure the resource consumption of the PTP applications on each node. Collected metrics include CPU usage, memory usage, network traffic, and clock synchronization statistics. The benchmark runs for 15 minutes to collect a sufficient amount of data. It is otherwise identical to the base benchmark.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 856 | Resource Consumption | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 530 ns | 1.7 µs | 79 µs| - | - | 0:00:01 | 39 µs | 39 µs |
| 864 | Resource Consumption | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 474 ns | 1.7 µs | 79 µs| - | - | 0:00:01 | 36 µs | 36 µs |
| 850 | Resource Consumption | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.7 µs | 21 µs | 71 µs| - | - | 0:03:24.916570 | 130 µs | 633 ns |
| 859 | Resource Consumption | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.2 µs | 15 µs | 64 µs| - | - | 0:00:01 | 8.4 µs | 8.4 µs |
| 857 | Resource Consumption | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 164 ns | 436 ns | 75 µs| - | - | 0:00:01 | 5.6 µs | 5.6 µs |
| 855 | Resource Consumption | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 321 ns | 909 ns | 37 µs| - | - | 0:00:01 | 566 ms | 566 ms |
| 854 | Resource Consumption | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.4 µs | 4.4 µs | 118 µs| - | - | 0:07:23.986592 | 253 µs | 570 ns |
| 853 | Resource Consumption | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 8.1 µs | 132 µs| - | - | 0:00:01 | 7.4 µs | 7.4 µs |
| 852 | Resource Consumption | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 7.9 µs | 72 µs| - | - | 0:00:01 | 14 µs | 14 µs |
| 849 | Resource Consumption | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 165 ns | 436 ns | 75 µs| - | - | 0:00:01 | 1.9 µs | 1.9 µs |
| 863 | Resource Consumption | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 326 ns | 856 ns | 37 µs| - | - | 0:00:01 | 56 ms | 56 ms |
| 862 | Resource Consumption | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.2 µs | 4.4 µs | 118 µs| - | - | 0:07:41.923136 | 251 µs | 543 ns |
| 861 | Resource Consumption | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.4 µs | 8.4 µs | 132 µs| - | - | 0:00:01 | 21 µs | 21 µs |
| 860 | Resource Consumption | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 7.8 µs | 72 µs| - | - | 0:00:01 | 13 µs | 13 µs |
| 858 | Resource Consumption | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 17 µs | 69 µs| - | - | 0:04:17.977315 | 117 µs | 452 ns |
| 851 | Resource Consumption | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.6 µs | 16 µs | 64 µs| - | - | 0:00:01 | 2.4 µs | 2.4 µs |
### Benchmark: Unprioritized Network 10% Load
_Id: `load/net_unprioritized/load_10`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 10% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 10% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 100 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1120 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.2 µs | 36 µs | 102 µs| 0% | 56% | 0:00:29.284225 | 39 µs | 1.3 µs |
| 1134 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.4 µs | 23 µs | 56 µs| 0% | 14% | 0:02:57.443117 | 110 µs | 618 ns |
| 1103 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.9 µs | 39 µs | 101 µs| 0% | 46% | 0:00:12.127677 | 13 µs | 1.0 µs |
| 1136 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 204 µs | 59 µs| 0% | 90% | 0:00:14.976857 | 11 µs | 740 ns |
| 1182 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.6 µs | 20 µs | 76 µs| 0% | 16% | 0:03:31.980175 | 113 µs | 533 ns |
| 1184 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 137 µs | 58 µs| 0% | 84% | 0:00:11.005236 | 13 µs | 1.2 µs |
| 1200 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 15 µs | 52 µs| 0% | 91% | 0:00:16.002669 | 8.5 µs | 532 ns |
| 1233 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 45 µs | 106 µs| 0% | 80% | 0:00:17.167468 | 391 µs | 23 µs |
| 1217 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 159 µs | 58 µs| 0% | 95% | 0:00:16.003520 | 203 µs | 13 µs |
| 1215 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 12 µs | 56 µs| 0% | 7% | 0:05:13.959160 | 230 µs | 733 ns |
| 1232 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 µs | 37 µs | 58 µs| 0% | 98% | 0:00:13.781173 | 46 µs | 3.4 µs |
| 1231 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 µs | 11 µs | 52 µs| 0% | 87% | 0:01:23.002482 | 25 µs | 303 ns |
| 1169 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 73 µs | 105 µs| 0% | 64% | 0:00:10 | 9.1 µs | 912 ns |
| 1152 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 66 µs | 58 µs| 0% | 90% | 0:00:15.936416 | 67 µs | 4.2 µs |
| 1151 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 22 µs | 52 µs| 0% | 91% | 0:00:19.001653 | 8.7 µs | 460 ns |
| 1101 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 µs | 12 µs | 53 µs| 0% | 92% | 0:00:29.000041 | 4.4 µs | 153 ns |
| 1102 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 36 µs | 56 µs| 0% | 92% | 0:00:11.003747 | 13 µs | 1.1 µs |
| 1100 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 14 µs | 69 µs| 0% | 5% | 0:04:24.974175 | 123 µs | 464 ns |
| 1216 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 9.7 µs | 52 µs| 0% | 93% | 0:00:32.004575 | 13 µs | 396 ns |
| 1218 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 151 µs | 101 µs| 0% | 55% | 0:00:14.176010 | 257 µs | 18 µs |
| 1183 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 µs | 12 µs | 53 µs| 0% | 91% | 0:00:22.001294 | 6.4 µs | 291 ns |
| 1150 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.8 µs | 17 µs | 72 µs| 0% | 10% | 0:04:17.916606 | 112 µs | 436 ns |
| 1198 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.8 µs | 13 µs | 57 µs| 0% | 6% | 0:05:20.972570 | 94 µs | 292 ns |
| 1168 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 293 µs | 58 µs| 0% | 83% | 0:00:10 | 7.6 µs | 756 ns |
| 1249 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.8 µs | 52 µs | 101 µs| 0% | 69% | 0:00:21.203495 | 403 µs | 19 µs |
| 1137 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 179 µs | 102 µs| 0% | 80% | 0:00:10.110633 | 316 µs | 31 µs |
| 1202 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.1 µs | 57 µs | 102 µs| 0% | 54% | 0:00:12.117358 | 351 µs | 29 µs |
| 1166 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 13 µs | 56 µs| 0% | 7% | 0:03:59.980765 | 106 µs | 443 ns |
| 1135 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 µs | 12 µs | 53 µs| 0% | 91% | 0:00:22.000978 | 30 µs | 1.4 µs |
| 1118 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 µs | 11 µs | 52 µs| 0% | 96% | 0:00:58.004268 | 7.6 µs | 131 ns |
| 1117 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.8 µs | 17 µs | 69 µs| 0% | 17% | 0:04:31.882962 | 114 µs | 419 ns |
| 1185 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 50 µs | 106 µs| 0% | 58% | 0:00:44.144817 | 526 µs | 12 µs |
| 1119 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 59 µs | 56 µs| 0% | 94% | 0:00:10 | 34 µs | 3.4 µs |
| 1248 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 30 µs | 56 µs| 3% | 95% | 0:00:10 | 13 µs | 1.3 µs |
| 1246 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 18 µs | 57 µs| 0% | 1% | 0:05:06.966300 | 216 µs | 703 ns |
| 1247 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 16 µs | 53 µs| 0.3% | 89% | 0:00:17.941698 | 15 µs | 818 ns |
| 2059 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 336 ns | 7.1 µs | 37 µs| 0.3% | 97% | 0:00:36.719508 | 728 ms | 20 ms |
| 1335 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 µs | 11 µs | 53 µs| 0% | 89% | 0:00:23.016987 | 6.1 µs | 265 ns |
| 1336 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 26 µs | 59 µs| 0% | 98% | 0:00:13.564387 | 16 µs | 1.2 µs |
| 1337 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.1 µs | 73 µs | 106 µs| 0% | 94% | 0:00:17.623496 | 15 µs | 834 ns |
| 1167 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 12 µs | 52 µs| 0% | 90% | 0:00:18.002085 | 7.4 µs | 411 ns |
| 1153 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 976 ns | 39 µs | 104 µs| 0% | 85% | 0:00:14.185705 | 47 µs | 3.3 µs |
| 1201 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 µs | 83 µs | 59 µs| 0% | 96% | 0:00:17.003399 | 108 µs | 6.4 µs |
| 1616 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 µs | 11 µs | 52 µs| 0% | 87% | 0:00:33.002185 | 19 µs | 581 ns |
| 1615 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 17 µs | 74 µs| 0% | 7% | 0:04:45.527157 | 219 µs | 766 ns |
| 1767 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 µs | 140 µs | 58 µs| 0% | 93% | 0:00:19.771342 | 163 µs | 8.3 µs |
| 1768 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 58 µs | 105 µs| 0% | 87% | 0:00:11.137574 | 269 µs | 24 µs |
| 1835 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.7 µs | 12 µs | 73 µs| 0% | 9% | 0:05:44.973781 | 232 µs | 672 ns |
| 1838 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 µs | 32 µs | 105 µs| 0% | 66% | 0:00:14.948482 | 7.9 µs | 530 ns |
| 1836 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 11 µs | 53 µs| 0% | 81% | 0:00:13.004743 | 12 µs | 925 ns |
| 1837 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 µs | 37 µs | 58 µs| 0% | 95% | 0:00:12.742970 | 37 µs | 2.9 µs |
| 1869 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 µs | 9.0 µs | 53 µs| 2% | 84% | 0:02:28.008985 | 62 µs | 419 ns |
| 1864 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 9.8 µs | 52 µs| 0% | 86% | 0:00:18.001477 | 8.3 µs | 459 ns |
| 1888 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.6 µs | 9.7 µs | 67 µs| 0% | 2% | 0:06:22.976589 | 225 µs | 587 ns |
| 1914 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 13 µs | 69 µs| 0% | 7% | 0:05:28.963467 | 239 µs | 728 ns |
| 1889 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 28 µs | 59 µs| 0% | 96% | 0:00:13.709536 | 49 µs | 3.6 µs |
| 1890 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 55 µs | 105 µs| 0% | 88% | 0:00:32.848450 | 44 µs | 1.3 µs |
| 1915 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 37 µs | 59 µs| 0% | 96% | 0:00:10 | 6.7 µs | 675 ns |
| 1916 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 30 µs | 104 µs| 0% | 80% | 0:00:11.607267 | 16 µs | 1.4 µs |
| 2057 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.7 µs | 6.2 µs | 125 µs| 0% | 10% | 0:09:00.995154 | 910 µs | 1.7 µs |
| 2058 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 458 ns | 9.0 µs | 37 µs| 27% | 94% | 0:00:13.002584 | 494 ms | 38 ms |
| 2094 | Unprioritized Network 10% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 377 ns | 7.6 µs | 37 µs| 0% | 95% | 0:00:32.983191 | 173 ms | 5.2 ms |
| 2060 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.2 µs | 13 µs | 75 µs| 0% | 66% | 0:00:10 | 6.1 µs | 607 ns |
| 2092 | Unprioritized Network 10% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.2 µs | 18 µs | 141 µs| 0% | 2% | 0:09:20.015819 | 908 µs | 1.6 µs |
| 2093 | Unprioritized Network 10% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 427 ns | 5.3 µs | 37 µs| 7% | 93% | 0:00:21.003228 | 205 ms | 9.8 ms |
| 2095 | Unprioritized Network 10% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.4 µs | 8.9 µs | 75 µs| 0% | 64% | 0:00:10.957006 | 30 µs | 2.7 µs |
### Benchmark: Unprioritized Network 20% Load
_Id: `load/net_unprioritized/load_20`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 20% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 20% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 200 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 72 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.9 µs | 42 µs | 55 µs| 0% | 79% | 0:00:10 | 2.6 µs | 262 ns |
| 69 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 30 µs | 78 µs | 84 µs| 0% | 11% | 0:01:24.887683 | 147 µs | 1.7 µs |
| 67 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 49 µs | 72 µs| 0% | 5% | 0:02:29.325880 | 129 µs | 866 ns |
| 71 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.8 µs | 45 µs | 75 µs| 0% | 3% | 0:02:35.654250 | 154 µs | 989 ns |
| 70 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 30 µs | 55 µs| 0% | 59% | 0:01:08.544476 | 201 µs | 2.9 µs |
| 65 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 44 µs | 90 µs| 0% | 4% | 0:03:44.840160 | 115 µs | 510 ns |
| 66 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 21 µs | 55 µs| 0% | 65% | 0:00:15.002347 | 15 µs | 1.0 µs |
| 433 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.2 µs | 259 µs | 104 µs| 0% | 78% | 0:00:17.537419 | 40 µs | 2.3 µs |
| 210 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 42 µs | 58 µs| 0% | 87% | 0:00:14.004578 | 44 µs | 3.2 µs |
| 211 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.1 µs | 182 µs | 105 µs| 0% | 58% | 0:00:27.100769 | 428 µs | 16 µs |
| 195 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 58 µs | 107 µs| 0% | 68% | 0:00:18.885160 | 116 µs | 6.2 µs |
| 203 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.7 µs | 164 µs | 105 µs| 0% | 50% | 0:00:15.075847 | 250 µs | 17 µs |
| 193 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 32 µs | 52 µs| 0% | 70% | 0:00:26.999874 | 2.3 µs | 84 ns |
| 270 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 4.9 µs | 13 µs | 75 µs| - | - | 0:00:01 | 5.2 µs | 5.2 µs |
| 439 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 49 µs | 52 µs| 0% | 55% | 0:02:34.007388 | 89 µs | 575 ns |
| 432 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.4 µs | 36 µs | 56 µs| 0% | 88% | 0:00:20.650496 | 35 µs | 1.7 µs |
| 476 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.9 µs | 12 µs | 59 µs| 0% | 9% | 0:00:32.962719 | 52 µs | 1.6 µs |
| 477 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.8 µs | 33 µs | 52 µs| 0% | 69% | 0:00:10.000872 | 3.3 µs | 334 ns |
| 267 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 8.0 µs | 31 µs | 215 µs| - | - | 0:09:05.000214 | 423 µs | 776 ns |
| 279 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.5 µs | 13 µs | 75 µs| - | - | 0:00:01 | 5.8 µs | 5.8 µs |
| 473 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 8.6 µs | 57 µs| 0% | 6% | 0:00:52.968072 | 43 µs | 803 ns |
| 489 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 52 µs | 104 µs| 0% | 72% | 0:00:10 | 90 µs | 9.0 µs |
| 488 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 72 µs | 106 µs| 0% | 77% | 0:00:22.271960 | 79 µs | 3.5 µs |
| 486 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 48 µs | 105 µs| 0% | 72% | 0:00:17.939681 | 115 µs | 6.4 µs |
| 484 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 226 µs | 58 µs| 0% | 99% | 0:00:13.862390 | 287 µs | 21 µs |
| 482 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 256 µs | 58 µs| 0% | 89% | 0:00:14.136756 | 403 µs | 28 µs |
| 480 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 375 µs | 57 µs| 0% | 94% | 0:00:18.822876 | 519 µs | 28 µs |
| 474 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.8 µs | 14 µs | 60 µs| 0% | 10% | 0:00:44.974652 | 53 µs | 1.2 µs |
| 472 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 14 µs | 104 µs| 0% | 5% | 0:00:45.974898 | 73 µs | 1.6 µs |
| 487 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.4 µs | 142 µs | 105 µs| 0% | 53% | 0:00:12.621982 | 188 µs | 15 µs |
| 481 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.8 µs | 361 µs | 58 µs| 0% | 86% | 0:00:13.948873 | 95 µs | 6.8 µs |
| 478 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 20 µs | 52 µs| 0% | 75% | 0:01:44.009801 | 35 µs | 340 ns |
| 1252 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.9 µs | 39 µs | 58 µs| 0.3% | 88% | 0:00:10 | 9.5 µs | 953 ns |
| 1251 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.9 µs | 19 µs | 52 µs| 0% | 69% | 0:00:10 | 2.9 µs | 288 ns |
| 1250 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.7 µs | 12 µs | 96 µs| 0% | 8% | 0:05:38.392206 | 380 µs | 1.1 µs |
| 1253 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.6 µs | 61 µs | 104 µs| 0% | 43% | 0:00:21.435706 | 423 µs | 20 µs |
| 1339 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.8 µs | 44 µs | 52 µs| 0% | 64% | 0:00:15.003722 | 8.7 µs | 578 ns |
| 1340 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.3 µs | 354 µs | 57 µs| 0% | 79% | 0:00:26.232274 | 393 µs | 15 µs |
| 1341 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.8 µs | 235 µs | 104 µs| 0% | 54% | 0:00:11.749918 | 357 µs | 30 µs |
| 63 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 22 µs | 49 µs | 75 µs| 0% | 7% | 0:02:46.986044 | 132 µs | 789 ns |
| 194 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.0 µs | 42 µs | 58 µs| 0% | 90% | 0:00:15.936056 | 30 µs | 1.9 µs |
| 68 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 20 µs | 56 µs| 0.3% | 73% | 0:01:00.821091 | 86 µs | 1.4 µs |
| 490 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.5 µs | 214 µs | 105 µs| 0% | 59% | 0:02:08.960175 | 509 µs | 3.9 µs |
| 485 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 305 µs | 57 µs| 0% | 89% | 0:00:10 | 282 µs | 28 µs |
| 202 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 143 µs | 58 µs| 0% | 96% | 0:00:13.805795 | 127 µs | 9.2 µs |
| 475 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.8 µs | 17 µs | 98 µs| 0% | 5% | 0:00:32.983508 | 140 µs | 4.2 µs |
| 483 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.7 µs | 41 µs | 57 µs| 0% | 81% | 0:00:21.935344 | 30 µs | 1.4 µs |
| 479 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 44 µs | 52 µs| 0% | 73% | 0:00:16.999543 | 3.2 µs | 186 ns |
| 434 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 230 µs | 105 µs| 0% | 70% | 0:00:13.833762 | 286 µs | 21 µs |
| 440 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.8 µs | 27 µs | 52 µs| 0% | 61% | 0:00:20.001801 | 24 µs | 1.2 µs |
| 1781 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 15 µs | 59 µs| 0% | 9% | 0:04:44.967830 | 233 µs | 819 ns |
| 1782 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 27 µs | 53 µs| 0% | 75% | 0:00:18.001986 | 26 µs | 1.4 µs |
| 1783 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.0 µs | 35 µs | 56 µs| 0% | 92% | 0:00:23.653719 | 52 µs | 2.2 µs |
| 1784 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.2 µs | 54 µs | 104 µs| 0% | 54% | 0:00:10 | 29 µs | 2.9 µs |
| 1841 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.1 µs | 46 µs | 57 µs| 0% | 95% | 0:00:11.966037 | 42 µs | 3.5 µs |
| 1842 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.0 µs | 149 µs | 101 µs| 0% | 66% | 0:00:12.144602 | 326 µs | 27 µs |
| 1839 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.5 µs | 13 µs | 78 µs| 0% | 5% | 0:05:46.909198 | 228 µs | 657 ns |
| 1840 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.6 µs | 23 µs | 52 µs| 0% | 71% | 0:04:49.017154 | 126 µs | 436 ns |
| 1865 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 18 µs | 52 µs| 0.7% | 71% | 0:00:33.003257 | 15 µs | 451 ns |
| 1891 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 22 µs | 90 µs| 0% | 8% | 0:04:28.843311 | 242 µs | 900 ns |
| 1892 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.4 µs | 311 µs | 57 µs| 0.3% | 80% | 0:00:13.996678 | 231 µs | 17 µs |
| 1893 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.8 µs | 63 µs | 101 µs| 0% | 39% | 0:00:12.126123 | 47 µs | 3.9 µs |
| 2069 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.0 µs | 7.9 µs | 37 µs| 0% | 72% | 0:00:35.724184 | 397 ms | 11 ms |
| 2097 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 690 ns | 18 µs | 37 µs| 40% | 89% | 0:00:19.001838 | 26 ms | 1.4 ms |
| 2067 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.0 µs | 10 µs | 166 µs| 0% | 1% | 0:10:02.243167 | 886 µs | 1.5 µs |
| 2068 | Unprioritized Network 20% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 664 ns | 16 µs | 37 µs| 38% | 88% | 0:00:15.001692 | 414 ms | 28 ms |
| 2070 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.2 µs | 13 µs | 75 µs| 0% | 74% | 0:00:10 | 16 µs | 1.6 µs |
| 2096 | Unprioritized Network 20% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 12 µs | 42 µs | 234 µs| 0% | 3% | 0:07:00.003043 | 926 µs | 2.2 µs |
| 2098 | Unprioritized Network 20% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.1 µs | 8.5 µs | 37 µs| 0% | 63% | 0:00:27.955380 | 72 ms | 2.6 ms |
| 2099 | Unprioritized Network 20% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.0 µs | 8.8 µs | 75 µs| 0% | 88% | 0:00:20.247313 | 35 µs | 1.7 µs |
### Benchmark: Unprioritized Network 33% Load
_Id: `load/net_unprioritized/load_33`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 33% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 33% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 330 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1107 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 283 µs | 104 µs| 0% | 30% | 0:00:15.179136 | 428 µs | 28 µs |
| 1105 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 86 µs | 52 µs| 0% | 39% | 0:00:40.003442 | 60 µs | 1.5 µs |
| 1155 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.0 µs | 34 µs | 52 µs| 2% | 36% | 0:01:09.007356 | 134 µs | 1.9 µs |
| 1156 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.8 µs | 38 µs | 60 µs| 0% | 92% | 0:00:12.006310 | 37 µs | 3.1 µs |
| 1154 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 12 µs | 67 µs| 0% | 5% | 0:05:28.975771 | 104 µs | 318 ns |
| 1157 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 323 µs | 104 µs| 0% | 52% | 0:00:56.516123 | 542 µs | 9.6 µs |
| 1186 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.7 µs | 13 µs | 127 µs| 0% | 4% | 0:04:42.975509 | 104 µs | 367 ns |
| 1189 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.4 µs | 87 µs | 101 µs| 0% | 30% | 0:00:15.178924 | 33 µs | 2.2 µs |
| 1237 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10.0 µs | 261 µs | 101 µs| 0% | 30% | 0:00:22.262232 | 371 µs | 17 µs |
| 1220 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.5 µs | 29 µs | 52 µs| 2% | 44% | 0:02:23.010153 | 70 µs | 491 ns |
| 1222 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.7 µs | 391 µs | 101 µs| 0% | 40% | 0:00:12.120341 | 335 µs | 28 µs |
| 1205 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 86 µs | 636 µs | 58 µs| 0% | 59% | 0:00:22.942983 | 475 µs | 21 µs |
| 1187 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.7 µs | 34 µs | 53 µs| 2% | 53% | 0:00:31.037089 | 53 µs | 1.7 µs |
| 1170 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.7 µs | 38 µs | 131 µs| 0% | 12% | 0:03:31.878287 | 173 µs | 817 ns |
| 1188 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 61 µs | 489 µs | 58 µs| 0.3% | 78% | 0:00:10.329115 | 470 µs | 45 µs |
| 1139 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 87 µs | 54 µs| 0% | 34% | 0:00:17.056065 | 104 µs | 6.1 µs |
| 1171 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 18 µs | 86 µs | 56 µs| 0% | 29% | 0:00:22.002444 | 82 µs | 3.7 µs |
| 1140 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 52 µs | 469 µs | 56 µs| 0% | 75% | 0:00:10 | 405 µs | 41 µs |
| 1138 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10.0 µs | 32 µs | 69 µs| 0% | 6% | 0:03:32.644957 | 155 µs | 727 ns |
| 1122 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 70 µs | 52 µs| 0% | 34% | 0:01:16.004685 | 157 µs | 2.1 µs |
| 1206 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.9 µs | 297 µs | 105 µs| 0% | 84% | 0:00:12.875232 | 168 µs | 13 µs |
| 1234 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.1 µs | 23 µs | 60 µs| 0% | 12% | 0:04:15.402474 | 213 µs | 835 ns |
| 1173 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.6 µs | 419 µs | 102 µs| 0% | 72% | 0:00:17.182399 | 461 µs | 27 µs |
| 1236 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.4 µs | 47 µs | 60 µs| 0% | 85% | 0:00:12.794945 | 35 µs | 2.7 µs |
| 1219 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.5 µs | 28 µs | 64 µs| 0% | 12% | 0:04:39.393127 | 227 µs | 813 ns |
| 1141 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.8 µs | 282 µs | 101 µs| 0% | 34% | 0:00:11.110848 | 546 µs | 49 µs |
| 1124 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 292 µs | 105 µs| 0% | 25% | 0:00:10 | 327 µs | 33 µs |
| 1104 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 15 µs | 126 µs| 0% | 3% | 0:05:16.973068 | 135 µs | 425 ns |
| 1106 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 55 µs | 58 µs| 0% | 92% | 0:00:12.004439 | 73 µs | 6.1 µs |
| 1221 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 45 µs | 368 µs | 58 µs| 0% | 82% | 0:00:18.811126 | 226 µs | 12 µs |
| 1203 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.9 µs | 32 µs | 121 µs| 0% | 9% | 0:03:52.411922 | 119 µs | 513 ns |
| 1204 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 29 µs | 52 µs| 2% | 42% | 0:00:23.997392 | 53 µs | 2.2 µs |
| 1257 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.5 µs | 270 µs | 105 µs| 0% | 62% | 0:00:13.570908 | 475 µs | 35 µs |
| 1255 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.5 µs | 23 µs | 52 µs| 0% | 52% | 0:00:36.002288 | 27 µs | 764 ns |
| 1256 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 39 µs | 413 µs | 58 µs| 0.4% | 82% | 0:00:17.426440 | 532 µs | 31 µs |
| 1254 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 40 µs | 70 µs| 0% | 12% | 0:03:19.258738 | 224 µs | 1.1 µs |
| 1343 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.5 µs | 24 µs | 52 µs| 0% | 46% | 0:00:37.004201 | 17 µs | 454 ns |
| 1344 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 167 µs | 61 µs| 5% | 76% | 0:00:10 | 44 µs | 4.4 µs |
| 1345 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 268 µs | 106 µs| 15% | 35% | 0:00:10 | 291 µs | 29 µs |
| 1172 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.3 µs | 43 µs | 60 µs| 0.3% | 79% | 0:00:17.653438 | 38 µs | 2.2 µs |
| 1121 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.0 µs | 30 µs | 61 µs| 0% | 17% | 0:03:46.978031 | 140 µs | 615 ns |
| 1235 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 88 µs | 52 µs| 0% | 43% | 0:04:35.019501 | 282 µs | 1.0 µs |
| 1123 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 62 µs | 58 µs| 0% | 92% | 0:00:20.007388 | 57 µs | 2.9 µs |
| 1785 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.6 µs | 26 µs | 121 µs| 0% | 7% | 0:04:03.910703 | 285 µs | 1.2 µs |
| 1786 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 71 µs | 53 µs| 0% | 36% | 0:00:31.001729 | 103 µs | 3.3 µs |
| 1787 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 52 µs | 436 µs | 58 µs| 0% | 75% | 0:00:15.999016 | 101 µs | 6.3 µs |
| 1788 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 259 µs | 104 µs| 0% | 30% | 0:00:12.500800 | 56 µs | 4.5 µs |
| 1844 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.1 µs | 28 µs | 52 µs| 2% | 39% | 0:01:00.006417 | 97 µs | 1.6 µs |
| 1843 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.6 µs | 27 µs | 119 µs| 0% | 10% | 0:04:07.219778 | 259 µs | 1.0 µs |
| 1845 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 52 µs | 417 µs | 59 µs| 0% | 85% | 0:00:10 | 299 µs | 30 µs |
| 1846 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.3 µs | 353 µs | 106 µs| 0% | 70% | 0:00:10 | 292 µs | 29 µs |
| 1894 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 12 µs | 62 µs| 0% | 6% | 0:06:40.989946 | 229 µs | 570 ns |
| 1897 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 120 µs | 106 µs| 0% | 20% | 0:00:45.229534 | 271 µs | 6.0 µs |
| 1917 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.2 µs | 32 µs | 126 µs| 0% | 7% | 0:07:57.296246 | 1.6 ms | 3.3 µs |
| 1920 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 353 µs | 105 µs| 0% | 42% | 0:00:10 | 513 µs | 51 µs |
| 1895 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 75 µs | 53 µs| 0% | 36% | 0:00:27.010438 | 140 µs | 5.2 µs |
| 1896 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 56 µs | 57 µs| 0% | 90% | 0:00:15.022943 | 97 µs | 6.5 µs |
| 1918 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.4 µs | 24 µs | 52 µs| 0% | 46% | 0:00:13.005030 | 28 µs | 2.2 µs |
| 1919 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 71 µs | 2.5 ms | 56 µs| 0% | 76% | 0:00:13.010481 | 506 µs | 39 µs |
| 2074 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.7 µs | 10 µs | 75 µs| 0% | 93% | 0:00:17.176247 | 11 µs | 668 ns |
| 2100 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 10 µs | 34 µs | 314 µs| 0% | 8% | 0:04:28.986247 | 129 µs | 480 ns |
| 2103 | Unprioritized Network 33% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 4.8 µs | 11 µs | 75 µs| 0% | 87% | 0:00:11.979769 | 51 µs | 4.3 µs |
| 2071 | Unprioritized Network 33% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 9.7 µs | 37 µs | 335 µs| 0% | 5% | 0:08:30.957814 | 899 µs | 1.8 µs |
| 2072 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.5 µs | 19 µs | 36 µs| 44% | 89% | 0:00:35.001026 | 648 ms | 19 ms |
| 2073 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.6 µs | 9.9 µs | 37 µs| 0% | 94% | 0:00:26.945410 | 240 ms | 8.9 ms |
| 2101 | Unprioritized Network 33% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.6 µs | 18 µs | 36 µs| 47% | 90% | 0:00:18.001302 | 71 ms | 3.9 ms |
| 2102 | Unprioritized Network 33% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.6 µs | 10 µs | 37 µs| 0% | 93% | 0:00:41.850472 | 661 ms | 16 ms |
### Benchmark: Unprioritized Network 50% Load
_Id: `load/net_unprioritized/load_50`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 50% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 50% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 500 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 61 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 48 µs | 78 µs| 0% | 7% | 0:02:14.775296 | 115 µs | 856 ns |
| 437 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 41 µs | 416 µs | 151 µs| 0% | 9% | 0:00:10 | 368 µs | 37 µs |
| 55 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 18 µs | 46 µs | 95 µs| 0.3% | 6% | 0:02:20.182246 | 228 µs | 1.6 µs |
| 57 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.6 µs | 52 µs | 204 µs| 0% | 10% | 0:01:32.977070 | 222 µs | 2.4 µs |
| 59 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 18 µs | 39 µs | 62 µs| 0% | 7% | 0:02:14.769290 | 111 µs | 827 ns |
| 56 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 26 µs | 150 µs | 72 µs| 0% | 54% | 0:00:54.710137 | 265 µs | 4.8 µs |
| 62 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 46 µs | 75 µs| 6% | 53% | 0:00:22.004048 | 30 µs | 1.4 µs |
| 54 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 32 µs | 62 µs| 0% | 84% | 0:01:10.003796 | 97 µs | 1.4 µs |
| 60 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 103 µs | 98 µs| 0% | 26% | 0:00:25.999616 | 127 µs | 4.9 µs |
| 205 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 335 µs | 138 µs| 0% | 12% | 0:00:10 | 394 µs | 39 µs |
| 213 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 339 µs | 136 µs| 0% | 13% | 0:00:16.752886 | 435 µs | 26 µs |
| 204 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 53 µs | 144 µs | 112 µs| 0% | 98% | 0:00:11.834530 | 138 µs | 12 µs |
| 196 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 58 µs | 83 µs| 0% | 100% | 0:00:10 | 64 µs | 6.4 µs |
| 281 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.2 µs | 66 µs | 34 µs| - | - | 0:00:01 | 837 ms | 837 ms |
| 444 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 31 µs | 386 µs | 135 µs| 0% | 17% | 0:00:10 | 299 µs | 30 µs |
| 315 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 4.2 µs | 10 µs | 75 µs| - | - | 0:00:01 | 115 µs | 115 µs |
| 435 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 107 µs | 495 µs | 105 µs| 0% | 92% | 0:00:14.128357 | 416 µs | 29 µs |
| 436 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 44 µs | 74 µs| 0% | 96% | 0:00:10 | 38 µs | 3.8 µs |
| 271 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 9.1 µs | 27 µs | 411 µs| - | - | 0:07:59.000217 | 1.3 ms | 2.7 µs |
| 282 | Unprioritized Network 50% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 176 µs | 890 µs | 766 µs| - | - | 0:00:01 | 19 µs | 19 µs |
| 283 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.7 µs | 10 µs | 75 µs| - | - | 0:00:01 | 45 µs | 45 µs |
| 297 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.8 µs | 91 µs | 34 µs| - | - | 0:00:01 | 1.8 µs | 1.8 µs |
| 314 | Unprioritized Network 50% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 165 µs | 655 µs | 514 µs| - | - | 0:00:01 | 306 µs | 306 µs |
| 492 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.8 µs | 13 µs | 62 µs| 0% | 7% | 0:00:57.920454 | 57 µs | 976 ns |
| 438 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 421 µs | 147 µs| 0% | 14% | 0:00:10 | 476 µs | 48 µs |
| 514 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 21 µs | 104 µs | 138 µs| 0% | 82% | 0:00:10 | 96 µs | 9.6 µs |
| 495 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.9 µs | 15 µs | 64 µs| 0% | 6% | 0:00:50.964269 | 56 µs | 1.1 µs |
| 498 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 58 µs | 66 µs| 0% | 31% | 0:00:11.001439 | 119 µs | 11 µs |
| 502 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 41 µs | 73 µs| 0% | 99% | 0:00:13.445955 | 51 µs | 3.8 µs |
| 494 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 24 µs | 169 µs| 0% | 7% | 0:00:44.976927 | 135 µs | 3.0 µs |
| 497 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 41 µs | 135 µs | 110 µs| 0% | 13% | 0:00:41.001705 | 120 µs | 2.9 µs |
| 500 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 34 µs | 120 µs | 94 µs| 0% | 31% | 0:00:12.996191 | 74 µs | 5.7 µs |
| 501 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 46 µs | 74 µs| 0% | 97% | 0:00:10 | 105 µs | 10 µs |
| 504 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 43 µs | 74 µs| 0% | 99% | 0:00:13.168000 | 35 µs | 2.7 µs |
| 511 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 21 µs | 57 µs | 84 µs| 0% | 100% | 0:00:16.331908 | 67 µs | 4.1 µs |
| 515 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 31 µs | 127 µs | 141 µs| 0% | 46% | 0:00:10 | 111 µs | 11 µs |
| 512 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 427 µs | 152 µs| 0% | 14% | 0:00:23.543936 | 471 µs | 20 µs |
| 1015 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 36 µs | 76 µs| 5% | 45% | 0:00:20.003236 | 14 µs | 700 ns |
| 1016 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 35 µs | 122 µs | 94 µs| 0% | 32% | 0:02:21.010802 | 275 µs | 1.9 µs |
| 1108 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 63 µs | 67 µs| 0% | 43% | 0:00:10.002503 | 17 µs | 1.7 µs |
| 1125 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 30 µs | 101 µs | 88 µs| 0% | 36% | 0:02:21.007988 | 283 µs | 2.0 µs |
| 1258 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.1 µs | 32 µs | 171 µs| 0% | 7% | 0:03:39.089128 | 241 µs | 1.1 µs |
| 1259 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 38 µs | 124 µs | 91 µs| 0% | 33% | 0:02:28.943086 | 273 µs | 1.8 µs |
| 1261 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 332 µs | 130 µs| 0% | 7% | 0:00:16.179710 | 271 µs | 17 µs |
| 1277 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 23 µs | 110 µs | 138 µs| 0% | 71% | 0:00:10 | 143 µs | 14 µs |
| 58 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 22 µs | 115 µs | 53 µs| 0% | 51% | 0:00:10 | 15 µs | 1.5 µs |
| 53 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 21 µs | 52 µs | 123 µs| 0% | 10% | 0:02:46.974565 | 228 µs | 1.4 µs |
| 212 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 126 µs | 462 µs | 115 µs| 0% | 98% | 0:00:11.002934 | 286 µs | 26 µs |
| 503 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 51 µs | 75 µs| 0% | 98% | 0:00:13.434876 | 87 µs | 6.5 µs |
| 493 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 14 µs | 62 µs| 0% | 10% | 0:00:30.976871 | 50 µs | 1.6 µs |
| 491 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 18 µs | 163 µs| 0% | 4% | 0:00:52.919034 | 106 µs | 2.0 µs |
| 197 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 34 µs | 255 µs | 139 µs| 0% | 15% | 0:00:46.129488 | 295 µs | 6.4 µs |
| 513 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 219 µs | 139 µs| 0% | 17% | 0:00:16.665008 | 130 µs | 7.8 µs |
| 1260 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 43 µs | 75 µs| 0% | 98% | 0:00:19.011846 | 34 µs | 1.8 µs |
| 1775 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 34 µs | 109 µs | 103 µs| 0% | 37% | 0:00:29.002602 | 124 µs | 4.3 µs |
| 1776 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 21 µs | 57 µs | 65 µs| 0% | 98% | 0:00:10 | 66 µs | 6.6 µs |
| 1774 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.5 µs | 24 µs | 106 µs| 0% | 9% | 0:04:27.500828 | 239 µs | 893 ns |
| 1791 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 49 µs | 74 µs| 0% | 97% | 0:00:13.774070 | 72 µs | 5.2 µs |
| 1790 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.0 µs | 27 µs | 67 µs| 0% | 44% | 0:00:29.001039 | 48 µs | 1.7 µs |
| 1789 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.5 µs | 25 µs | 64 µs| 0% | 5% | 0:04:22.975895 | 234 µs | 890 ns |
| 1847 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 41 µs | 68 µs| 0% | 5% | 0:04:01.269046 | 265 µs | 1.1 µs |
| 1822 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 47 µs | 449 µs | 191 µs| 0% | 39% | 0:00:10.099982 | 309 µs | 31 µs |
| 1848 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 53 µs | 68 µs| 0% | 100% | 0:00:20.972480 | 58 µs | 2.8 µs |
| 1849 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 42 µs | 434 µs | 171 µs| 0% | 31% | 0:00:10 | 419 µs | 42 µs |
| 1900 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 36 µs | 386 µs | 138 µs| 0% | 14% | 0:00:11.077016 | 529 µs | 48 µs |
| 1898 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.8 µs | 17 µs | 161 µs| 0% | 4% | 0:06:04.969573 | 346 µs | 949 ns |
| 1899 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.8 µs | 41 µs | 75 µs| 0% | 99% | 0:00:12.720831 | 56 µs | 4.4 µs |
| 2006 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 414 µs | 140 µs| 0% | 28% | 0:00:14.139980 | 454 µs | 32 µs |
| 2007 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 122 µs | 463 µs | 102 µs| 0.4% | 97% | 0:00:10 | 431 µs | 43 µs |
| 2008 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 31 µs | 175 µs | 135 µs| 0% | 18% | 0:00:10 | 222 µs | 22 µs |
| 2009 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 116 µs | 461 µs | 93 µs| 0% | 97% | 0:00:17.305089 | 615 µs | 36 µs |
| 2010 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 23 µs | 110 µs | 138 µs| 0% | 75% | 0:00:10.491815 | 93 µs | 8.8 µs |
| 2011 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 132 µs | 498 µs | 107 µs| 0% | 95% | 0:00:10 | 381 µs | 38 µs |
| 2077 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.7 µs | 11 µs | 42 µs| 0% | 99% | 0:00:27.216671 | 214 ms | 7.9 ms |
| 2075 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 11 µs | 29 µs | 388 µs| 0% | 8% | 0:06:52.010800 | 925 µs | 2.2 µs |
| 2076 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.4 µs | 45 µs | 34 µs| 51% | 80% | 0:01:25.007678 | 430 ms | 5.1 ms |
| 2078 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 4.1 µs | 9.8 µs | 75 µs| 0% | 95% | 0:00:20.221232 | 9.5 µs | 468 ns |
| 2104 | Unprioritized Network 50% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 11 µs | 30 µs | 360 µs| 0% | 8% | 0:07:07.737149 | 943 µs | 2.2 µs |
| 2105 | Unprioritized Network 50% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.7 µs | 67 µs | 34 µs| 53% | 89% | 0:00:15.001941 | 422 ms | 28 ms |
| 2106 | Unprioritized Network 50% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.5 µs | 9.8 µs | 42 µs| 0% | 100% | 0:00:21.005130 | 258 ms | 12 ms |
| 2107 | Unprioritized Network 50% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.6 µs | 8.5 µs | 86 µs| 0% | 91% | 0:00:10 | 40 µs | 4.0 µs |
### Benchmark: Unprioritized Network 66% Load
_Id: `load/net_unprioritized/load_66`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 66% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 66% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 660 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1851 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 53 µs | 150 µs | 202 µs| 0% | 23% | 0:01:11.001948 | 205 µs | 2.9 µs |
| 1112 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 34 µs | 189 µs | 138 µs| 0% | 66% | 0:00:12.725165 | 136 µs | 11 µs |
| 1126 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 22 µs | 65 µs | 103 µs| 0% | 10% | 0:01:51.814473 | 119 µs | 1.1 µs |
| 1109 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.2 µs | 27 µs | 68 µs| 0% | 12% | 0:03:40.962721 | 138 µs | 623 ns |
| 1159 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 47 µs | 162 µs | 187 µs| 0% | 26% | 0:00:57.004273 | 176 µs | 3.1 µs |
| 1160 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 41 µs | 68 µs| 0% | 100% | 0:00:11.366701 | 32 µs | 2.8 µs |
| 1161 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 36 µs | 320 µs | 138 µs| 0% | 29% | 0:00:14.157432 | 492 µs | 35 µs |
| 1176 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 112 µs | 354 µs | 112 µs| 0% | 99% | 0:00:19.728396 | 495 µs | 25 µs |
| 1192 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 75 µs | 219 µs | 178 µs| 0% | 99% | 0:00:10.802060 | 179 µs | 17 µs |
| 1207 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.2 µs | 22 µs | 79 µs| 0% | 9% | 0:04:18.966300 | 232 µs | 895 ns |
| 1209 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 42 µs | 72 µs| 0% | 99% | 0:00:10 | 46 µs | 4.6 µs |
| 1111 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 46 µs | 72 µs| 0% | 100% | 0:00:12.924418 | 47 µs | 3.7 µs |
| 1129 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 338 µs | 138 µs| 0% | 36% | 0:00:17.196595 | 430 µs | 25 µs |
| 1110 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 56 µs | 163 µs | 192 µs| 0% | 22% | 0:00:59.005988 | 205 µs | 3.5 µs |
| 1224 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 54 µs | 159 µs | 189 µs| 0% | 21% | 0:00:33.001975 | 207 µs | 6.3 µs |
| 1225 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 100 µs | 72 µs| 0% | 97% | 0:00:10 | 107 µs | 11 µs |
| 1208 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 30 µs | 132 µs | 194 µs| 5% | 34% | 0:00:38.000795 | 187 µs | 4.9 µs |
| 1190 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.6 µs | 19 µs | 67 µs| 0% | 14% | 0:03:29.965531 | 116 µs | 553 ns |
| 1191 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 45 µs | 152 µs | 177 µs| 0% | 28% | 0:00:10 | 47 µs | 4.7 µs |
| 1174 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.2 µs | 23 µs | 67 µs| 0% | 10% | 0:03:45.149710 | 117 µs | 518 ns |
| 1143 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 71 µs | 67 µs| 0% | 53% | 0:00:13.001898 | 136 µs | 10 µs |
| 1142 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.0 µs | 32 µs | 67 µs| 0% | 9% | 0:03:42.975358 | 204 µs | 916 ns |
| 1210 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 95 µs | 470 µs | 269 µs| 0% | 26% | 0:00:11.114050 | 401 µs | 36 µs |
| 1158 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 45 µs | 76 µs| 0% | 17% | 0:03:03.936991 | 151 µs | 820 ns |
| 1145 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 75 µs | 549 µs | 218 µs| 0% | 6% | 0:00:17.207743 | 578 µs | 34 µs |
| 1128 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 48 µs | 72 µs| 0% | 100% | 0:00:15.492859 | 54 µs | 3.5 µs |
| 1127 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 54 µs | 169 µs | 218 µs| 0% | 31% | 0:00:49.005840 | 256 µs | 5.2 µs |
| 1193 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 35 µs | 207 µs | 138 µs| 0% | 70% | 0:00:10 | 100 µs | 10.0 µs |
| 1175 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.2 µs | 29 µs | 68 µs| 0% | 76% | 0:00:14.000411 | 68 µs | 4.9 µs |
| 1144 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 171 µs | 582 µs | 159 µs| 0% | 100% | 0:00:10 | 196 µs | 20 µs |
| 1238 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 29 µs | 240 µs| 0% | 7% | 0:04:20.926312 | 412 µs | 1.6 µs |
| 1239 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.5 µs | 23 µs | 68 µs| 0% | 82% | 0:00:51.003108 | 98 µs | 1.9 µs |
| 1262 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 42 µs | 78 µs| 0% | 18% | 0:03:23.856851 | 238 µs | 1.2 µs |
| 1263 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.7 µs | 25 µs | 67 µs| 0% | 81% | 0:00:11.002194 | 73 µs | 6.6 µs |
| 1265 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 35 µs | 197 µs | 138 µs| 0% | 62% | 0:00:11.546725 | 160 µs | 14 µs |
| 1240 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 123 µs | 378 µs | 114 µs| 0% | 100% | 0:00:16.003497 | 374 µs | 23 µs |
| 1177 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 42 µs | 461 µs | 143 µs| 0% | 12% | 0:00:15.031222 | 653 µs | 43 µs |
| 1241 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 180 µs | 139 µs| 0% | 73% | 0:00:13.980507 | 61 µs | 4.4 µs |
| 1226 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 187 µs | 139 µs| 0% | 77% | 0:00:10.019954 | 107 µs | 11 µs |
| 1264 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 160 µs | 584 µs | 166 µs| 0% | 99% | 0:00:12.208311 | 725 µs | 59 µs |
| 1223 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 33 µs | 78 µs| 0% | 9% | 0:04:13.950262 | 335 µs | 1.3 µs |
| 1778 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 24 µs | 67 µs| 0% | 86% | 0:00:18.001223 | 22 µs | 1.2 µs |
| 1777 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.9 µs | 24 µs | 82 µs| 0% | 9% | 0:04:53.914105 | 233 µs | 792 ns |
| 1780 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 196 µs | 138 µs| 0% | 72% | 0:00:12.723317 | 130 µs | 10 µs |
| 1779 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 156 µs | 576 µs | 145 µs| 0% | 99% | 0:00:10 | 623 µs | 62 µs |
| 1823 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.2 µs | 21 µs | 253 µs| 0% | 11% | 0:05:04.871137 | 312 µs | 1.0 µs |
| 1826 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 43 µs | 433 µs | 140 µs| 0% | 15% | 0:00:11.130609 | 441 µs | 40 µs |
| 1850 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.4 µs | 27 µs | 237 µs| 0% | 5% | 0:04:20.983526 | 351 µs | 1.3 µs |
| 1824 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 51 µs | 158 µs | 199 µs| 0% | 28% | 0:01:22.004687 | 229 µs | 2.8 µs |
| 1825 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 44 µs | 72 µs| 0% | 100% | 0:00:13.483925 | 58 µs | 4.3 µs |
| 1852 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 82 µs | 72 µs| 0% | 97% | 0:00:12.729663 | 144 µs | 11 µs |
| 1853 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 337 µs | 139 µs| 0% | 34% | 0:00:11.804831 | 403 µs | 34 µs |
| 1903 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 168 µs | 544 µs | 158 µs| 0% | 99% | 0:00:10 | 827 µs | 83 µs |
| 1923 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 23 µs | 113 µs | 82 µs| 0.3% | 95% | 0:00:14.525389 | 128 µs | 8.8 µs |
| 1901 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 32 µs | 96 µs | 112 µs| 0% | 13% | 0:02:09.975253 | 265 µs | 2.0 µs |
| 1902 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 71 µs | 67 µs| 0% | 72% | 0:00:16.989920 | 47 µs | 2.8 µs |
| 1904 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 34 µs | 93 µs | 134 µs| 0% | 24% | 0:00:12.129625 | 59 µs | 4.8 µs |
| 1921 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.1 µs | 23 µs | 67 µs| 0% | 17% | 0:08:46.126462 | 1.6 ms | 3.0 µs |
| 1922 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 79 µs | 67 µs| 0% | 52% | 0:00:25.006358 | 192 µs | 7.7 µs |
| 1924 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 93 µs | 612 µs | 253 µs| 0% | 4% | 0:00:12.065393 | 779 µs | 65 µs |
| 2080 | Unprioritized Network 66% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.5 µs | 67 µs | 34 µs| 56% | 86% | 0:01:05.004432 | 85 ms | 1.3 ms |
| 2079 | Unprioritized Network 66% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 9.7 µs | 29 µs | 417 µs| 0% | 6% | 0:03:11.992819 | 312 µs | 1.6 µs |
| 2081 | Unprioritized Network 66% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 310 ns | 11 µs | 42 µs| 0% | 96% | 0:00:24.744523 | 36 ms | 1.5 ms |
| 2082 | Unprioritized Network 66% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 4.6 µs | 11 µs | 69 µs| 0% | 95% | 0:00:11.063838 | 60 µs | 5.4 µs |
### Benchmark: Unprioritized Network 80% Load
_Id: `load/net_unprioritized/load_80`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 80% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 80% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 800 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 77 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.0 µs | 30 µs | 55 µs| 0% | 13% | 0:02:48.964008 | 123 µs | 725 ns |
| 80 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 51 µs | 66 µs| 0% | 81% | 0:00:23.946263 | 56 µs | 2.3 µs |
| 82 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 97 µs | 70 µs| 0% | 59% | 0:00:19.864318 | 151 µs | 7.6 µs |
| 78 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 49 µs | 180 µs | 240 µs| 0% | 24% | 0:00:31.366126 | 294 µs | 9.4 µs |
| 76 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 38 µs | 113 µs | 205 µs| 0% | 38% | 0:00:25.812585 | 95 µs | 3.7 µs |
| 75 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 59 µs | 87 µs| 0% | 12% | 0:02:10.990623 | 131 µs | 997 ns |
| 81 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 62 µs | 155 µs| 0% | 8% | 0:00:38.816535 | 392 µs | 10 µs |
| 73 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 48 µs | 68 µs| 0.3% | 12% | 0:02:13.664123 | 116 µs | 867 ns |
| 198 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 220 µs | 767 µs | 257 µs| 0% | 100% | 0:00:13.886013 | 569 µs | 41 µs |
| 207 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 156 µs | 700 µs | 392 µs| 0% | 7% | 0:00:10 | 668 µs | 67 µs |
| 199 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 29 µs | 445 µs | 142 µs| 0% | 38% | 0:00:24.683396 | 440 µs | 18 µs |
| 284 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 12 µs | 38 µs | 357 µs| - | - | 0:04:20.582866 | 511 µs | 2.0 µs |
| 430 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 186 µs | 141 µs| 0% | 96% | 0:00:16.211659 | 211 µs | 13 µs |
| 426 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 19 µs | 55 µs | 83 µs| 0% | 100% | 0:00:10 | 58 µs | 5.8 µs |
| 300 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 6.7 µs | 18 µs | 362 µs| - | - | 0:04:49.020110 | 424 µs | 1.5 µs |
| 449 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 194 µs | 624 µs | 208 µs| 0% | 100% | 0:00:10 | 971 µs | 97 µs |
| 318 | Unprioritized Network 80% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 135 µs | 428 µs | 370 µs| - | - | 0:00:01 | 357 µs | 357 µs |
| 427 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.1 µs | 41 µs | 73 µs| 0% | 99% | 0:00:14.727947 | 64 µs | 4.3 µs |
| 301 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.9 µs | 186 µs | 30 µs| - | - | 0:00:01 | 327 ms | 327 ms |
| 303 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 14 µs | 15 µs | 69 µs| - | - | 0:00:01 | 18 µs | 18 µs |
| 316 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.0 µs | 16 µs | 381 µs| - | - | 0:04:51.000438 | 342 µs | 1.2 µs |
| 317 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 3.6 µs | 155 µs | 30 µs| - | - | 0:00:01 | 151 ms | 151 ms |
| 319 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 14 µs | 15 µs | 69 µs| - | - | 0:00:01 | 8.1 µs | 8.1 µs |
| 533 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.6 µs | 80 µs | 68 µs| 0% | 45% | 0:00:11.000758 | 3.7 µs | 335 ns |
| 526 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.7 µs | 33 µs | 338 µs| 0% | 6% | 0:01:39.892517 | 342 µs | 3.4 µs |
| 540 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 59 µs | 639 µs | 208 µs| 0% | 15% | 0:00:10.661765 | 752 µs | 70 µs |
| 538 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 38 µs | 539 µs | 159 µs| 0% | 21% | 0:00:10 | 1.7 ms | 175 µs |
| 535 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 205 µs | 620 µs | 219 µs| 0% | 100% | 0:00:15.936135 | 437 µs | 27 µs |
| 529 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.9 µs | 23 µs | 341 µs| 0% | 11% | 0:00:36.970571 | 58 µs | 1.6 µs |
| 516 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.8 µs | 25 µs | 74 µs| 0% | 10% | 0:00:51.902203 | 73 µs | 1.4 µs |
| 539 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 165 µs | 719 µs | 412 µs| 0% | 6% | 0:00:47.245671 | 2.7 ms | 57 µs |
| 537 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 206 µs | 648 µs | 228 µs| 0% | 100% | 0:00:10 | 468 µs | 47 µs |
| 536 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 56 µs | 84 µs| 0% | 100% | 0:00:12.560870 | 122 µs | 9.7 µs |
| 534 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 28 µs | 68 µs| 0% | 80% | 0:00:28.999787 | 54 µs | 1.9 µs |
| 532 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 61 µs | 171 µs | 315 µs| 0% | 25% | 0:00:30.003130 | 199 µs | 6.6 µs |
| 531 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 58 µs | 168 µs | 297 µs| 0% | 39% | 0:01:17.005139 | 222 µs | 2.9 µs |
| 528 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 33 µs | 250 µs| 0% | 6% | 0:00:42.561399 | 92 µs | 2.2 µs |
| 527 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.4 µs | 27 µs | 327 µs| 0% | 5% | 0:00:50.975637 | 360 µs | 7.1 µs |
| 542 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 66 µs | 683 µs | 218 µs| 0% | 16% | 0:00:10 | 1.0 ms | 104 µs |
| 541 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 41 µs | 662 µs | 159 µs| 0% | 19% | 0:00:14.683701 | 435 µs | 30 µs |
| 1608 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 31 µs | 420 µs | 142 µs| 0% | 31% | 0:00:10.562092 | 377 µs | 36 µs |
| 1266 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 69 µs | 108 µs| 0% | 13% | 0:02:56.768917 | 284 µs | 1.6 µs |
| 1268 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 38 µs | 73 µs| 0% | 100% | 0:00:12.712830 | 39 µs | 3.1 µs |
| 1269 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 459 µs | 141 µs| 0% | 18% | 0:00:16.904183 | 654 µs | 39 µs |
| 1350 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 36 µs | 88 µs | 89 µs| 0% | 8% | 0:02:15.990913 | 270 µs | 2.0 µs |
| 79 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.9 µs | 33 µs | 343 µs| 0% | 8% | 0:02:54.441307 | 126 µs | 723 ns |
| 74 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 86 µs | 70 µs| 0% | 70% | 0:00:22.002207 | 63 µs | 2.9 µs |
| 206 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.6 µs | 53 µs | 73 µs| 0% | 100% | 0:00:12.008388 | 94 µs | 7.8 µs |
| 214 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.7 µs | 41 µs | 73 µs| 0% | 99% | 0:00:10 | 54 µs | 5.4 µs |
| 450 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.6 µs | 41 µs | 73 µs| 0% | 99% | 0:00:10 | 111 µs | 11 µs |
| 429 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 27 µs | 202 µs | 140 µs| 0% | 78% | 0:00:10 | 146 µs | 15 µs |
| 428 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 18 µs | 184 µs | 140 µs| 0% | 87% | 0:00:17.905813 | 150 µs | 8.4 µs |
| 530 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 29 µs | 68 µs| 0% | 83% | 0:00:10.000461 | 15 µs | 1.5 µs |
| 1267 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.4 µs | 31 µs | 68 µs| 0% | 82% | 0:00:57.004206 | 71 µs | 1.2 µs |
| 1606 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 60 µs | 90 µs| 62% | 49% | 0:00:35.919951 | 38 µs | 1.1 µs |
| 1607 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 84 µs | 73 µs| 0% | 98% | 0:00:12.627531 | 35 µs | 2.7 µs |
| 1829 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 19 µs | 57 µs | 84 µs| 0.3% | 100% | 0:00:10.508995 | 86 µs | 8.1 µs |
| 1854 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.9 µs | 33 µs | 339 µs| 0% | 9% | 0:04:27.931821 | 366 µs | 1.4 µs |
| 1857 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 168 µs | 716 µs | 416 µs| 0% | 4% | 0:00:28.309116 | 731 µs | 26 µs |
| 1827 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.5 µs | 27 µs | 335 µs| 0% | 5% | 0:04:57.812941 | 407 µs | 1.4 µs |
| 1828 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 96 µs | 240 µs| 14% | 32% | 0:00:41.001177 | 165 µs | 4.0 µs |
| 1830 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 24 µs | 186 µs | 141 µs| 0% | 89% | 0:00:11.532602 | 155 µs | 13 µs |
| 1855 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 58 µs | 165 µs | 304 µs| 0% | 29% | 0:00:19.000436 | 225 µs | 12 µs |
| 1856 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.8 µs | 40 µs | 73 µs| 0.3% | 100% | 0:00:14.445639 | 41 µs | 2.8 µs |
| 1866 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 85 µs | 88 µs| 68% | 43% | 0:01:07.003653 | 59 µs | 876 ns |
| 1906 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.0 µs | 39 µs | 73 µs| 0% | 100% | 0:00:14.936399 | 69 µs | 4.6 µs |
| 1905 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.8 µs | 25 µs | 336 µs| 0% | 3% | 0:05:14.982802 | 344 µs | 1.1 µs |
| 1907 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 44 µs | 443 µs | 160 µs| 0% | 18% | 0:00:12.138426 | 439 µs | 36 µs |
| 2083 | Unprioritized Network 80% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 6.4 µs | 18 µs | 376 µs| 0% | 5% | 0:07:13.005293 | 937 µs | 2.2 µs |
| 2086 | Unprioritized Network 80% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 14 µs | 15 µs | 69 µs| 0% | 14% | 0:00:11.111299 | 486 µs | 44 µs |
| 2084 | Unprioritized Network 80% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.7 µs | 143 µs | 29 µs| 65% | 90% | 0:00:42.002539 | 122 ms | 2.9 ms |
| 2085 | Unprioritized Network 80% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 6.1 µs | 11 µs | 25 µs| 0% | 99% | 0:00:31.743360 | 516 ms | 16 ms |
### Benchmark: Unprioritized Network 90% Load
_Id: `load/net_unprioritized/load_90`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 90% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 90% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 900 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1114 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 712 µs | 2.3 ms | 3.4 ms| 0% | 27% | 0:01:37.004205 | 3.3 ms | 34 µs |
| 1162 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 19 µs | 1.8 ms| 0% | 7% | 0:10:20.923495 | 201 µs | 323 ns |
| 1148 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 15 µs | 62 µs| 0% | 99% | 0:00:10.118597 | 12 µs | 1.2 µs |
| 1196 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.5 µs | 18 µs | 62 µs| 0% | 98% | 0:00:10 | 8.1 µs | 813 ns |
| 1194 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.2 µs | 20 µs | 64 µs| 0% | 9% | 0:03:03.581079 | 105 µs | 573 ns |
| 1197 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 ms | 12 ms | 3.4 ms| 0% | 3% | 0:00:14.244975 | 11 ms | 772 µs |
| 1227 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 112 µs | 298 µs | 4.5 ms| 0% | 0.2% | 0:01:05.917426 | 2.5 ms | 38 µs |
| 1229 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.6 µs | 38 µs | 62 µs| 0% | 100% | 0:00:10 | 37 µs | 3.7 µs |
| 1147 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 689 µs | 2.3 ms | 2.5 ms| 0% | 16% | 0:00:29.003802 | 2.8 ms | 97 µs |
| 1178 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.2 µs | 18 µs | 64 µs| 0% | 8% | 0:03:57.914587 | 104 µs | 438 ns |
| 1179 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.9 µs | 51 µs | 59 µs| 0% | 77% | 0:00:23.998024 | 20 µs | 829 ns |
| 1130 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.9 µs | 36 µs | 66 µs| 0% | 7% | 0:03:34.979996 | 136 µs | 631 ns |
| 1131 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.9 µs | 58 µs | 59 µs| 0% | 69% | 0:00:18.000883 | 52 µs | 2.9 µs |
| 1244 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 ms | 11 ms | 2.4 ms| 0% | 100% | 0:00:17.504667 | 9.1 ms | 518 µs |
| 1163 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.7 µs | 41 µs | 59 µs| 0% | 74% | 0:00:10.003585 | 4.8 µs | 484 ns |
| 1180 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 25 µs | 140 µs | 184 µs| 0% | 99% | 0:00:16.995564 | 237 µs | 14 µs |
| 1242 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 135 µs | 368 µs | 4.8 ms| 0% | 0.6% | 0:03:02.891206 | 2.7 ms | 15 µs |
| 1243 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 498 µs | 1.7 ms | 2.1 ms| 0% | 20% | 0:01:26.003339 | 2.6 ms | 30 µs |
| 1245 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 123 µs | 120 µs| 0% | 93% | 0:00:10 | 120 µs | 12 µs |
| 1133 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 126 µs | 119 µs| 0% | 92% | 0:00:10.674528 | 133 µs | 12 µs |
| 1132 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 25 µs | 69 µs| 0% | 98% | 0:00:11.824997 | 25 µs | 2.1 µs |
| 1115 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 ms | 11 ms | 2.7 ms| 0% | 99% | 0:00:10.003798 | 4.6 ms | 457 µs |
| 1113 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 95 µs | 277 µs | 3.9 ms| 0% | 0.7% | 0:03:05.638444 | 3.4 ms | 18 µs |
| 1146 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.0 µs | 47 µs | 74 µs| 0% | 7% | 0:03:53.927196 | 137 µs | 586 ns |
| 1228 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 696 µs | 2.5 ms | 2.7 ms| 0% | 19% | 0:04:22.020690 | 11 ms | 43 µs |
| 1116 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 675 µs | 10 ms | 1.4 ms| 0% | 4% | 0:02:00.231873 | 24 ms | 202 µs |
| 1230 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 122 µs | 119 µs| 0% | 89% | 0:00:13.184167 | 110 µs | 8.3 µs |
| 1213 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.9 µs | 35 µs | 62 µs| 0% | 100% | 0:00:13.715542 | 50 µs | 3.7 µs |
| 1195 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 11 µs | 59 µs| 0% | 88% | 0:00:39.001863 | 80 µs | 2.0 µs |
| 1273 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 423 µs | 8.5 ms | 902 µs| 0% | 11% | 0:00:14.161792 | 20 ms | 1.4 ms |
| 1270 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.7 µs | 28 µs | 1.4 ms| 0% | 6% | 0:05:28.297943 | 242 µs | 738 ns |
| 1271 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.6 µs | 45 µs | 59 µs| 0% | 73% | 0:00:21.001476 | 47 µs | 2.2 µs |
| 1272 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 ms | 9.1 ms | 2.4 ms| 0% | 99% | 0:00:10 | 14 ms | 1.4 ms |
| 1331 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 ms | 9.8 ms | 2.2 ms| 0% | 99% | 0:00:10.743010 | 5.6 ms | 523 µs |
| 1330 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 417 µs | 1.4 ms | 1.7 ms| 0% | 18% | 0:00:30.988181 | 1.5 ms | 49 µs |
| 1332 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 9.8 ms | 143 µs| 0% | 56% | 0:00:11.166419 | 9.3 ms | 834 µs |
| 1214 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 ms | 16 ms | 3.5 ms| 0% | 3% | 0:00:27.725797 | 27 ms | 984 µs |
| 1181 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 561 µs | 6.6 ms | 1.2 ms| 0% | 7% | 0:00:17.542440 | 30 ms | 1.7 ms |
| 1164 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 ms | 9.3 ms | 2.3 ms| 0% | 99% | 0:00:15.731275 | 13 ms | 799 µs |
| 1149 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 9.6 ms | 141 µs| 0% | 17% | 0:00:17.054384 | 15 ms | 857 µs |
| 1165 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 127 µs | 120 µs| 0% | 91% | 0:00:18.212162 | 93 µs | 5.1 µs |
| 1211 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 81 µs | 225 µs | 2.9 ms| 0% | 0.8% | 0:02:04.938846 | 2.1 ms | 17 µs |
| 1212 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 977 µs | 3.3 ms | 3.7 ms| 0% | 14% | 0:01:35.002611 | 5.3 ms | 56 µs |
| 1769 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 87 µs | 354 µs | 3.8 ms| 0% | 0.2% | 0:02:07.956871 | 2.3 ms | 18 µs |
| 1770 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 657 µs | 2.3 ms | 2.6 ms| 0% | 19% | 0:00:36.004360 | 2.5 ms | 70 µs |
| 1771 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.4 µs | 17 µs | 62 µs| 0% | 99% | 0:00:17.793864 | 12 µs | 674 ns |
| 1772 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 8.4 ms | 142 µs| 0% | 13% | 0:00:10.863273 | 8.5 ms | 784 µs |
| 1773 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 8.2 ms | 144 µs| 0% | 32% | 0:00:14.275146 | 22 ms | 1.5 ms |
| 1867 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.0 µs | 39 µs | 59 µs| 0% | 76% | 0:00:10 | 52 µs | 5.2 µs |
| 1859 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 833 µs | 2.3 ms | 3.1 ms| 0% | 19% | 0:01:48.006606 | 3.5 ms | 33 µs |
| 1858 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 37 µs | 64 µs| 0% | 6% | 0:03:34.868320 | 235 µs | 1.1 µs |
| 1882 | Unprioritized Network 90% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 861 µs | 3.1 ms | 3.4 ms| 0% | 15% | 0:02:11.001249 | 7.3 ms | 56 µs |
| 1910 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 575 µs | 11 ms | 1.3 ms| 0% | 8% | 0:00:10.438691 | 6.0 ms | 574 µs |
| 1883 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 13 µs | 62 µs| 0% | 100% | 0:00:10 | 24 µs | 2.4 µs |
| 1884 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 ms | 12 ms | 3.6 ms| 0% | 0.3% | 0:00:24.409209 | 23 ms | 923 µs |
| 1908 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.2 µs | 21 µs | 64 µs| 0% | 12% | 0:04:36.978060 | 239 µs | 864 ns |
| 1909 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.8 µs | 23 µs | 69 µs| 0% | 99% | 0:00:14.006263 | 23 µs | 1.7 µs |
| 1925 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.8 µs | 16 µs | 63 µs| 0% | 17% | 0:08:31.009193 | 1.6 ms | 3.1 µs |
| 1926 | Unprioritized Network 90% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 ms | 7.6 ms | 2.5 ms| 0.3% | 97% | 0:00:10 | 12 ms | 1.2 ms |
| 2087 | Unprioritized Network 90% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 6.8 µs | 26 µs | 1.4 ms| 0% | 11% | 0:07:05.003317 | 929 µs | 2.2 µs |
| 2089 | Unprioritized Network 90% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 43 ns | 154 ns | 52 µs| 0% | 93% | 0:00:27.390401 | 7.8 µs | 286 ns |
### Benchmark: Unprioritized Network 100% Load
_Id: `load/net_unprioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 100% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 1000 Mbit/s.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 43 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 18 µs | 83 µs | 1.7 ms| 1% | 5% | 0:01:44.752576 | 109 µs | 1.0 µs |
| 51 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 18 µs | 56 µs | 86 µs| 0.3% | 11% | 0:00:40.235162 | 428 µs | 11 µs |
| 423 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 729 µs | 2.5 ms | 2.7 ms| 0% | 29% | 0:00:58.022347 | 2.9 ms | 49 µs |
| 50 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 115 µs | 43 µs| 0% | 55% | 0:02:03.904081 | 114 µs | 922 ns |
| 49 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 54 µs | 64 µs| 0% | 11% | 0:01:29.310167 | 142 µs | 1.6 µs |
| 422 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 586 µs | 2.0 ms | 2.4 ms| 0% | 16% | 0:02:02.006217 | 4.3 ms | 36 µs |
| 217 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.7 µs | 6.4 ms | 121 µs| 0% | 47% | 0:00:14.022869 | 58 µs | 4.2 µs |
| 200 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 ms | 11 ms | 2.7 ms| 0% | 99% | 0:00:19.813474 | 17 ms | 847 µs |
| 216 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 30 µs | 221 µs | 184 µs| 0% | 91% | 0:00:15.009823 | 178 µs | 12 µs |
| 1979 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 ms | 9.6 ms | 2.4 ms| 0% | 98% | 0:00:10 | 5.2 ms | 516 µs |
| 201 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 477 µs | 9.0 ms | 1.1 ms| 0% | 10% | 0:00:10 | 21 ms | 2.1 ms |
| 208 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 ms | 9.0 ms | 2.4 ms| 0% | 99% | 0:00:11.702264 | 8.9 ms | 758 µs |
| 209 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 129 µs | 119 µs| 0% | 91% | 0:00:10 | 193 µs | 19 µs |
| 424 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 ms | 15 ms | 2.9 ms| 0% | 97% | 0:00:13.309823 | 11 ms | 815 µs |
| 443 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 14 µs | 62 µs| 0% | 100% | 0:00:11.636530 | 34 µs | 2.9 µs |
| 425 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 369 µs | 8.5 ms | 858 µs| 0% | 15% | 0:00:11.300675 | 2.9 ms | 254 µs |
| 448 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 631 µs | 12 ms | 1.4 ms| 0% | 8% | 0:00:20.306250 | 17 ms | 847 µs |
| 306 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 201 µs | 441 µs | 1.2 ms| - | - | 0:00:01 | 463 µs | 463 µs |
| 322 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 86 µs | 230 µs | 1.2 ms| - | - | 0:00:01 | 268 µs | 268 µs |
| 442 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 15 µs | 62 µs| 0% | 98% | 0:00:10 | 17 µs | 1.7 µs |
| 441 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 ms | 11 ms | 2.4 ms| 0% | 100% | 0:00:14.436870 | 10 ms | 694 µs |
| 445 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 ms | 11 ms | 2.8 ms| 0% | 99% | 0:00:17.681754 | 11 ms | 619 µs |
| 288 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 12 µs | 32 µs | 2.0 ms| 0% | 14% | 0:05:50.988878 | 981 µs | 2.8 µs |
| 275 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 125 µs | 337 µs | 1.3 ms| - | - | 0:00:01 | 220 µs | 220 µs |
| 276 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 35 ns | 110 ns | 52 µs| - | - | 0:00:01 | 340 µs | 340 µs |
| 307 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 35 ns | 102 ns | 52 µs| - | - | 0:00:01 | 48 µs | 48 µs |
| 323 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 36 ns | 116 ns | 52 µs| - | - | 0:00:01 | 2.9 µs | 2.9 µs |
| 446 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 16 µs | 62 µs| 0% | 98% | 0:00:14.464158 | 38 µs | 2.6 µs |
| 545 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.0 µs | 17 µs | 63 µs| 0% | 9% | 0:01:06.933264 | 72 µs | 1.1 µs |
| 543 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 103 µs | 313 µs | 4.0 ms| 0% | 0.3% | 0:01:08.734072 | 1.7 ms | 24 µs |
| 552 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.5 µs | 39 µs | 59 µs| 0% | 75% | 0:00:14.000859 | 51 µs | 3.7 µs |
| 549 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.9 µs | 11 µs | 59 µs| 0% | 93% | 0:00:13.999801 | 11 µs | 802 ns |
| 548 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 12 µs | 59 µs| 0% | 88% | 0:00:55.002759 | 32 µs | 585 ns |
| 551 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 16 µs | 59 µs| 0% | 85% | 0:00:18.020379 | 25 µs | 1.4 µs |
| 550 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 12 µs | 59 µs| 0% | 93% | 0:00:16.998512 | 8.4 µs | 497 ns |
| 547 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 125 µs | 363 µs | 4.3 ms| 0% | 0.3% | 0:02:12.977202 | 2.9 ms | 22 µs |
| 544 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 82 µs | 257 µs | 3.6 ms| 0% | 0.10% | 0:02:02.931869 | 3.4 ms | 27 µs |
| 555 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 15 µs | 9.8 ms | 143 µs| 0% | 23% | 0:00:11.929793 | 7.0 ms | 588 µs |
| 553 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.2 µs | 6.0 ms | 120 µs| 0% | 76% | 0:00:11.560701 | 4.1 ms | 356 µs |
| 554 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 121 µs | 119 µs| 0% | 94% | 0:00:17.179726 | 126 µs | 7.4 µs |
| 1034 | Unprioritized Network 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 9.9 µs | 16 µs | 36 µs| 0% | 19% | 0:00:22.291612 | 61 µs | 2.7 µs |
| 1017 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 7.5 µs | 35 µs | 1.4 ms| 0% | - | 0:03:06.946421 | 987 µs | 5.3 µs |
| 1035 | Unprioritized Network 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 32 µs | 106 µs | 60 µs| 0% | 11% | 0:00:46.926997 | 132 µs | 2.8 µs |
| 1609 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.5 µs | 36 µs | 65 µs| 0% | 4% | 0:03:42.967290 | 220 µs | 989 ns |
| 1037 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 166 µs | 647 µs | 350 µs| 0% | 97% | 0:00:16.005833 | 186 µs | 12 µs |
| 1038 | Unprioritized Network 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 7.9 µs | 15 µs | 36 µs| 0% | 39% | 0:00:17.047689 | 33 µs | 1.9 µs |
| 1975 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.6 µs | 31 µs | 69 µs| 0% | 96% | 0:00:11.377802 | 45 µs | 4.0 µs |
| 1014 | Unprioritized Network 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 5.2 µs | 263 µs | 17 µs| 70% | 91% | 0:00:10.000450 | 20 µs | 2.0 µs |
| 1976 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 125 µs | 119 µs| 0% | 96% | 0:00:16.209975 | 119 µs | 7.4 µs |
| 1077 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 87 µs | 224 µs | 1.2 ms| 0% | - | 0:00:01 | 347 µs | 347 µs |
| 1074 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 39 ns | 131 ns | 52 µs| 0% | - | 0:00:01 | 7.2 µs | 7.2 µs |
| 1089 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 94 µs | 222 µs | 1.5 ms| 0% | - | 0:00:01 | 278 µs | 278 µs |
| 1081 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 137 µs | 421 µs | 1.2 ms| 0% | - | 0:00:01 | 199 µs | 199 µs |
| 1082 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 49 ns | 279 ns | 52 µs| 0% | - | 0:00:01 | 1.2 ms | 1.2 ms |
| 1094 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 44 ns | 195 ns | 52 µs| 0% | - | 0:00:01 | 1.7 µs | 1.7 µs |
| 1075 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.9 µs | 23 µs | 1.3 ms| 0% | - | 0:03:24.674288 | 906 µs | 4.4 µs |
| 1977 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.1 µs | 18 µs | 1.7 ms| 0% | 10% | 0:09:35.921711 | 913 µs | 1.6 µs |
| 1978 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.8 µs | 49 µs | 59 µs| 0% | 75% | 0:00:25.001451 | 90 µs | 3.6 µs |
| 1980 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 337 µs | 10 ms | 782 µs| 0% | 50% | 0:00:13.169154 | 8.0 ms | 609 µs |
| 1981 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.8 µs | 25 µs | 1.4 ms| 0% | 5% | 0:06:57.304158 | 161 µs | 386 ns |
| 1982 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.7 µs | 50 µs | 59 µs| 0% | 84% | 0:01:03.005311 | 95 µs | 1.5 µs |
| 1079 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 7.5 µs | 30 µs | 1.3 ms| 0% | - | 0:02:44.970291 | 948 µs | 5.7 µs |
| 1090 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 48 ns | 183 ns | 52 µs| 0% | - | 0:00:01 | 2.4 µs | 2.4 µs |
| 1091 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 7.7 µs | 27 µs | 1.3 ms| 0% | - | 0:03:26.671597 | 964 µs | 4.7 µs |
| 1083 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 10 µs | 33 µs | 1.3 ms| 0% | - | 0:02:50.965289 | 1.1 ms | 6.6 µs |
| 1983 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 ms | 11 ms | 2.5 ms| 0% | 97% | 0:00:12.984631 | 21 ms | 1.6 ms |
| 1085 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 86 µs | 217 µs | 1.2 ms| 0% | - | 0:00:01 | 432 µs | 432 µs |
| 1095 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.1 µs | 21 µs | 1.3 ms| 0% | - | 0:03:17.076276 | 897 µs | 4.6 µs |
| 1086 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 46 ns | 177 ns | 52 µs| 0% | - | 0:00:31.371617 | 5.2 µs | 166 ns |
| 1984 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 17 µs | 7.8 ms | 143 µs| 0% | 22% | 0:00:10 | 1.8 ms | 181 µs |
| 1087 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.7 µs | 23 µs | 1.3 ms| 0% | - | 0:04:02.984969 | 1.0 ms | 4.3 µs |
| 1098 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 48 ns | 159 ns | 52 µs| 0% | - | 0:00:01 | 3.5 µs | 3.5 µs |
| 1078 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 37 ns | 113 ns | 52 µs| 0% | - | 0:00:01 | 1.2 ms | 1.2 ms |
| 1274 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 83 µs | 235 µs | 3.5 ms| 0% | 0.8% | 0:02:18.981002 | 5.1 ms | 36 µs |
| 1987 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.2 µs | 23 µs | 68 µs| 0.4% | 100% | 0:00:13.344553 | 53 µs | 4.0 µs |
| 1276 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 14 µs | 62 µs| 0% | 100% | 0:00:18.007182 | 21 µs | 1.2 µs |
| 45 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 40 µs | 68 µs| 0.4% | 4% | 0:02:02.031710 | 117 µs | 957 ns |
| 1408 | Unprioritized Network 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.4 µs | 29 µs | 238 µs| 0% | 100% | 0:00:15.165015 | 71 µs | 4.7 µs |
| 1404 | Unprioritized Network 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 3.6 µs | 11 µs | 17 µs| 0% | 100% | 0:00:17.961019 | 16 µs | 904 ns |
| 1403 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 30 ns | 91 ns | 25 µs| 0% | - | 0:00:01 | 342 ms | 342 ms |
| 1985 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 82 µs | 247 µs | 3.6 ms| 0% | 0.2% | 0:03:26.305976 | 3.4 ms | 17 µs |
| 1986 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 230 µs | 409 µs | 366 µs| 31% | 64% | 0:02:33.781314 | 70 µs | 458 ns |
| 1988 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.7 µs | 126 µs | 120 µs| 0% | 91% | 0:00:10 | 115 µs | 11 µs |
| 1989 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.5 µs | 27 µs | 1.4 ms| 0% | 7% | 0:06:08.747741 | 916 µs | 2.5 µs |
| 1990 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.1 µs | 42 µs | 59 µs| 0% | 80% | 0:00:29.015972 | 43 µs | 1.5 µs |
| 1991 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 17 µs | 62 µs| 0% | 97% | 0:00:15.373542 | 42 µs | 2.7 µs |
| 52 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 195 µs | 46 µs| 0% | 53% | 0:04:38.695545 | 293 µs | 1.1 µs |
| 47 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 19 µs | 57 µs | 80 µs| 0% | 7% | 0:00:33.345746 | 618 µs | 19 µs |
| 44 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.9 µs | 30 µs | 42 µs| 0.3% | 79% | 0:01:35.578216 | 124 µs | 1.3 µs |
| 242 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 685 µs | 11 ms | 1.5 ms| 0% | 4% | 0:00:56.264220 | 18 ms | 323 µs |
| 241 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 ms | 14 ms | 3.4 ms| 0% | 100% | 0:00:13.694124 | 19 ms | 1.4 ms |
| 447 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 516 µs | 9.9 ms | 1.1 ms| 0% | 8% | 0:00:27.384940 | 8.8 ms | 323 µs |
| 546 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 77 µs | 246 µs | 3.6 ms| 0% | 0.6% | 0:02:23.985994 | 3.9 ms | 27 µs |
| 1333 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 13 µs | 8.3 ms | 140 µs| 0% | 24% | 0:00:11.158688 | 13 ms | 1.2 ms |
| 1033 | Unprioritized Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 171 µs | 566 µs | 308 µs| 0% | 100% | 0:00:15.002319 | 376 µs | 25 µs |
| 1032 | Unprioritized Network 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 675 ns | 18 µs | 17 µs| 0% | 91% | 0:00:18.999635 | 5.8 µs | 303 ns |
| 1612 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 12 µs | 59 µs| 0% | 80% | 0:00:23.001778 | 41 µs | 1.8 µs |
| 1613 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 13 µs | 62 µs| 0% | 100% | 0:00:12.009964 | 23 µs | 1.9 µs |
| 1614 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 127 µs | 119 µs| 0% | 93% | 0:00:10 | 124 µs | 12 µs |
| 1992 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.4 µs | 5.2 ms | 120 µs| 0% | 92% | 0:00:18.190967 | 2.0 ms | 108 µs |
| 1993 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 991 µs | 3.1 ms | 3.3 ms| 0% | 19% | 0:01:13.004421 | 5.0 ms | 68 µs |
| 1832 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 611 µs | 2.1 ms | 2.4 ms| 0% | 20% | 0:00:46.003038 | 3.4 ms | 73 µs |
| 1831 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 103 µs | 316 µs | 4.3 ms| 0% | 0.4% | 0:01:51.383030 | 5.5 ms | 50 µs |
| 1833 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 15 µs | 62 µs| 0% | 98% | 0:00:12.934568 | 25 µs | 1.9 µs |
| 1834 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 714 µs | 13 ms | 1.5 ms| 0% | 10% | 0:00:24.414628 | 16 ms | 673 µs |
| 1868 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.2 µs | 47 µs | 59 µs| 0% | 82% | 0:00:10 | 66 µs | 6.6 µs |
| 1863 | Unprioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 881 µs | 2.9 ms | 3.5 ms| 0% | 19% | 0:01:53.006497 | 5.7 ms | 51 µs |
| 1885 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.8 µs | 24 µs | 1.3 ms| 0% | 6% | 0:03:59.925193 | 267 µs | 1.1 µs |
| 1911 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.0 µs | 38 µs | 66 µs| 0% | 5% | 0:03:38.503401 | 236 µs | 1.1 µs |
| 1997 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 26 ns | 81 ns | 25 µs| 0% | 98% | 0:00:31.908089 | 215 ms | 6.7 ms |
| 1886 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 ms | 13 ms | 2.7 ms| 0% | 99% | 0:00:10 | 24 ms | 2.4 ms |
| 1887 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 129 µs | 120 µs| 0% | 92% | 0:00:12.710386 | 125 µs | 9.9 µs |
| 1912 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.8 µs | 22 µs | 70 µs| 0% | 100% | 0:00:10.312768 | 14 µs | 1.3 µs |
| 1913 | Unprioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 555 µs | 9.6 ms | 1.2 ms| 0% | 9% | 0:00:10.211359 | 7.5 ms | 737 µs |
| 1973 | Unprioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.4 µs | 23 µs | 65 µs| 0% | 10% | 0:06:19.902586 | 908 µs | 2.4 µs |
| 2018 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 32 ns | 99 ns | 25 µs| 0% | 91% | 0:00:49.010429 | 299 ms | 6.1 ms |
| 2027 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 33 ns | 104 ns | 25 µs| 0% | 96% | 0:00:41.003659 | 392 ms | 9.6 ms |
| 2033 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 35 ns | 97 ns | 25 µs| 0% | 85% | 0:00:36.783634 | 497 ms | 14 ms |
| 2091 | Unprioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 31 ns | 95 ns | 25 µs| 0% | 88% | 0:00:28.997915 | 128 ms | 4.4 ms |
### Benchmark: Prioritized Network 100% Load
_Id: `load/net_prioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 100% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 1000 Mbit/s.The network traffic generated by iPerf is marked with a low priority DSCP value. This should allow the network to prioritize PTP traffic over the generated network traffic, which is expected to improve the PTP performance under network contention. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 218 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.6 µs | 67 µs | 1.5 ms| 0% | 6% | 0:00:47.885942 | 70 µs | 1.5 µs |
| 229 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 6.9 ms | 121 µs| 0% | 69% | 0:00:10 | 4.8 ms | 476 µs |
| 228 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 31 µs | 62 µs| 0% | 100% | 0:00:23.575194 | 26 µs | 1.1 µs |
| 227 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 732 µs | 2.3 ms | 2.9 ms| 0% | 16% | 0:00:16.000176 | 1.9 ms | 120 µs |
| 226 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.2 µs | 17 µs | 63 µs| 0% | 9% | 0:00:45.859036 | 45 µs | 979 ns |
| 220 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 ms | 10 ms | 2.5 ms| 0% | 100% | 0:00:13.818399 | 12 ms | 843 µs |
| 243 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 95 µs | 366 µs | 3.2 ms| 0% | 0% | 0:02:23.979294 | 2.0 ms | 14 µs |
| 246 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 8.3 ms | 120 µs| 0% | 36% | 0:00:17.467196 | 17 ms | 947 µs |
| 248 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 403 µs | 1.6 ms | 1.8 ms| 0% | 13% | 0:01:33.003873 | 3.7 ms | 40 µs |
| 251 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.6 µs | 18 µs | 64 µs| 0% | 9% | 0:01:22.991398 | 57 µs | 684 ns |
| 253 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 ms | 11 ms | 2.7 ms| 0% | 100% | 0:00:10 | 24 ms | 2.4 ms |
| 467 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 ms | 9.2 ms | 2.9 ms| 0% | 2% | 0:00:10 | 4.5 ms | 449 µs |
| 461 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 502 µs | 1.8 ms | 2.0 ms| 0% | 16% | 0:00:50.006843 | 3.1 ms | 61 µs |
| 458 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.7 µs | 63 µs | 1.7 ms| 0% | 4% | 0:01:14.976065 | 70 µs | 939 ns |
| 453 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 757 µs | 2.6 ms | 2.9 ms| 0% | 11% | 0:00:37.001601 | 2.1 ms | 57 µs |
| 331 | Prioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 39 ns | 121 ns | 52 µs| 0% | 85% | 0:00:27.134570 | 307 µs | 11 µs |
| 470 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 18 µs | 7.4 ms | 140 µs| 0% | 18% | 0:00:10 | 1.0 ms | 103 µs |
| 338 | Prioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 176 µs | 466 µs | 1.3 ms| 0% | 100% | 0:00:18.008395 | 581 µs | 32 µs |
| 326 | Prioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 94 µs | 225 µs | 1.2 ms| 0% | 100% | 0:00:11.005860 | 703 µs | 64 µs |
| 254 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 131 µs | 119 µs| 0% | 94% | 0:00:16.509021 | 149 µs | 9.0 µs |
| 250 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 ms | 8.0 ms | 2.4 ms| 0% | 2% | 0:00:10.961214 | 20 ms | 1.8 ms |
| 249 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.2 µs | 23 µs | 69 µs| 0% | 100% | 0:00:10.505252 | 20 µs | 1.9 µs |
| 247 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 57 µs | 1.9 ms| 0% | 4% | 0:00:51.983548 | 77 µs | 1.5 µs |
| 245 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 35 µs | 62 µs| 0% | 100% | 0:00:10 | 24 µs | 2.4 µs |
| 244 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 13 µs | 59 µs| 0% | 91% | 0:00:11.004437 | 11 µs | 1.0 µs |
| 343 | Prioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 37 ns | 106 ns | 52 µs| 0% | 79% | 0:00:31.093583 | 11 µs | 343 ns |
| 336 | Prioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 9.0 µs | 27 µs | 1.3 ms| 0% | 16% | 0:02:39.967186 | 1.1 ms | 6.6 µs |
| 335 | Prioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 37 ns | 119 ns | 52 µs| 0% | 84% | 0:00:18.120945 | 319 µs | 18 µs |
| 327 | Prioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 37 ns | 108 ns | 52 µs| 0% | 83% | 0:00:21.311516 | 62 µs | 2.9 µs |
| 324 | Prioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.6 µs | 20 µs | 1.3 ms| 0% | 16% | 0:03:22.981070 | 909 µs | 4.5 µs |
| 457 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 107 µs | 289 µs | 4.3 ms| 0% | 0.6% | 0:02:23.975610 | 2.5 ms | 17 µs |
| 462 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 14 µs | 59 µs| 0% | 88% | 0:00:29.002983 | 15 µs | 518 ns |
| 471 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.4 µs | 5.5 ms | 121 µs| 0% | 40% | 0:00:11.707061 | 10.0 ms | 850 µs |
| 464 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.4 µs | 20 µs | 62 µs| 0% | 96% | 0:00:13.009797 | 34 µs | 2.6 µs |
| 456 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.6 µs | 18 µs | 64 µs| 0% | 12% | 0:01:17.892272 | 47 µs | 603 ns |
| 466 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 496 µs | 10.0 ms | 1.1 ms| 0% | 4% | 0:00:16.979049 | 11 ms | 653 µs |
| 463 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.2 µs | 34 µs | 62 µs| 0% | 99% | 0:00:10 | 34 µs | 3.4 µs |
| 451 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 ms | 11 ms | 2.4 ms| 0% | 99% | 0:00:10.847566 | 13 ms | 1.2 ms |
| 1049 | Prioritized Network 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 8.3 µs | 15 µs | 36 µs| 0% | 36% | 0:00:19.036772 | 38 µs | 2.0 µs |
| 1051 | Prioritized Network 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 32 µs | 112 µs | 375 µs| 0% | 9% | 0:00:46.975201 | 314 µs | 6.7 µs |
| 1041 | Prioritized Network 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 34 µs | 115 µs | 62 µs| 0% | 7% | 0:00:50.168671 | 192 µs | 3.8 µs |
| 1053 | Prioritized Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 13 µs | 131 µs | 37 µs| 0% | 100% | 0:00:19.005581 | 54 µs | 2.8 µs |
| 1043 | Prioritized Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 16 µs | 93 µs | 28 µs| 0% | 99% | 0:00:10 | 55 µs | 5.5 µs |
| 1054 | Prioritized Network 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 5.8 µs | 14 µs | 36 µs| 4% | 54% | 0:00:10 | 37 µs | 3.7 µs |
| 1044 | Prioritized Network 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 576 ns | 13 µs | 20 µs| 0% | 58% | 0:00:24.333632 | 88 µs | 3.6 µs |
| 1047 | Prioritized Network 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 5.1 µs | 1.1 ms | 17 µs| 70% | 85% | 0:00:52.971256 | 362 µs | 6.8 µs |
| 1040 | Prioritized Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 87 µs | 230 µs | 1.2 ms| 0% | 99% | 0:00:12.003507 | 280 µs | 23 µs |
| 1048 | Prioritized Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 234 µs | 609 µs | 373 µs| 0% | 99% | 0:00:10.005705 | 710 µs | 71 µs |
| 2000 | Prioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 29 ns | 83 ns | 25 µs| 0% | 97% | 0:00:51.919120 | 172 ms | 3.3 ms |
| 1998 | Prioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 7.1 µs | 26 µs | 1.3 ms| 0% | 7% | 0:06:21.961978 | 893 µs | 2.3 µs |
| 1411 | Prioritized Network 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 363 ns | 8.9 µs | 9.0 µs| 0% | 92% | 0:00:10 | 13 µs | 1.3 µs |
| 1415 | Prioritized Network 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.0 µs | 16 µs | 239 µs| 0% | 81% | 0:00:11.138737 | 55 µs | 5.0 µs |
| 219 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 356 µs | 1.3 ms | 1.6 ms| 0% | 17% | 0:03:36.019531 | 3.9 ms | 18 µs |
| 455 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 100 µs | 312 µs | 4.2 ms| 0% | 0% | 0:02:37.901371 | 3.3 ms | 21 µs |
| 465 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 13 µs | 62 µs| 0% | 100% | 0:00:12.006362 | 21 µs | 1.7 µs |
| 459 | Prioritized Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 75 µs | 240 µs | 3.4 ms| 0% | 0.9% | 0:02:30.917056 | 5.0 ms | 33 µs |
| 452 | Prioritized Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.5 µs | 35 µs | 62 µs| 0% | 100% | 0:00:12.508457 | 17 µs | 1.4 µs |
| 328 | Prioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 5.6 µs | 21 µs | 1.3 ms| 0% | 10% | 0:03:01.977469 | 899 µs | 4.9 µs |
| 252 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 538 µs | 1.8 ms | 2.1 ms| 0% | 17% | 0:01:11.004469 | 2.1 ms | 30 µs |
| 1410 | Prioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 30 ns | 83 ns | 25 µs| 0% | 97% | 0:00:29.690650 | 123 ms | 4.2 ms |
| 460 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 480 µs | 1.8 ms | 2.4 ms| 0% | 21% | 0:00:31.002939 | 1.6 ms | 52 µs |
| 1052 | Prioritized Network 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 554 ns | 18 µs | 17 µs| 0% | 92% | 0:00:16.015754 | 825 ms | 52 ms |
| 1820 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 17 µs | 8.2 ms | 139 µs| 0% | 12% | 0:00:13.172110 | 9.0 ms | 681 µs |
| 1819 | Prioritized Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 626 µs | 1.7 ms | 2.3 ms| 0% | 19% | 0:01:29.225096 | 2.3 ms | 26 µs |
| 1821 | Prioritized Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 22 µs | 9.1 ms | 145 µs| 0% | 14% | 0:00:10 | 13 ms | 1.3 ms |
| 2012 | Prioritized Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 39 ns | 125 ns | 52 µs| 0% | 84% | 0:00:18.225313 | 15 µs | 841 ns |
| 2019 | Prioritized Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 6.8 µs | 28 µs | 1.3 ms| 0% | 16% | 0:06:34.014061 | 924 µs | 2.3 µs |
| 2021 | Prioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 31 ns | 89 ns | 25 µs| 0% | 97% | 0:00:28.994261 | 135 ms | 4.7 ms |
| 2029 | Prioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 33 ns | 102 ns | 25 µs| 0% | 90% | 0:00:42.759763 | 886 ms | 21 ms |
| 2035 | Prioritized Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 29 ns | 97 ns | 25 µs| 0% | 97% | 0:00:27.991098 | 15 ms | 546 µs |
### Benchmark: Isolated Network 100% Load
_Id: `load/net_isolated/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 100% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 1000 Mbit/s.The network traffic generated by iPerf uses a secondary network interface that is different from the network interface used by PTP. The secondary network interface is specified in the machine configuration. This will isolate the network traffic from the PTP applications, which is expected to improve the PTP performance under network contention. The network traffic is also marked with a low priority DSCP value, to avoid disrupting SSH and database connections as well as other traffic on the secondary interface. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 224 | Isolated Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 9.7 µs | 69 µs| 2% | 100% | 0:00:10 | 18 µs | 1.8 µs |
| 238 | Isolated Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.2 µs | 13 µs | 63 µs| 0.3% | 100% | 0:00:21.199320 | 28 µs | 1.3 µs |
| 239 | Isolated Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 11 µs | 69 µs| 0.7% | 100% | 0:00:10 | 16 µs | 1.6 µs |
| 237 | Isolated Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.9 µs | 18 µs | 68 µs| 0.6% | 12% | 0:00:39.837856 | 60 µs | 1.5 µs |
| 233 | Isolated Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 6.9 µs | 128 µs| 3% | 96% | 0:00:10 | 24 µs | 2.4 µs |
| 240 | Isolated Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 6.0 µs | 128 µs| 0.3% | 97% | 0:00:10 | 8.6 µs | 858 ns |
| 259 | Isolated Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.2 µs | 15 µs | 66 µs| 4% | 14% | 0:00:28.625669 | 60 µs | 2.1 µs |
| 262 | Isolated Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 7.2 µs | 128 µs| 9% | 93% | 0:00:10 | 13 µs | 1.3 µs |
| 266 | Isolated Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 6.5 µs | 128 µs| 5% | 96% | 0:00:10.995374 | 29 µs | 2.6 µs |
| 357 | Isolated Network 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 269 ns | 821 ns | 37 µs| 0.3% | 96% | 0:00:15.212924 | 64 ms | 4.2 ms |
| 265 | Isolated Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 µs | 6.3 µs | 69 µs| 3% | 100% | 0:00:10 | 9.9 µs | 988 ns |
| 264 | Isolated Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.9 µs | 13 µs | 63 µs| 7% | 100% | 0:00:10 | 28 µs | 2.8 µs |
| 261 | Isolated Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.6 µs | 9.3 µs | 68 µs| 3% | 100% | 0:00:10 | 7.8 µs | 782 ns |
| 260 | Isolated Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 13 µs | 63 µs| 5% | 100% | 0:00:28.416640 | 16 µs | 553 ns |
| 258 | Isolated Network 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 6.6 µs | 128 µs| 0.4% | 95% | 0:00:13.482465 | 28 µs | 2.1 µs |
| 354 | Isolated Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 549 ns | 1.9 µs | 79 µs| 6% | 100% | 0:00:10 | 12 µs | 1.2 µs |
| 349 | Isolated Network 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 316 ns | 826 ns | 37 µs| 7% | 99% | 0:00:12.013386 | 373 ms | 31 ms |
| 363 | Isolated Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 160 ns | 434 ns | 75 µs| 11% | 98% | 0:00:10 | 5.4 µs | 540 ns |
| 1064 | Isolated Network 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 376 ns | 1.1 µs | 20 µs| 0% | 99% | 0:00:15.004186 | 248 ms | 17 ms |
| 1057 | Isolated Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 326 ns | 8.5 µs | 75 µs| 37% | 58% | 0:00:10 | 6.8 µs | 677 ns |
| 1058 | Isolated Network 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 20 µs | 94 µs | 65 µs| 0% | 3% | 0:01:23.941227 | 149 µs | 1.8 µs |
| 1061 | Isolated Network 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 367 ns | 1.1 µs | 42 µs| 0% | 82% | 0:00:22.314866 | 45 µs | 2.0 µs |
| 1062 | Isolated Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.3 µs | 5.7 µs | 117 µs| 0.5% | 10% | 0:07:09.981613 | 254 µs | 591 ns |
| 1059 | Isolated Network 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 422 ns | 1.1 µs | 20 µs| 0% | 100% | 0:00:18.998362 | 756 ms | 40 ms |
| 1063 | Isolated Network 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 17 µs | 84 µs | 65 µs| 0% | 3% | 0:01:17.899346 | 130 µs | 1.7 µs |
| 1056 | Isolated Network 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 406 ns | 909 ns | 37 µs| 2% | 100% | 0:00:16.694467 | 864 ms | 52 ms |
| 1067 | Isolated Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.1 µs | 4.4 µs | 116 µs| 0.5% | 15% | 0:07:52.407368 | 255 µs | 539 ns |
| 1069 | Isolated Network 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 370 ns | 1.0 µs | 20 µs| 0% | 100% | 0:00:13.001189 | 2.8 µs | 215 ns |
| 1070 | Isolated Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 3.9 µs | 91 µs | 43 µs| 0% | 98% | 0:00:13.003604 | 10 µs | 791 ns |
| 1066 | Isolated Network 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 396 ns | 1.1 µs | 42 µs| 0.3% | 81% | 0:00:11.986022 | 3.8 µs | 321 ns |
| 1068 | Isolated Network 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 21 µs | 85 µs | 65 µs| 0% | 3% | 0:01:13.942212 | 158 µs | 2.1 µs |
| 1416 | Isolated Network 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 288 ns | 875 ns | 20 µs| 0% | 98% | 0:00:15.012918 | 3.1 µs | 205 ns |
| 1418 | Isolated Network 100% Load | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 30 ms | 81 ms | 16 ms| 1% | 95% | 0:00:10 | 64 ms | 6.4 ms |
| 1420 | Isolated Network 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 13 ms | 60 ms | 26 ms| 0% | 3% | 0:01:16.560920 | 32 ms | 416 µs |
| 362 | Isolated Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 468 ns | 1.6 µs | 79 µs| 7% | 100% | 0:00:10 | 12 µs | 1.2 µs |
| 350 | Isolated Network 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 496 ns | 1.8 µs | 79 µs| 5% | 100% | 0:00:10 | 11 µs | 1.1 µs |
| 1065 | Isolated Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 4.2 µs | 109 µs | 43 µs| 0% | 97% | 0:00:15.003787 | 3.4 µs | 225 ns |
| 236 | Isolated Network 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.9 µs | 12 µs | 63 µs| 0.4% | 100% | 0:00:13.358764 | 14 µs | 1.1 µs |
| 1060 | Isolated Network 100% Load | SPTP (Software Timestamping) | Xilinx | petalinux02 | PRIMARY_SLAVE | 5.0 µs | 115 µs | 43 µs| 0% | 98% | 0:00:12.008303 | 102 µs | 8.5 µs |
| 230 | Isolated Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.9 µs | 16 µs | 67 µs| 5% | 13% | 0:00:34.301974 | 94 µs | 2.7 µs |
| 257 | Isolated Network 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.2 µs | 9.7 µs | 69 µs| 4% | 99% | 0:00:14.660598 | 8.3 µs | 567 ns |
| 255 | Isolated Network 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 15 µs | 67 µs| 2% | 12% | 0:00:40.151724 | 71 µs | 1.8 µs |
| 351 | Isolated Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 180 ns | 466 ns | 75 µs| 10% | 93% | 0:00:10 | 6.1 µs | 611 ns |
| 2039 | Isolated Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 204 ns | 584 ns | 37 µs| 14% | 100% | 0:00:36.306691 | 853 ms | 23 ms |
| 2014 | Isolated Network 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 329 ns | 866 ns | 37 µs| 2% | 100% | 0:00:12.996662 | 282 ms | 22 ms |
| 2015 | Isolated Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 206 ns | 582 ns | 37 µs| 2% | 100% | 0:00:24.699891 | 27 ms | 1.1 ms |
| 2016 | Isolated Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 163 ns | 456 ns | 75 µs| 4% | 96% | 0:00:10 | 6.1 µs | 610 ns |
| 2023 | Isolated Network 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 316 ns | 906 ns | 37 µs| 5% | 100% | 0:00:15.003560 | 300 ms | 20 ms |
| 2024 | Isolated Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 227 ns | 505 ns | 37 µs| 5% | 100% | 0:00:43.088225 | 567 ms | 13 ms |
| 2025 | Isolated Network 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 171 ns | 473 ns | 75 µs| 9% | 94% | 0:00:11.133844 | 44 µs | 3.9 µs |
| 2030 | Isolated Network 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.1 µs | 5.5 µs | 117 µs| 3% | 19% | 0:08:59.227521 | 911 µs | 1.7 µs |
| 2031 | Isolated Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 219 ns | 608 ns | 37 µs| 8% | 100% | 0:00:28.929379 | 223 ms | 7.7 ms |
| 2036 | Isolated Network 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 203 ns | 571 ns | 37 µs| 10% | 100% | 0:00:30.949503 | 319 ms | 10 ms |
### Benchmark: Unprioritized CPU 10% Load
_Id: `load/cpu_unprioritized/load_10`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 10% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 10% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Unprioritized CPU 20% Load
_Id: `load/cpu_unprioritized/load_20`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 20% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 20% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Unprioritized CPU 33% Load
_Id: `load/cpu_unprioritized/load_33`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 33% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 33% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Unprioritized CPU 50% Load
_Id: `load/cpu_unprioritized/load_50`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 50% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 50% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1994 | Unprioritized CPU 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 14 µs | 61 µs| 0% | 19% | 0:03:10.974205 | 92 µs | 484 ns |
| 1995 | Unprioritized CPU 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.7 µs | 16 µs | 60 µs| 0% | 100% | 0:00:31.998623 | 28 µs | 875 ns |
| 2040 | Unprioritized CPU 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 7.0 µs | 62 µs| 0% | 100% | 0:00:12.373296 | 39 µs | 3.2 µs |
| 2041 | Unprioritized CPU 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 µs | 5.2 µs | 118 µs| 0% | 91% | 0:00:19.276041 | 19 µs | 987 ns |
| 2042 | Unprioritized CPU 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.6 µs | 16 µs | 62 µs| 0% | 14% | 0:02:55.068481 | 83 µs | 471 ns |
| 2043 | Unprioritized CPU 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.1 µs | 15 µs | 59 µs| 0% | 100% | 0:00:23.005943 | 36 µs | 1.5 µs |
| 2044 | Unprioritized CPU 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 9.6 µs | 62 µs| 0% | 98% | 0:00:15.015621 | 36 µs | 2.4 µs |
| 2045 | Unprioritized CPU 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.1 µs | 119 µs| 0% | 65% | 0:00:12.171459 | 35 µs | 2.9 µs |
| 2046 | Unprioritized CPU 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 14 µs | 60 µs| 0% | 14% | 0:03:26.973024 | 81 µs | 393 ns |
| 2047 | Unprioritized CPU 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.2 µs | 16 µs | 60 µs| 0% | 100% | 0:00:40.009435 | 41 µs | 1.0 µs |
| 2048 | Unprioritized CPU 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.6 µs | 63 µs| 0% | 100% | 0:00:14.003641 | 42 µs | 3.0 µs |
| 2049 | Unprioritized CPU 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 6.5 µs | 117 µs| 0% | 92% | 0:00:10 | 17 µs | 1.7 µs |
| 2050 | Unprioritized CPU 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 14 µs | 61 µs| 0% | 10% | 0:08:42.966855 | 793 µs | 1.5 µs |
| 2051 | Unprioritized CPU 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 16 µs | 62 µs| 0% | 93% | 0:00:10 | 17 µs | 1.7 µs |
| 2052 | Unprioritized CPU 50% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 8.1 µs | 63 µs| 0% | 100% | 0:00:14.008440 | 50 µs | 3.5 µs |
| 2053 | Unprioritized CPU 50% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 µs | 6.4 µs | 118 µs| 0% | 91% | 0:00:10 | 18 µs | 1.8 µs |
| 2054 | Unprioritized CPU 50% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.1 µs | 12 µs | 60 µs| 0% | 18% | 0:03:56.940446 | 82 µs | 346 ns |
| 2055 | Unprioritized CPU 50% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.8 µs | 17 µs | 60 µs| 0% | 99% | 0:00:30.018224 | 45 µs | 1.5 µs |
### Benchmark: Unprioritized CPU 66% Load
_Id: `load/cpu_unprioritized/load_66`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 66% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 66% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Unprioritized CPU 80% Load
_Id: `load/cpu_unprioritized/load_80`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 80% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 80% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Unprioritized CPU 90% Load
_Id: `load/cpu_unprioritized/load_90`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 90% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 90% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Unprioritized CPU 100% Load
_Id: `load/cpu_unprioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 100% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 364 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 18 µs | 64 µs| - | - | 0:00:41.054359 | 65 µs | 1.6 µs |
| 366 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 8.2 µs | 66 µs| - | - | 0:00:01 | 2.1 µs | 2.1 µs |
| 369 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.0 µs | 15 µs | 66 µs| - | - | 0:00:01 | 7.0 µs | 7.0 µs |
| 371 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 5.8 µs | 124 µs| - | - | 0:01:10.781411 | 27 µs | 380 ns |
| 374 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 µs | 7.7 µs | 66 µs| - | - | 0:00:01 | 370 ns | 370 ns |
| 376 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 16 µs | 65 µs| - | - | 0:01:22.746022 | 61 µs | 736 ns |
| 381 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 18 µs | 66 µs| - | - | 0:00:01 | 6.5 µs | 6.5 µs |
| 384 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.7 µs | 5.2 µs | 124 µs| - | - | 0:06:37.000144 | 225 µs | 568 ns |
| 386 | Unprioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.1 µs | 4.0 µs | 82 µs| - | - | 0:00:01 | 46 µs | 46 µs |
| 389 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 334 ns | 865 ns | 37 µs| - | - | 0:00:01 | 705 ms | 705 ms |
| 391 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 207 ns | 605 ns | 75 µs| - | - | 0:00:01 | 45 µs | 45 µs |
| 394 | Unprioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.2 µs | 4.0 µs | 81 µs| - | - | 0:00:01 | 48 µs | 48 µs |
| 397 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 329 ns | 987 ns | 37 µs| - | - | 0:00:01 | 337 ms | 337 ms |
| 365 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.9 µs | 16 µs | 66 µs| - | - | 0:00:01 | 15 µs | 15 µs |
| 367 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 5.9 µs | 124 µs| - | - | 0:01:22.066813 | 22 µs | 264 ns |
| 368 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.1 µs | 20 µs | 67 µs| - | - | 0:01:22.280967 | 63 µs | 763 ns |
| 370 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 7.1 µs | 66 µs| - | - | 0:00:01 | 1.5 µs | 1.5 µs |
| 372 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 18 µs | 71 µs| - | - | 0:00:50.999899 | 50 µs | 983 ns |
| 373 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 15 µs | 66 µs| - | - | 0:00:01 | 684 ns | 684 ns |
| 375 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 6.3 µs | 124 µs| - | - | 0:00:59.842846 | 17 µs | 289 ns |
| 377 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.4 µs | 17 µs | 66 µs| - | - | 0:00:01 | 8.9 µs | 8.9 µs |
| 378 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 8.4 µs | 67 µs| - | - | 0:00:01 | 13 µs | 13 µs |
| 379 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 6.1 µs | 125 µs| - | - | 0:00:32.400051 | 14 µs | 438 ns |
| 380 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.2 µs | 18 µs | 69 µs| - | - | 0:01:19.209631 | 66 µs | 839 ns |
| 382 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 7.7 µs | 66 µs| - | - | 0:00:01 | 3.8 µs | 3.8 µs |
| 383 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 5.8 µs | 124 µs| - | - | 0:00:01 | 23 µs | 23 µs |
| 385 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 331 ns | 888 ns | 37 µs| - | - | 0:00:01 | 520 ms | 520 ms |
| 387 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 178 ns | 578 ns | 75 µs| - | - | 0:00:01 | 12 µs | 12 µs |
| 388 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.5 µs | 8.5 µs | 123 µs| - | - | 0:05:40.000083 | 228 µs | 670 ns |
| 390 | Unprioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.2 µs | 4.0 µs | 81 µs| - | - | 0:00:01 | 47 µs | 47 µs |
| 392 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.1 µs | 6.7 µs | 124 µs| - | - | 0:06:41.000112 | 223 µs | 556 ns |
| 393 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 320 ns | 1.0 µs | 37 µs| - | - | 0:00:01 | 113 ms | 113 ms |
| 395 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 207 ns | 663 ns | 75 µs| - | - | 0:00:01 | 50 µs | 50 µs |
| 396 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.7 µs | 5.5 µs | 124 µs| - | - | 0:07:14.134240 | 222 µs | 511 ns |
| 398 | Unprioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.2 µs | 4.0 µs | 81 µs| - | - | 0:00:01 | 47 µs | 47 µs |
| 596 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 313 ns | 913 ns | 37 µs| - | - | 0:00:01 | 484 ms | 484 ms |
| 598 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 187 ns | 533 ns | 75 µs| - | - | 0:00:01 | 11 µs | 11 µs |
| 1604 | Unprioritized CPU 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 12 µs | 47 µs | 366 µs| 0% | 51% | 0:00:20.285325 | 77 µs | 3.8 µs |
| 1934 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.2 µs | 17 µs | 67 µs| 0% | 99% | 0:00:34.016850 | 35 µs | 1.0 µs |
| 595 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.8 µs | 5.9 µs | 124 µs| - | - | 0:06:00.982941 | 224 µs | 620 ns |
| 597 | Unprioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.3 µs | 4.1 µs | 81 µs| - | - | 0:00:01 | 50 µs | 50 µs |
| 599 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 251 ns | 8.5 µs | 75 µs| - | - | 0:00:01 | 11 µs | 11 µs |
| 1596 | Unprioritized CPU 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 362 ns | 1.1 µs | 42 µs| 0% | 80% | 0:00:16.245620 | 9.8 µs | 605 ns |
| 1595 | Unprioritized CPU 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 305 ns | 802 ns | 20 µs| 0% | 96% | 0:00:14.008709 | 2.7 µs | 191 ns |
| 1355 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 217 ns | 665 ns | 37 µs| 0% | - | 0:00:01 | 767 ms | 767 ms |
| 1356 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 207 ns | 597 ns | 37 µs| 0% | - | 0:00:01 | 3.8 µs | 3.8 µs |
| 1387 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 213 ns | 646 ns | 37 µs| 0% | - | 0:00:01 | 426 ms | 426 ms |
| 1423 | Unprioritized CPU 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 317 ns | 885 ns | 20 µs| 0% | - | 0:00:01 | 886 ns | 886 ns |
| 1388 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 225 ns | 668 ns | 37 µs| 0% | - | 0:00:01 | 537 ms | 537 ms |
| 1386 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 213 ns | 665 ns | 37 µs| 0% | - | 0:00:01 | 233 ms | 233 ms |
| 1422 | Unprioritized CPU 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 385 ns | 1.1 µs | 20 µs| 0% | - | 0:00:01 | 765 ms | 765 ms |
| 1424 | Unprioritized CPU 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 344 ns | 1.1 µs | 42 µs| 0% | - | 0:00:01 | 2.1 µs | 2.1 µs |
| 1425 | Unprioritized CPU 100% Load | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 8.3 µs | 28 µs | 95 µs| 0% | - | 0:00:19.981913 | 73 µs | 3.7 µs |
| 1421 | Unprioritized CPU 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 6.8 µs | 19 µs | 64 µs| 0% | - | 0:00:32.671691 | 63 µs | 1.9 µs |
| 1426 | Unprioritized CPU 100% Load | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 12 µs | 38 µs | 78 µs| 0% | - | 0:00:10 | 44 µs | 4.4 µs |
| 1428 | Unprioritized CPU 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 3.5 µs | 16 µs | 360 µs| 0% | - | 0:00:10 | 58 µs | 5.8 µs |
| 1531 | Unprioritized CPU 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 374 ns | 1.0 µs | 42 µs| 0% | 78% | 0:00:23.314762 | 22 µs | 924 ns |
| 1529 | Unprioritized CPU 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 408 ns | 1.8 µs | 20 µs| 0% | 100% | 0:00:17.002828 | 251 ms | 15 ms |
| 1589 | Unprioritized CPU 100% Load | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 7.8 µs | 34 µs | 100 µs| 0% | 12% | 0:00:34.981387 | 103 µs | 2.9 µs |
| 1590 | Unprioritized CPU 100% Load | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 12 µs | 30 µs | 78 µs| 0% | 100% | 0:00:14.002404 | 139 µs | 9.9 µs |
| 1597 | Unprioritized CPU 100% Load | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 7.0 µs | 32 µs | 99 µs| 0% | 20% | 0:00:24.965308 | 46 µs | 1.9 µs |
| 1592 | Unprioritized CPU 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 8.5 µs | 20 µs | 375 µs| 0% | 99% | 0:00:19.224408 | 92 µs | 4.8 µs |
| 1528 | Unprioritized CPU 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 5.6 µs | 19 µs | 61 µs| 0% | 11% | 0:03:50.903322 | 49 µs | 212 ns |
| 1593 | Unprioritized CPU 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 8.3 µs | 23 µs | 64 µs| 0% | 16% | 0:05:14.965157 | 228 µs | 723 ns |
| 1530 | Unprioritized CPU 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 272 ns | 833 ns | 20 µs| 0% | 98% | 0:00:14.000128 | 3.7 µs | 264 ns |
| 1594 | Unprioritized CPU 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 410 ns | 1.3 µs | 20 µs| 0% | 99% | 0:00:10 | 857 ms | 86 ms |
| 1602 | Unprioritized CPU 100% Load | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 11 µs | 33 µs | 78 µs| 0% | 99% | 0:00:20.000221 | 127 µs | 6.3 µs |
| 1955 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 7.7 µs | 66 µs| 0% | 100% | 0:00:10.004992 | 14 µs | 1.4 µs |
| 1933 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.5 µs | 19 µs | 65 µs| 0% | 19% | 0:08:35.078760 | 1.6 ms | 3.0 µs |
| 1970 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 15 µs | 66 µs| 0% | 98% | 0:00:10 | 28 µs | 2.8 µs |
| 1971 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 7.6 µs | 66 µs| 0% | 100% | 0:00:11.003987 | 11 µs | 962 ns |
| 1972 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 6.2 µs | 125 µs| 0% | 92% | 0:00:10.153182 | 16 µs | 1.6 µs |
| 1956 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.5 µs | 6.5 µs | 124 µs| 0% | 97% | 0:00:19.211979 | 29 µs | 1.5 µs |
| 1957 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.1 µs | 23 µs | 66 µs| 0% | 9% | 0:02:46.985161 | 116 µs | 693 ns |
| 1958 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.9 µs | 14 µs | 67 µs| 0% | 98% | 0:00:33.008676 | 26 µs | 794 ns |
| 1959 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 7.8 µs | 66 µs| 0% | 100% | 0:00:16.007055 | 22 µs | 1.3 µs |
| 1960 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 6.1 µs | 125 µs| 0% | 98% | 0:00:16.180249 | 22 µs | 1.3 µs |
| 1961 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.8 µs | 21 µs | 65 µs| 0% | 12% | 0:03:44.979459 | 124 µs | 553 ns |
| 1962 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 13 µs | 66 µs| 0% | 98% | 0:00:18.004197 | 41 µs | 2.3 µs |
| 1963 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.4 µs | 8.4 µs | 66 µs| 0% | 100% | 0:00:10 | 15 µs | 1.5 µs |
| 1964 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 µs | 6.6 µs | 124 µs| 0% | 95% | 0:00:19.242780 | 26 µs | 1.4 µs |
| 1965 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.5 µs | 22 µs | 66 µs| 0% | 14% | 0:03:20.977527 | 119 µs | 594 ns |
| 1966 | Unprioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.9 µs | 16 µs | 66 µs| 0% | 100% | 0:00:11.000511 | 11 µs | 1.0 µs |
| 1967 | Unprioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.5 µs | 8.3 µs | 66 µs| 0% | 100% | 0:00:12.022320 | 16 µs | 1.3 µs |
| 1968 | Unprioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.6 µs | 6.8 µs | 125 µs| 0% | 97% | 0:00:15.206878 | 37 µs | 2.4 µs |
| 1969 | Unprioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.7 µs | 20 µs | 65 µs| 0% | 10% | 0:03:32.986533 | 120 µs | 564 ns |
### Benchmark: Prioritized CPU 100% Load
_Id: `load/cpu_prioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 100% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. The Stress-NG CPU load is generated using the idle scheduler, which is expected to give priority to the PTP applications over the generated CPU load. This is expected to improve the PTP performance under CPU contention. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 400 | Prioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.3 µs | 4.2 µs | 81 µs| - | - | 0:00:01 | 43 µs | 43 µs |
| 403 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.3 µs | 16 µs | 65 µs| - | - | 0:00:01 | 3.2 µs | 3.2 µs |
| 405 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 6.6 µs | 123 µs| - | - | 0:00:01 | 18 µs | 18 µs |
| 408 | Prioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 7.1 µs | 64 µs| - | - | 0:00:01 | 17 µs | 17 µs |
| 410 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.4 µs | 20 µs | 72 µs| - | - | 0:01:42.000005 | 74 µs | 722 ns |
| 416 | Prioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 6.7 µs | 65 µs| - | - | 0:00:01 | 15 µs | 15 µs |
| 419 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.4 µs | 16 µs | 64 µs| - | - | 0:00:01 | 26 µs | 26 µs |
| 421 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 5.5 µs | 123 µs| - | - | 0:00:01 | 12 µs | 12 µs |
| 401 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 226 ns | 754 ns | 75 µs| - | - | 0:00:01 | 11 µs | 11 µs |
| 402 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.1 µs | 19 µs | 69 µs| - | - | 0:01:25.999955 | 62 µs | 719 ns |
| 404 | Prioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 8.0 µs | 65 µs| - | - | 0:00:01 | 15 µs | 15 µs |
| 406 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.4 µs | 21 µs | 73 µs| - | - | 0:00:53.000101 | 68 µs | 1.3 µs |
| 407 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.4 µs | 17 µs | 65 µs| - | - | 0:00:01 | 1.7 µs | 1.7 µs |
| 409 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 6.2 µs | 123 µs| - | - | 0:00:01 | 9.2 µs | 9.2 µs |
| 411 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.7 µs | 16 µs | 64 µs| - | - | 0:00:01 | 2.5 µs | 2.5 µs |
| 412 | Prioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 7.8 µs | 65 µs| - | - | 0:00:01 | 26 µs | 26 µs |
| 413 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 6.1 µs | 123 µs| - | - | 0:01:15.901020 | 47 µs | 624 ns |
| 414 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.9 µs | 20 µs | 73 µs| - | - | 0:02:20.215430 | 65 µs | 461 ns |
| 415 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.9 µs | 17 µs | 65 µs| - | - | 0:00:01 | 3.3 µs | 3.3 µs |
| 417 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.3 µs | 6.0 µs | 123 µs| - | - | 0:00:01 | 19 µs | 19 µs |
| 418 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.3 µs | 20 µs | 72 µs| - | - | 0:01:37.000065 | 61 µs | 629 ns |
| 420 | Prioritized CPU 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.0 µs | 7.2 µs | 65 µs| - | - | 0:00:01 | 6.9 µs | 6.9 µs |
| 628 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.8 µs | 8.6 µs | 121 µs| - | - | 0:08:59.216656 | 616 µs | 1.1 µs |
| 631 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.5 µs | 8.6 µs | 121 µs| - | - | 0:06:54.761024 | 246 µs | 594 ns |
| 633 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 323 ns | 867 ns | 37 µs| - | - | 0:00:01 | 497 ms | 497 ms |
| 636 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 319 ns | 874 ns | 37 µs| - | - | 0:00:01 | 214 ms | 214 ms |
| 638 | Prioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.3 µs | 4.2 µs | 81 µs| - | - | 0:00:01 | 46 µs | 46 µs |
| 641 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 195 ns | 634 ns | 75 µs| - | - | 0:00:01 | 53 µs | 53 µs |
| 643 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 201 ns | 604 ns | 75 µs| - | - | 0:00:01 | 52 µs | 52 µs |
| 627 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.3 µs | 8.7 µs | 124 µs| - | - | 0:07:42.749754 | 618 µs | 1.3 µs |
| 629 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.6 µs | 9.5 µs | 121 µs| - | - | 0:07:33.952193 | 251 µs | 552 ns |
| 630 | Prioritized CPU 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 2.7 µs | 9.3 µs | 121 µs| - | - | 0:06:40.495267 | 251 µs | 626 ns |
| 632 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 332 ns | 853 ns | 37 µs| - | - | 0:00:01 | 744 ms | 744 ms |
| 634 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 310 ns | 888 ns | 37 µs| - | - | 0:00:01 | 299 ms | 299 ms |
| 635 | Prioritized CPU 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 338 ns | 886 ns | 37 µs| - | - | 0:00:01 | 104 ms | 104 ms |
| 637 | Prioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.3 µs | 4.4 µs | 81 µs| - | - | 0:00:01 | 46 µs | 46 µs |
| 639 | Prioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.3 µs | 4.0 µs | 81 µs| - | - | 0:00:01 | 49 µs | 49 µs |
| 640 | Prioritized CPU 100% Load | SPTP (Software Timestamping) | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 1.3 µs | 4.3 µs | 81 µs| - | - | 0:00:01 | 50 µs | 50 µs |
| 642 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 201 ns | 568 ns | 75 µs| - | - | 0:00:01 | 7.9 µs | 7.9 µs |
| 644 | Prioritized CPU 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 200 ns | 595 ns | 75 µs| - | - | 0:00:01 | 12 µs | 12 µs |
### Benchmark: Isolated CPU 100% Load
_Id: `load/cpu_isolated/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 100% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. The Stress-NG CPU load is generated using task affinity to restrict the CPU cores used by the load. PTP is thus open to use all the other cores. This will isolate the CPU load from the PTP applications, which is expected to improve the PTP performance under CPU contention. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
### Benchmark: Unprioritized Alarm 100% Load
_Id: `load/aux_alarm/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Alarm contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --alarm 4.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 506 | Unprioritized Alarm 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.7 µs | 14 µs | 58 µs| - | - | 0:00:01 | 9.5 µs | 9.5 µs |
| 577 | Unprioritized Alarm 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.7 µs | 7.5 µs | 53 µs| - | - | 0:00:46.000030 | 44 µs | 954 ns |
| 563 | Unprioritized Alarm 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 15 µs | 58 µs| - | - | 0:00:01 | 6.0 µs | 6.0 µs |
| 583 | Unprioritized Alarm 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.9 µs | 5.7 µs | 57 µs| - | - | 0:00:01 | 13 µs | 13 µs |
| 584 | Unprioritized Alarm 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.2 µs | 4.4 µs | 108 µs| - | - | 0:00:01 | 14 µs | 14 µs |
### Benchmark: Unprioritized Cache 100% Load
_Id: `load/aux_cache/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Cache contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --cache 4.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1362 | Unprioritized Cache 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 10 µs | 34 µs | 133 µs| 0% | - | 0:03:02.963075 | 200 µs | 1.1 µs |
| 1363 | Unprioritized Cache 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 343 ns | 1.1 µs | 37 µs| 0% | - | 0:00:01 | 68 ms | 68 ms |
| 1376 | Unprioritized Cache 100% Load | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 7.4 µs | 33 µs | 115 µs| 0% | - | 0:00:25.466806 | 105 µs | 4.1 µs |
| 1358 | Unprioritized Cache 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 206 ns | 690 ns | 37 µs| 0% | - | 0:00:01 | 635 ms | 635 ms |
| 1364 | Unprioritized Cache 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 197 ns | 598 ns | 75 µs| 0% | - | 0:00:01 | 24 µs | 24 µs |
| 1359 | Unprioritized Cache 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 284 ns | 825 ns | 20 µs| 0% | - | 0:00:01 | 2.7 µs | 2.7 µs |
| 1365 | Unprioritized Cache 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 21 µs | 67 µs | 114 µs| 0% | - | 0:00:01 | 10 µs | 10 µs |
| 1377 | Unprioritized Cache 100% Load | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.2 µs | 18 µs | 94 µs| 0% | - | 0:00:01 | 790 ns | 790 ns |
| 1366 | Unprioritized Cache 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 378 ns | 1.0 µs | 20 µs| 0% | - | 0:00:01 | 117 ms | 117 ms |
| 1378 | Unprioritized Cache 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 7.5 µs | 26 µs | 419 µs| 0% | - | 0:00:01 | 8.1 µs | 8.1 µs |
| 1367 | Unprioritized Cache 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 371 ns | 1.1 µs | 42 µs| 0% | - | 0:00:01 | 116 µs | 116 µs |
| 507 | Unprioritized Cache 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 34 µs | 106 µs| - | - | 0:00:01 | 56 µs | 56 µs |
| 586 | Unprioritized Cache 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 7.7 µs | 25 µs | 200 µs| - | - | 0:00:01 | 105 µs | 105 µs |
| 578 | Unprioritized Cache 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 24 µs | 64 µs | 115 µs| - | - | 0:00:22.109492 | 94 µs | 4.2 µs |
| 564 | Unprioritized Cache 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 12 µs | 38 µs | 105 µs| - | - | 0:02:08.144654 | 117 µs | 912 ns |
| 585 | Unprioritized Cache 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 16 µs | 49 µs | 118 µs| - | - | 0:00:01 | 89 µs | 89 µs |
### Benchmark: Unprioritized Cyclic 100% Load
_Id: `load/aux_cyclic/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Cyclic contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --cyclic 1.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 587 | Unprioritized Cyclic 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.1 µs | 6.8 µs | 61 µs| - | - | 0:00:01 | 354 ns | 354 ns |
| 508 | Unprioritized Cyclic 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.2 µs | 16 µs | 58 µs| - | - | 0:00:01 | 21 µs | 21 µs |
| 588 | Unprioritized Cyclic 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.0 µs | 4.1 µs | 113 µs| - | - | 0:00:01 | 5.6 µs | 5.6 µs |
| 565 | Unprioritized Cyclic 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 14 µs | 58 µs| - | - | 0:00:01 | 1.3 µs | 1.3 µs |
| 579 | Unprioritized Cyclic 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.0 µs | 15 µs | 57 µs| - | - | 0:00:59.000035 | 56 µs | 956 ns |
### Benchmark: Unprioritized Memory 100% Load
_Id: `load/aux_memory/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Memory contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --stream 4.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 1479 | Unprioritized Memory 100% Load | PTPd | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 5.0 µs | 24 µs | 117 µs| 0% | 12% | 0:00:32.969981 | 85 µs | 2.6 µs |
| 1480 | Unprioritized Memory 100% Load | PTP4L | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 4.5 µs | 24 µs | 100 µs| 0% | 99% | 0:00:10 | 16 µs | 1.6 µs |
| 1482 | Unprioritized Memory 100% Load | Chrony | Jetson TK-1 | tk1-2 | PRIMARY_SLAVE | 6.2 µs | 24 µs | 443 µs| 0% | 95% | 0:00:12.156686 | 131 µs | 11 µs |
| 1471 | Unprioritized Memory 100% Load | PTPd | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 10 µs | 28 µs | 168 µs| 0% | 7% | 0:04:47.981699 | 339 µs | 1.2 µs |
| 1472 | Unprioritized Memory 100% Load | PTP4L | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 318 ns | 881 ns | 37 µs| 0% | 100% | 0:00:10 | 565 ms | 57 ms |
| 1473 | Unprioritized Memory 100% Load | SPTP | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 197 ns | 599 ns | 37 µs| 0% | 100% | 0:00:40.322411 | 836 ms | 21 ms |
| 1474 | Unprioritized Memory 100% Load | Chrony | Raspberry Pi 5 | rpi58 | PRIMARY_SLAVE | 186 ns | 577 ns | 75 µs| 0% | 90% | 0:00:33.475529 | 60 µs | 1.8 µs |
| 510 | Unprioritized Memory 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 9.0 µs | 29 µs | 132 µs| - | - | 0:00:01 | 42 µs | 42 µs |
| 1475 | Unprioritized Memory 100% Load | PTPd | Xilinx | petalinux02 | PRIMARY_SLAVE | 11 µs | 35 µs | 101 µs| 0% | 13% | 0:02:23.970895 | 92 µs | 636 ns |
| 589 | Unprioritized Memory 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 27 µs | 144 µs| - | - | 0:00:01 | 20 µs | 20 µs |
| 590 | Unprioritized Memory 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 19 µs | 270 µs| - | - | 0:02:08.108046 | 111 µs | 863 ns |
| 566 | Unprioritized Memory 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 10 µs | 31 µs | 131 µs| - | - | 0:00:01 | 70 µs | 70 µs |
| 580 | Unprioritized Memory 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 14 µs | 48 µs | 143 µs| - | - | 0:00:28.000162 | 99 µs | 3.5 µs |
| 1476 | Unprioritized Memory 100% Load | PTP4L | Xilinx | petalinux02 | PRIMARY_SLAVE | 376 ns | 1.3 µs | 20 µs| 0% | 99% | 0:00:10 | 603 ms | 60 ms |
| 662 | Unprioritized Memory 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 19 µs | 62 µs | 157 µs| - | - | 0:00:52.321347 | 119 µs | 2.3 µs |
| 663 | Unprioritized Memory 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 17 µs | 54 µs | 141 µs| - | - | 0:00:32.252506 | 118 µs | 3.7 µs |
| 664 | Unprioritized Memory 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 26 µs | 133 µs| - | - | 0:00:01 | 27 µs | 27 µs |
| 1477 | Unprioritized Memory 100% Load | SPTP | Xilinx | petalinux02 | PRIMARY_SLAVE | 287 ns | 820 ns | 20 µs| 0% | 100% | 0:00:15.027345 | 2.8 µs | 186 ns |
| 1478 | Unprioritized Memory 100% Load | Chrony | Xilinx | petalinux02 | PRIMARY_SLAVE | 362 ns | 1.1 µs | 42 µs| 0% | 80% | 0:00:27.575622 | 59 µs | 2.1 µs |
### Benchmark: Unprioritized Switch 100% Load
_Id: `load/aux_switch/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Switch contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --switch 4.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 556 | Unprioritized Switch 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.9 µs | 10 µs | 51 µs| - | - | 0:02:00.009443 | 31 µs | 257 ns |
| 591 | Unprioritized Switch 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.7 µs | 4.8 µs | 57 µs| - | - | 0:00:01 | 2.9 µs | 2.9 µs |
| 592 | Unprioritized Switch 100% Load | Chrony | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 996 ns | 3.3 µs | 106 µs| - | - | 0:00:01 | 14 µs | 14 µs |
| 567 | Unprioritized Switch 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.4 µs | 9.9 µs | 52 µs| - | - | 0:00:01 | 17 µs | 17 µs |
| 568 | Unprioritized Switch 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 10 µs | 52 µs| - | - | 0:00:01 | 938 ns | 938 ns |
| 581 | Unprioritized Switch 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 2.3 µs | 7.0 µs | 54 µs| - | - | 0:02:42.626012 | 52 µs | 323 ns |
### Benchmark: Unprioritized Timer 100% Load
_Id: `load/aux_timer/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Timer contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --timer 4.


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 575 | Unprioritized Timer 100% Load | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.3 µs | 11 µs | 49 µs| - | - | 0:00:32.001305 | 16 µs | 494 ns |
| 593 | Unprioritized Timer 100% Load | SPTP | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.4 µs | 4.1 µs | 56 µs| - | - | 0:00:01 | 11 µs | 11 µs |
| 582 | Unprioritized Timer 100% Load | PTPd | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 1.8 µs | 7.0 µs | 52 µs| - | - | 0:03:12.483815 | 52 µs | 271 ns |
### Benchmark: Config Interval +3
_Id: `config/interval/+3`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 887 | Config Interval +3 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.9 µs | 14 µs | 63 µs| - | - | 0:05:20.001370 | 78 µs | 245 ns |
| 955 | Config Interval +3 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 12 µs | 64 µs| - | - | 0:00:01 | 4.8 µs | 4.8 µs |
| 944 | Config Interval +3 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 20 µs | 63 µs| - | - | 0:00:01 | 29 µs | 29 µs |
### Benchmark: Config Interval +2
_Id: `config/interval/+2`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 888 | Config Interval +2 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.1 µs | 12 µs | 62 µs| - | - | 0:00:01 | 3.3 µs | 3.3 µs |
| 956 | Config Interval +2 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 10 µs | 64 µs| - | - | 0:00:01 | 15 µs | 15 µs |
| 945 | Config Interval +2 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.7 µs | 10 µs | 64 µs| - | - | 0:00:01 | 6.4 µs | 6.4 µs |
### Benchmark: Config Interval +1
_Id: `config/interval/+1`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 916 | Config Interval +1 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.0 µs | 14 µs | 64 µs| - | - | 0:00:01 | 5.5 µs | 5.5 µs |
| 957 | Config Interval +1 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.3 µs | 12 µs | 64 µs| - | - | 0:00:01 | 6.7 µs | 6.7 µs |
| 946 | Config Interval +1 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.0 µs | 12 µs | 61 µs| - | - | 0:00:01 | 2.9 µs | 2.9 µs |
### Benchmark: Config Interval +0
_Id: `config/interval/+0`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 890 | Config Interval +0 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.8 µs | 13 µs | 58 µs| - | - | 0:00:01 | 11 µs | 11 µs |
| 947 | Config Interval +0 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.0 µs | 15 µs | 58 µs| - | - | 0:00:01 | 4.7 µs | 4.7 µs |
| 958 | Config Interval +0 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 3.6 µs | 14 µs | 58 µs| - | - | 0:00:32.987742 | 20 µs | 614 ns |
### Benchmark: Config Interval -1
_Id: `config/interval/-1`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 891 | Config Interval -1 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.8 µs | 14 µs | 58 µs| - | - | 0:00:01 | 13 µs | 13 µs |
| 959 | Config Interval -1 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.3 µs | 14 µs | 58 µs| - | - | 0:00:01 | 14 µs | 14 µs |
| 948 | Config Interval -1 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 4.9 µs | 14 µs | 59 µs| - | - | 0:00:01 | 17 µs | 17 µs |
### Benchmark: Config Interval -2
_Id: `config/interval/-2`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 892 | Config Interval -2 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.5 µs | 15 µs | 58 µs| - | - | 0:00:01 | 16 µs | 16 µs |
| 960 | Config Interval -2 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 5.7 µs | 14 µs | 57 µs| - | - | 0:00:01 | 14 µs | 14 µs |
| 949 | Config Interval -2 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 15 µs | 57 µs| - | - | 0:00:01 | 19 µs | 19 µs |
### Benchmark: Config Interval -3
_Id: `config/interval/-3`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 961 | Config Interval -3 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.9 µs | 14 µs | 58 µs| - | - | 0:00:01 | 22 µs | 22 µs |
| 950 | Config Interval -3 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.7 µs | 14 µs | 58 µs| - | - | 0:00:01 | 18 µs | 18 µs |
### Benchmark: Config Interval -4
_Id: `config/interval/-4`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 918 | Config Interval -4 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 16 µs | 60 µs| - | - | 0:00:02.066860 | 26 µs | 12 µs |
| 962 | Config Interval -4 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 15 µs | 59 µs| - | - | 0:00:01 | 23 µs | 23 µs |
| 951 | Config Interval -4 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 8.3 µs | 15 µs | 60 µs| - | - | 0:00:01 | 26 µs | 26 µs |
### Benchmark: Config Interval -5
_Id: `config/interval/-5`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 895 | Config Interval -5 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.0 µs | 17 µs | 59 µs| - | - | 0:00:01 | 17 µs | 17 µs |
| 963 | Config Interval -5 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.1 µs | 16 µs | 59 µs| - | - | 0:00:01 | 43 µs | 43 µs |
| 952 | Config Interval -5 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 6.3 µs | 17 µs | 59 µs| - | - | 0:00:01 | 19 µs | 19 µs |
### Benchmark: Config Interval -6
_Id: `config/interval/-6`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 896 | Config Interval -6 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 267 µs | 56 µs| - | - | 0:00:01 | 19 µs | 19 µs |
| 953 | Config Interval -6 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 11 µs | 243 µs | 57 µs| - | - | 0:00:01 | 26 µs | 26 µs |
| 964 | Config Interval -6 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 44 µs | 528 µs | 57 µs| - | - | 0:00:01.699430 | 27 µs | 16 µs |
### Benchmark: Config Interval -7
_Id: `config/interval/-7`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 


| Profile id | Benchmark | Vendor | Cluster | Machine | Endpoint type | Clock diff median | Clock diff p95 | Path delay median | Missing samples percent | Converged percentage | Convergence duration | Convergence max offset | Convergence rate |
|------------|-----------|--------|---------|---------|---------------|-------------------|----------------|-------------------|-------------------------|----------------------|----------------------|------------------------|------------------|
| 897 | Config Interval -7 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 201 µs | 2.6 ms | 52 µs| - | - | 0:00:01.450598 | 24 µs | 16 µs |
| 954 | Config Interval -7 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 33 µs | 1.1 ms | 53 µs| - | - | 0:00:01 | 32 µs | 32 µs |
| 965 | Config Interval -7 | PTP4L | Raspberry Pi 4 | rpi08 | PRIMARY_SLAVE | 20 µs | 229 µs | 53 µs| - | - | 0:00:01 | 36 µs | 36 µs |
