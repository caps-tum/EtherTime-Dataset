# Benchmark Database

This document provides an overview of all benchmarks in the database, according to category. Each benchmark is described with its key properties and a brief explanation of what it measures. For more detailed information, see the benchmark definition in the source code at `ptp_perf/registry/benchmark_db.py`.

### Benchmark: Baseline
_Id: `base`, 2 machines, 0:20:00 duration._

The base benchmark to compare other benchmarks against. It is the default benchmark for all new clusters. It is used to measure the performance of the cluster without any additional load or faults. 

### Benchmark: Test
_Id: `test/test`, 2 machines, 0:01:00 duration._

A test benchmark to quickly verify the cluster is working correctly. It is identical to the base benchmark but runs for a shorter duration.

### Benchmark: Demo
_Id: `test/demo`, 2 machines, 0:05:00 duration._

A demo benchmark to quickly assess the capabilities of the cluster. It is identical to the base benchmark but runs for a shorter duration.

### Benchmark: 2 Nodes
_Id: `scalability/1_to_1`, 2 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 2 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 3 Nodes
_Id: `scalability/1_to_2`, 3 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 3 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 12 Nodes
_Id: `scalability/1_to_11`, 12 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 12 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 4 Nodes
_Id: `scalability/1_to_3`, 4 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 4 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 5 Nodes
_Id: `scalability/1_to_4`, 5 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 5 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 6 Nodes
_Id: `scalability/1_to_5`, 6 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 6 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 7 Nodes
_Id: `scalability/1_to_6`, 7 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 7 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 8 Nodes
_Id: `scalability/1_to_7`, 8 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 8 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 9 Nodes
_Id: `scalability/1_to_8`, 9 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 9 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 10 Nodes
_Id: `scalability/1_to_9`, 10 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 10 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: 11 Nodes
_Id: `scalability/1_to_10`, 11 machines, 0:20:00 duration._

The benchmark is used to measure the performance of the cluster 11 nodes. The first node in the cluster is the master, the second node the primary slave. Further nodes are assigned as secondary/tertiary slaves where applicable.A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark. 

### Benchmark: Software Fault (Slave)
_Id: `fault/software/slave`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a software fault on a slave. The software fault is created by killing and restarting the PTP daemon on the slave machine. A second slave is used as a control node to check whether it is affected by the fault. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.

### Benchmark: Hardware Fault (Switch)
_Id: `fault/hardware/switch`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on the network switch. The hardware fault is created by turning off the power to the network switch using a smart PDU (check the documentation on how to register it with PTP-Perf). It is expected that both the primary and the secondary slave are affected by the network outage. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.

### Benchmark: Hardware Fault (Slave)
_Id: `fault/hardware/slave`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on a slave. The hardware fault is created by turning off the power to the slave machine using a smart PDU (check the documentation on how to register it with PTP-Perf). A second slave is used as a control node to check whether it is affected by the fault. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.

### Benchmark: Hardware Fault (Master)
_Id: `fault/hardware/master`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on the master. The hardware fault is created by turning off the power to the master machine using a smart PDU (check the documentation on how to register it with PTP-Perf). A second slave is used as a control node, it is expected to also be affected by the fault. The fault occurs 10 minutes into the benchmark and lasts for 1 minute.

### Benchmark: Hardware Fault (Failover)
_Id: `fault/hardware/master_failover`, 3 machines, 0:15:00 duration._

A benchmark to measure the performance of the cluster with a hardware fault on the master but with a failover master on the secondary slave that will take over once the primary master fails. The fault occurs 10 minutes into the benchmark and lasts for 1 minute. After the fault is resolved, the failover master will be demoted back to a slave, allowing the primary master to take over again. The benchmark is expected to show a seamless transition between the primary and failover masters. The hardware fault is created by turning off the power to the master machine using a smart PDU (check the documentation on how to register it with PTP-Perf). 

### Benchmark: No Switch
_Id: `configuration/no_switch`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster without a network switch. The configuration is identical to the baseline, the user is expected to rewire the cluster appropriately before running this benchmark. 

### Benchmark: Resource Consumption
_Id: `resource_consumption`, 2 machines, 0:20:00 duration._

A benchmark to measure the resource consumption of the PTP applications on each node. Collected metrics include CPU usage, memory usage, network traffic, and clock synchronization statistics. The benchmark runs for 15 minutes to collect a sufficient amount of data. It is otherwise identical to the base benchmark.

### Benchmark: Unprioritized Network 10% Load
_Id: `load/net_unprioritized/load_10`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 10% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 10% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 100 Mbit/s.

### Benchmark: Unprioritized Network 20% Load
_Id: `load/net_unprioritized/load_20`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 20% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 20% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 200 Mbit/s.

### Benchmark: Unprioritized Network 33% Load
_Id: `load/net_unprioritized/load_33`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 33% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 33% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 330 Mbit/s.

### Benchmark: Unprioritized Network 50% Load
_Id: `load/net_unprioritized/load_50`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 50% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 50% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 500 Mbit/s.

### Benchmark: Unprioritized Network 66% Load
_Id: `load/net_unprioritized/load_66`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 66% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 66% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 660 Mbit/s.

### Benchmark: Unprioritized Network 80% Load
_Id: `load/net_unprioritized/load_80`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 80% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 80% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 800 Mbit/s.

### Benchmark: Unprioritized Network 90% Load
_Id: `load/net_unprioritized/load_90`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 90% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 90% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 900 Mbit/s.

### Benchmark: Unprioritized Network 100% Load
_Id: `load/net_unprioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 100% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 1000 Mbit/s.

### Benchmark: Prioritized Network 100% Load
_Id: `load/net_prioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 100% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 1000 Mbit/s.The network traffic generated by iPerf is marked with a low priority DSCP value. This should allow the network to prioritize PTP traffic over the generated network traffic, which is expected to improve the PTP performance under network contention. 

### Benchmark: Isolated Network 100% Load
_Id: `load/net_isolated/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of Network contention. The Network is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The network load is generated using iPerf, a network performance testing tool. The target bandwidth is set to 100% of the network interface capacity.  A GigaBit Ethernet network interface is assumed, so the load is 1000 Mbit/s.The network traffic generated by iPerf uses a secondary network interface that is different from the network interface used by PTP. The secondary network interface is specified in the machine configuration. This will isolate the network traffic from the PTP applications, which is expected to improve the PTP performance under network contention. The network traffic is also marked with a low priority DSCP value, to avoid disrupting SSH and database connections as well as other traffic on the secondary interface. 

### Benchmark: Unprioritized CPU 10% Load
_Id: `load/cpu_unprioritized/load_10`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 10% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 10% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Unprioritized CPU 20% Load
_Id: `load/cpu_unprioritized/load_20`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 20% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 20% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Unprioritized CPU 33% Load
_Id: `load/cpu_unprioritized/load_33`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 33% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 33% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Unprioritized CPU 50% Load
_Id: `load/cpu_unprioritized/load_50`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 50% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 50% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Unprioritized CPU 66% Load
_Id: `load/cpu_unprioritized/load_66`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 66% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 66% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Unprioritized CPU 80% Load
_Id: `load/cpu_unprioritized/load_80`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 80% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 80% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Unprioritized CPU 90% Load
_Id: `load/cpu_unprioritized/load_90`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 90% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 90% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Unprioritized CPU 100% Load
_Id: `load/cpu_unprioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 100% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. 

### Benchmark: Prioritized CPU 100% Load
_Id: `load/cpu_prioritized/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 100% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. The Stress-NG CPU load is generated using the idle scheduler, which is expected to give priority to the PTP applications over the generated CPU load. This is expected to improve the PTP performance under CPU contention. 

### Benchmark: Isolated CPU 100% Load
_Id: `load/cpu_isolated/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under different levels of CPU contention. The CPU is loaded to 100% of its capacity. This is expected to affect the performance of the PTP applications running on the cluster. The CPU load is generated using Stress-NG, a stress testing tool. The target CPU load is set to 100% of the CPU capacity. Each node in the cluster uses the number of cores specified in the machine configuration. The Stress-NG CPU load is generated using task affinity to restrict the CPU cores used by the load. PTP is thus open to use all the other cores. This will isolate the CPU load from the PTP applications, which is expected to improve the PTP performance under CPU contention. 

### Benchmark: Unprioritized Alarm 100% Load
_Id: `load/aux_alarm/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Alarm contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --alarm 4.

### Benchmark: Unprioritized Cache 100% Load
_Id: `load/aux_cache/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Cache contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --cache 4.

### Benchmark: Unprioritized Cyclic 100% Load
_Id: `load/aux_cyclic/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Cyclic contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --cyclic 1.

### Benchmark: Unprioritized Memory 100% Load
_Id: `load/aux_memory/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Memory contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --stream 4.

### Benchmark: Unprioritized Switch 100% Load
_Id: `load/aux_switch/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Switch contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --switch 4.

### Benchmark: Unprioritized Timer 100% Load
_Id: `load/aux_timer/load_100`, 2 machines, 0:20:00 duration._

A benchmark to measure the performance of the cluster under auxiliary contention. Specifically, this benchmark tests Timer contention. The auxiliary contention is generated using Stress-NG, a stress testing tool. Refer to the Stress-NG documentation for more information on the specific options used. The Stress-NG options are: --timer 4.

### Benchmark: Config Interval +3
_Id: `config/interval/+3`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval +2
_Id: `config/interval/+2`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval +1
_Id: `config/interval/+1`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval +0
_Id: `config/interval/+0`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval -1
_Id: `config/interval/-1`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval -2
_Id: `config/interval/-2`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval -3
_Id: `config/interval/-3`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval -4
_Id: `config/interval/-4`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval -5
_Id: `config/interval/-5`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval -6
_Id: `config/interval/-6`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

### Benchmark: Config Interval -7
_Id: `config/interval/-7`, 2 machines, 0:20:00 duration._

A benchmark to test the performance of the cluster with a specific PTP configuration. Currently, this is only used to modify the frequency of PTP synchronization/path delay/announce messages. Refer to PTP documentation on the meaning of these message intervals. 

