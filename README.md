![logo_nobg.svg](doc/res/logo_nobg.svg)

# EtherTime Dataset

![Last Export](https://img.shields.io/badge/Last%20Export-%202024_05_27%20-%20green)
![Profiles Collected](https://img.shields.io/badge/Profiles%20Collected-%202000+%20-%20blue)
![Log Records](https://img.shields.io/badge/Log%20Records-%2013M%20-%20blue)
![Benchmarking Runtime](https://img.shields.io/badge/Benchmarking%20Runtime-%20450+%20hours%20-%20blue)

This is an anonymized dataset of profiles collected by the EtherTime project. The dataset contains performance metrics and log records from benchmarking runs conducted on various Precision Time Protocol (PTP) clusters using different PTP vendors.

Our dataset includes over 2000 profiles, each representing a specific benchmarking run conducted on a PTP cluster using a specific PTP vendor. 
Our four clusters are the Raspberry Pi 4 and 5, the Xilinx ZUBoard 1CG, and the NVIDIA Jetson TK-1.

These clusters have the following characteristics:
- **Raspberry Pi 4**: Does not support hardware timestamping and integrated real-time clocks.    
- **Raspberry Pi 5**: Featuring hardware timestamping and integrated real-time clocks.
- **Xilinx ZUBoard 1CG**: Combining ARM Cortex A53 and R5F cores, adapted for Debian with special Xilinx Kernels.
- **NVIDIA Jetson TK-1**: 32-bit ARMv7 boards running Ubuntu 22.04 LTS with a customized  NVIDIA 3.10 Linux kernel.

The assesed vendors include:
1. **PTPd**: An established, if dated, implementation widely deployed due to its simplicity.
2. **LinuxPTP**: A robust implementation tightly integrated with Linux, leveraging kernel and hardware features.
3. **SPTP**: A modern, high-performance implementation with a focus on scalability and performance.
4. **Chrony**: A state-of-the-art NTP server/client offering extensive features and capabilities.

The dataset is organized into profiles, each of which represents a specific benchmarking run conducted on a PTP cluster using a specific PTP vendor. Each profile contains metadata about the benchmark, vendor, and cluster used, as well as a list of endpoints on which the profile was conducted. Each endpoint contains performance metrics and log records collected during the benchmarking run.

### Benchmark Overview

We provide an overview in **[Benchmark Overview](benchmark_overview.md)** for your convenience. It includes a description of the benchmarks used in the dataset, their purpose, and the conditions under which they were conducted, and a summary of the performance metrics collected during the benchmarking runs for each vendor and cluster.

### Note for Anonymized Dataset Repository

Due to size limitations in the anonymization process and our repository infrastructure, not all data could be included in the anonymized access to the repository. We tried including as much data as possible, but the anonymized dataset repository contains only a subset of the profiles and log records collected during the EtherTime project. The full dataset is available upon request.

### Data Format

The dataset is grouped into profiles. Each profile is contained within a JSON file in the `profiles` directory. 

Each profile contains metadata about the profile itself, and a list of endpoints on which the profile was conducted. A profile always consists of a combination of benchmark (defining the experimentation scenario under which it is conducted), the vendor (defining the PTP implementation used), and the cluster (metadata about the physical machines used).

Each endpoint contains metadata about the endpoint, and a list of log records and samples associated with the endpoint.

### Sample Profile
In the following, we provide a sample profile to illustrate the structure of the dataset.
Please refer to the **[Types used](#types-used)** section for a detailed description of the data structures used in the dataset.

```javascript
profile = {
    // This is a profile, it consists of a list of endpoints on which it was conducted.
    // Profiles have metadata associated with them that track the state of the benchmarking run.
    "id": 1001,
    "benchmark_id": "base",
    "vendor_id": "ptpd",
    "cluster_id": "petalinux",
    "is_running": false,
    "is_successful": true,
    "is_processed": true,
    "is_corrupted": false,
    "start_time": "2024-05-09 22:59:11.833359+00:00",
    "stop_time": "2024-05-09 23:19:16.094730+00:00",
    "benchmark": {
        // This is the benchmark definition used for this profile. 
        // It describes the conditions under which the benchmark was conducted, and what is being measured.
        // For a list of available benchmarks, and a more detailed description of the model, see the Benchmark section below.
        "id": "base",
        "name": "Baseline",
        "description": "The base benchmark to compare other benchmarks against. It is the default benchmark for all new clusters. It is used to measure the performance of the cluster without any additional load or faults. ",
        "tags": [],
        "version": 1,
        "duration": "0:20:00",
        "num_machines": 2,
        "ptp_config": {
            // The PTP configuration used for this benchmark.
            // PTP configurations define the parameters used by the PTP daemon to synchronize the clocks of the machines in the cluster.
            // EtherTime passes these via the daemon configuration file to the actual vendor implementation.
            "delay_mechanism": "E2E",
            "log_announce_interval": 1,
            "log_sync_interval": 0,
            "log_delayreq_interval": 0
        },
        "ptp_keepalive": false,
        "analyze_limit_permissible_clock_steps": 1,
        "setup_use_initial_clock_offset": true,
        // Artificial load parameters used for this benchmark.
        // These parameters are only used if the benchmark includes artificial load, such as network or CPU load.
        // We use tools like iPerf and Stress-NG to generate this load, so that we can measure the impact on the PTP performance when resource contention is introduced.
        "artificial_load_network": 0,
        "artificial_load_network_dscp_priority": null,
        "artificial_load_network_secondary_interface": false,
        "artificial_load_cpu": 0,
        "artificial_load_cpu_scheduler": null,
        "artificial_load_cpu_restrict_cores": false,
        "artificial_load_aux": false,
        "artificial_load_aux_options": null,
        // Fault parameters used for this benchmark.
        // These parameters are only used if the benchmark includes faults, such as software or hardware faults which can be programmed to occur during the benchmark on specific machines, or network links.
        // Faults are used to simulate real-world conditions that can impact the performance of the PTP cluster.
        // For example, a software fault might simulate a crash of the PTP daemon on a machine, or a hardware fault might simulate a network link failure.
        "fault_ssh_keepalive": false,
        "fault_software": false,
        "fault_hardware": false,
        "fault_interval": null,
        "fault_duration": null,
        "fault_location": null,
        "fault_failover": false,
        // Whether EtherTime should monitor resource consumption during the benchmark run.
        // Resource consumption metrics include CPU usage, memory usage, network traffic, and clock synchronization statistics.
        // Monitoring resource consumption can help identify performance bottlenecks and issues that may affect the PTP performance.
        // For example, high CPU usage on a machine may indicate that the machine is overloaded and may not be able to keep up with the PTP synchronization requirements.
        "monitor_resource_consumption": false
    },
    "vendor": {
        // This is the vendor implementation used for this profile.
        // Each vendor provides a different implementation of the PTP protocol, and the EtherTime project is designed to evaluate and compare their performance under various conditions.
        // For a list of available vendors, and a more detailed description of the model, see the Vendor section below.
        "id": "ptpd",
        "name": "PTPd",
        "supports_non_standard_config_interval": true,
        "_process": null
    },
    "cluster": {
        // This is the cluster metadata used for this profile.
        // The cluster consists of a master machine, one or more slave machines, and optionally a failover master for fault toleranc benchmarks.
        // Each cluster is defined by a unique ID.
        // See the Cluster section below for more details on the model.
        "id": "petalinux",
        "name": "Xilinx",
        "machines": [
            {
                // This is a machine in the cluster used for this profile.
                // A cluster must have at least one master machine and one slave machine.
                // This configuration is imported from the user-provided `config.py` file, and is primarily used to define the network layout and nodes used in the benchmark.
                "id": "petalinux01",
                "address": "petalinux01",
                "user": null,
                "remote_root": "/home/rpi/ptp-perf",
                "deploy_root": true,
                "ptp_interface": "end0",
                "ptp_address": "10.0.0.81",
                "endpoint_type": "MASTER",
                "ptp_software_timestamping": false,
                "ptp_use_phc2sys": false,
                "python_executable": "python3",
                "initial_clock_offset": null,
                "plugin_settings": {
                    "iperf_server": true,
                    "iperf_address": "10.0.0.81",
                    "iperf_secondary_address": "192.168.1.181",
                    "stress_ng_cpus": 2,
                    "stress_ng_cpu_restrict_cores": "1"
                },
                "shutdown_delay": "0:00:00",
                "_ssh_session": null
            },
            {
                "id": "petalinux02",
                "address": "petalinux02",
                "user": null,
                "remote_root": "/home/rpi/ptp-perf",
                "deploy_root": true,
                "ptp_interface": "end0",
                "ptp_address": "10.0.0.82",
                "endpoint_type": "PRIMARY_SLAVE",
                "ptp_software_timestamping": false,
                "ptp_use_phc2sys": false,
                "python_executable": "python3",
                "initial_clock_offset": "-1 day, 23:59:00",
                "plugin_settings": {
                    "iperf_server": false,
                    "iperf_address": "10.0.0.82",
                    "iperf_secondary_address": "192.168.1.182",
                    "stress_ng_cpus": 2,
                    "stress_ng_cpu_restrict_cores": "1"
                },
                "shutdown_delay": "0:00:00",
            },
            /// More machines...
        ]
    },
    "endpoints": [
        {
            // This is an endpoint on which the profile was conducted.
            // An endpoint is a participant in the PTP cluster running on a specific machine.
            // Slave endpoints contain the actual performance metrics collected during the benchmarking run, such as clock difference.
            "id": 3242,
            "profile": 1001,
            "machine_id": "petalinux02",
            "restart_count": 1,
            "endpoint_type": "PRIMARY_SLAVE",
            // These are the most important summary statistics collected during the benchmarking run: clock difference and path delay.
            // Clock difference is the difference between the local clock and the master clock, and path delay is the time it takes for a message to travel from the master to the slave (one way only).
            // Generally speaking, the lower the clock difference and path delay, the better the synchronization performance.
            "clock_diff_median": 1.465e-06,
            "clock_diff_p05": 1.0585000000000001e-07,
            "clock_diff_p95": 6.233749999999999e-06,
            "path_delay_median": 3.9523e-05,
            "path_delay_p05": 3.616e-05,
            "path_delay_p95": 4.33466e-05,
            "path_delay_std": 2.0900357068628822e-06,
            // These are additional statistics collected during the benchmarking run.
            // The missing samples count and missing samples percent indicate how many samples were missing during the benchmarking run, because of network issues or other problems.
            // Samples are classified as missing if they are not received within a certain time window, which corresponds to three times the synchronization interval.
            "missing_samples_count": 0,
            "missing_samples_percent": 0.0,
            // The convergence statistics indicate how quickly the clock difference converged to a stable value after the benchmarking run started.
            // Convergence is an important metric because it indicates how quickly the PTP cluster can synchronize its clocks after a change in the network or other conditions.
            // The convergence timestamp is the time at which the clock difference converged, and the convergence duration is the time it took for the clock difference to converge.
            "convergence_timestamp": "2024-05-09 22:59:52.150228+00:00",
            "convergence_duration": "0:00:12.003742",
            // The convergence max offset is the maximum clock difference observed during the convergence period, and the convergence rate is the rate at which the clock difference converged in parts per second.
            "convergence_max_offset": 6.446000000000001e-06,
            "convergence_rate": 5.369992124122628e-07,
            // The convergence percentage indicates how many samples were received while the clock was considered stable, and the convergence samples indicate the number of samples received during this stable period.
            "converged_percentage": 0.998272884283247,
            "converged_samples": 1158,
            // The clock step statistics indicate if the clock was stepped during the initial phase of the benchmarking run, and if so, when and by how much.
            "clock_step_timestamp": "2024-05-09 22:59:39.145967+00:00",
            "clock_step_magnitude": 142.726376026,
            // The fault statistics indicate if any faults were introduced during the benchmarking run, and if so, what their impact was on the performance metrics.
            // All of these fields are null if no faults were introduced.
            // Faults are used to simulate real-world conditions that can impact the performance of the PTP cluster.
            // For example, a software fault might simulate a crash of the PTP daemon on a machine, or a hardware fault might simulate a network link failure.
            // The fault clock difference and fault path delay indicate the clock difference and path delay before (pre) or after (post) the fault period.
            // The fault actual duration indicates how long the fault lasted before PTP was able to re-establish the connection, and the fault ratio indicates the ratio of the performance metrics after the fault period to the pre-fault period.
            // The fault clock diff return to normal time indicates how long it took for the clock difference to return to normal after the fault period.
            // The fault clock diff mid max indicates the maximum clock difference observed during the fault period.
            "fault_clock_diff_pre_median": null,
            "fault_clock_diff_pre_p05": null,
            "fault_clock_diff_pre_p95": null,
            "fault_path_delay_pre_median": null,
            "fault_path_delay_pre_p05": null,
            "fault_path_delay_pre_p95": null,
            "fault_clock_diff_post_median": null,
            "fault_clock_diff_post_p05": null,
            "fault_clock_diff_post_p95": null,
            "fault_path_delay_post_median": null,
            "fault_path_delay_post_p05": null,
            "fault_path_delay_post_p95": null,
            "fault_actual_duration": null,
            "fault_ratio_clock_diff_median": null,
            "fault_ratio_clock_diff_p95": null,
            "fault_clock_diff_post_max": null,
            "fault_ratio_clock_diff_post_max_pre_median": null,
            "fault_clock_diff_return_to_normal_time": null,
            "fault_clock_diff_mid_max": null,
            // If resource consumption monitoring was enabled for this endpoint, the following fields contain the resource consumption metrics collected during the benchmarking run.
            "resource_profile_length": null,
            // Proc metrics are collected from the /proc filesystem and include CPU usage, memory usage, and I/O statistics for only the PTP-related processes.
            "proc_cpu_percent": null,
            "proc_cpu_percent_system": null,
            "proc_cpu_percent_user": null,
            "proc_mem_uss": null,
            "proc_mem_pss": null,
            "proc_mem_rss": null,
            "proc_mem_vms": null,
            "proc_io_write_count": null,
            "proc_io_write_bytes": null,
            "proc_io_read_count": null,
            "proc_io_read_bytes": null,
            "proc_ctx_switches_involuntary": null,
            "proc_ctx_switches_voluntary": null,
            // Sys metrics are collected from the /sys filesystem and include system-wide metrics such as CPU temperature, CPU frequency, and network statistics.
            // These metrics are collected for the entire system, not just the PTP-related processes.
            // The sys_net_ptp_iface metrics are collected from the PTP network interface.
            "sys_sensors_temperature_cpu": null,
            "sys_cpu_frequency": null,
            "sys_net_ptp_iface_bytes_sent": null,
            "sys_net_ptp_iface_packets_sent": null,
            "sys_net_ptp_iface_bytes_received": null,
            "sys_net_ptp_iface_packets_received": null,
            "sys_net_ptp_iface_bytes_total": null,
            "sys_net_ptp_iface_packets_total": null,
            "logrecord_set": [
                // This is a list of log records collected during the benchmarking run.
                // Log records are messages generated by the PTP daemon or other processes running on the machine.
                // These messages can include information about the state of the PTP cluster, errors, warnings, and other diagnostic information.
                // Log records are converted to samples (see below) by the EtherTime system, which are then used to calculate performance metrics such as clock difference and path delay.
                // Each log record is categorized by its source (e.g., PTP daemon, SSH, etc.), timestamp, and message content.
                // Log records can be used to diagnose issues with the PTP cluster, identify performance bottlenecks, and track the progress of the benchmarking run, 
                // but EtherTime already processes these logs into performance metrics so that users don't have to manually analyze them.
                // We provide a short excerpt of an actual profile log for illustrative purposes.
                {
                    "id": 4686225,
                    "timestamp": "2024-05-09 22:59:36.582480+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| petalinux01 time is now 2024-05-09 15:59:36.577623"
                },
                {
                    "id": 4686227,
                    "timestamp": "2024-05-09 22:59:36.598806+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| Starting SPTP..."
                },
                {
                    "id": 4686229,
                    "timestamp": "2024-05-09 22:59:36.617172+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| Benchmarking for 0:19:35.219063..."
                },
                {
                    "id": 4686232,
                    "timestamp": "2024-05-09 22:59:36.635619+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| ptp-perf > ptp4u -iface end0"
                },
                {
                    "id": 4686233,
                    "timestamp": "2024-05-09 22:59:37.150958+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| | time=\"2024-05-09T15:58:37-07:00\" level=warning msg=\"new best master selected: \\\"10.0.0.81\\\" (2ad652.fffe.3076df)\""
                },
                {
                    "id": 4686235,
                    "timestamp": "2024-05-09 22:59:37.173285+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| | time=\"2024-05-09T15:58:37-07:00\" level=info msg=\"offset 142726375559 s0 freq  -17058 path delay      40423 (-142726335136:142726415982)\""
                },
                {
                    "id": 4686237,
                    "timestamp": "2024-05-09 22:59:38.147001+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| | time=\"2024-05-09T15:58:38-07:00\" level=info msg=\"offset 142726387195 s1 freq   -5379 path delay      40812 (-142726346382:142726428007)\""
                },
                {
                    "id": 4686239,
                    "timestamp": "2024-05-09 22:59:38.164193+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| | time=\"2024-05-09T15:56:15-07:00\" level=warning msg=\"clock state 5 is not TIME_OK after stepping\""
                },
                {
                    "id": 4686241,
                    "timestamp": "2024-05-09 22:59:39.145774+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| | time=\"2024-05-09T15:56:16-07:00\" level=info msg=\"offset      11169 s2 freq   +5790 path delay      40687 ( 29519: 51856)\""
                },
                {
                    "id": 4686249,
                    "timestamp": "2024-05-09 22:59:42.147217+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| | time=\"2024-05-09T15:56:19-07:00\" level=info msg=\"offset      -6446 s2 freq   -9281 path delay      40398 ( 46845: 33952)\""
                },
                {
                    "id": 4686875,
                    "timestamp": "2024-05-09 23:04:55.356791+00:00",
                    "endpoint_id": 3240,
                    "source": "ssh",
                    "message": "| | time=\"2024-05-09T16:01:32-07:00\" level=info msg=\"offset       1142 s2 freq   -5696 path delay      40012 ( 38871: 41154)\""
                },
                {
                    "id": 4688598,
                    "timestamp": "2024-05-09 23:19:11.954796+00:00",
                    "endpoint_id": 3242,
                    "source": "root",
                    "message": "Task 'SPTP' was cancelled"
                }
            ],
            "sample_set": [
                // This is a list of samples collected during the benchmarking run, the processed performance metrics.
                // Samples are generated from log records and are used to calculate summary performance metrics such as clock difference and path delay for each endpoint.
                // They can also be used to generate time series data for visualization and analysis.
                // The two most important samples are clock difference and path delay, which indicate the synchronization performance of the PTP cluster.
                // Other sample types include faults and system resource consumption metrics.
                {
                    "id": 7728138,
                    "endpoint_id": 3242,
                    "timestamp": "2024-05-09 22:59:37.172172+00:00",
                    "sample_type": "CLOCK_DIFF",
                    "value": 142726375559
                },
                {
                    "id": 7728139,
                    "endpoint_id": 3242,
                    "timestamp": "2024-05-09 22:59:37.172172+00:00",
                    "sample_type": "PATH_DELAY",
                    "value": 40423
                },
                {
                    "id": 7728140,
                    "endpoint_id": 3242,
                    "timestamp": "2024-05-09 22:59:38.145572+00:00",
                    "sample_type": "CLOCK_DIFF",
                    "value": 142726387195
                },
                {
                    "id": 7730485,
                    "endpoint_id": 3242,
                    "timestamp": "2024-05-09 23:19:10.922771+00:00",
                    "sample_type": "PATH_DELAY",
                    "value": 40908
                }
            ]
        }
    ]
}
```

## Types used

The following sections describe the types used in the dataset, for consumption by external tools or libraries.

### Profile

The `PTPProfile` class represents a profile for a Precision Time Protocol (PTP) benchmarking run. Each instance of `PTPProfile` corresponds to a specific benchmarking run, characterized by the benchmark used (`benchmark_id`), the PTP vendor (`vendor_id`), and the cluster (`cluster_id`).

The `PTPProfile` class includes several attributes for metadata that tracks the state of the benchmarking run, such as `is_running`, `is_successful`, `is_processed`, and `is_corrupted`. It also includes timestamps for when the benchmarking run started (`start_time`) and stopped (`stop_time`).

This is the base structure which each profile in the dataset consists of. Nested within the profile are the endpoints on which the profile was conducted. Each endpoint contains metadata about the endpoint, such as the machine it was conducted on, the type of endpoint, and various performance metrics collected during the benchmarking run.

See below for a reference of nested data structures found within profiles.



### Benchmark
A benchmark in this context is a specific set of conditions and parameters under which the performance of the Precision Time Protocol (PTP) cluster is tested. Each benchmark is defined by a unique ID, a human-readable name, and a description that explains what the benchmark measures. It also includes various other parameters such as the duration of the benchmark, the number of machines to use, the PTP configuration, and various options for artificial load, faults, and monitoring.

In the `benchmark_db.py` file, several benchmarks are defined using the `Benchmark` class. Here are some examples for each category:

1. **Default Category (`CATEGORY_DEFAULT` tag)**: The `TEST` benchmark is a test benchmark to quickly verify the cluster is working correctly. It is identical to the base benchmark but runs for a shorter duration.

2. **Baseline Category (`CATEGORY_BASELINE` tag)**: The `BASE` benchmark is the base benchmark to compare other benchmarks against. It is the default benchmark for all new clusters. It is used to measure the performance of the cluster without any additional load or faults.

3. **Configuration Category (`CATEGORY_CONFIGURATION` tag)**: The `NO_SWITCH` benchmark measures the performance of the cluster without a network switch. The configuration is identical to the baseline, the user is expected to rewire the cluster appropriately before running this benchmark.

4. **Fault Category (`CATEGORY_FAULT` tag)**: The `SOFTWARE_FAULT_SLAVE` benchmark measures the performance of the cluster when software faults are introduced in the slave nodes. The faults are simulated and their impact on the PTP performance is measured.

5. **Load Category (`CATEGORY_LOAD` tag)**: The `resource_contention` benchmark measures the performance of the cluster under different levels of resource contention. The resource could be CPU, network, etc. The resource is loaded to a certain percentage of its capacity, which is expected to affect the performance of the PTP applications running on the cluster.

6. **Resource Consumption Category (`CATEGORY_RESOURCE_CONSUMPTION` tag)**: The `RESOURCE_CONSUMPTION` benchmark measures the resource consumption of the PTP applications on each node. Collected metrics include CPU usage, memory usage, network traffic, and clock synchronization statistics.

7. **Scalability Category (`CATEGORY_SCALABILITY` tag)**: The `BASE_AS_SCALABILITY` benchmark measures the performance of the cluster with two nodes. The first node in the cluster is the master, the second node the primary slave. A set of scalability benchmarks can show the scalability trend. System resource consumption is monitored during the benchmark.

Each benchmark is registered in the `BenchmarkDB` using the `register` or `register_all` methods. The `all_by_tags` method can be used to retrieve all benchmarks that include certain tags.

The `Benchmark` class in the `ptp_perf/profiles/benchmark.py` file is a dataclass that represents the definition of a benchmark to run on a PTP cluster. Here's a brief description of its attributes:

- `id`: The unique identifier of the benchmark.
- `name`: The human-readable name of the benchmark.
- `description`: An explanation of the benchmark and what it measures.
- `tags`: A list of tags to categorize the benchmark.
- `version`: The version of the benchmark definition, used to track changes to the benchmark.
- `duration`: The length of the benchmark, the time to run the benchmark for.
- `num_machines`: The number of machines to use in the benchmark.
- `ptp_config`: The PTP configuration to use for the benchmark, used to create the daemon configuration file.
- `ptp_keepalive`: Whether to keep the PTP daemon alive by restarting it if it crashes or exits unexpectedly.
- `analyze_limit_permissible_clock_steps`: The maximum number of clock steps that are allowed before the benchmark is considered invalid.
- `setup_use_initial_clock_offset`: Whether to set the initial clock offset at the beginning of the benchmark.
- `artificial_load_network`: The target bandwidth to use for artificial network load benchmark in megabits per second.
- `artificial_load_network_dscp_priority`: The DSCP priority to use for the iPerf traffic in the artificial network load benchmark.
- `artificial_load_network_secondary_interface`: Whether to use a secondary network interface for artificial load in the artificial network load benchmark.
- `artificial_load_cpu`: The target CPU load to use with Stress-NG for the artificial CPU load benchmark as a percentage.
- `artificial_load_cpu_scheduler`: The CPU scheduler to use for Stress-NG in the artificial CPU load benchmark.
- `artificial_load_cpu_restrict_cores`: Whether to restrict the CPU cores used by Stress-NG in the artificial CPU load benchmark using task affinity.
- `artificial_load_aux`: Whether this is an auxiliary artificial load benchmark that uses Stress-NG, such as memory bandwidth load, cache contention, etc.
- `artificial_load_aux_options`: Options to pass to Stress-NG for this auxiliary load benchmark.
- `fault_ssh_keepalive`: Whether to keep the SSH connection from the orchestrator to the workers and the worker PTP-Perf applications alive by restarting them upon unexpected disconnects or exits.
- `fault_software`: Whether to simulate software faults during the benchmark.
- `fault_hardware`: Whether to simulate hardware faults during the benchmark.
- `fault_interval`: How frequently a fault is generated.
- `fault_duration`: How long a fault lasts.
- `fault_location`: The location of the fault, e.g. the machine to create the fault on.
- `fault_failover`: Whether to use a failover master during the fault in this benchmark.
- `monitor_resource_consumption`: Capture system resource metrics during the benchmark run.

For a list of benchmarks with descriptions of each see the **[Benchmark Overview](benchmark_overview.md)**.
For detailed information on the attributes of the `Benchmark` class, refer to the `ptp_perf/profiles/benchmark.py` file.

### Vendor

A PTP vendor in this context refers to the specific implementation of the Precision Time Protocol (PTP) that is used in the system. Different vendors may implement the protocol in slightly different ways, leading to variations in performance, features, and compatibility.

In the EtherTime project, the following PTP vendors (implementations) are supported:

1. **PTPd**: An established, if dated, implementation widely deployed due to its simplicity. More information can be found on its [GitHub page](https://github.com/ptpd/ptpd).

2. **LinuxPTP**: A robust implementation tightly integrated with Linux, leveraging kernel and hardware features. More information can be found on its [website](https://www.linuxptp.org/).

3. **SPTP**: Meta's custom protocol, claiming increased resource efficiency and resilience. More information can be found on its [GitHub page](https://github.com/facebook/time/tree/main/ptp).

4. **Chrony**: A state-of-the-art NTP server/client offering extensive features and capabilities. More information can be found on its [website](https://chrony-project.org/).

Each of these vendors provides a different implementation of the PTP, and the EtherTime project is designed to evaluate and compare their performance under various conditions.

### Cluster

A PTP (Precision Time Protocol) cluster in this context refers to a group of machines networked together, running the Precision Time Protocol. The purpose of a PTP cluster is to synchronize the clocks of all the machines in the cluster to a high degree of precision and accuracy.

The Precision Time Protocol, defined in IEEE 1588, is used to synchronize the clock of a network of machines to a master clock. This is particularly useful in systems where precise timing is critical, such as telecommunications, data centers, and various scientific and industrial applications.

In the context of the EtherTime project, a PTP cluster is used for benchmarking different PTP implementations. The cluster consists of a master machine, one or more slave machines, and optionally a failover master. The performance of the PTP implementations is tested under various conditions defined by the benchmarks, such as different levels of resource contention, different PTP configurations, and the introduction of faults.

The `Machine` class represents a machine that is part of a cluster used for benchmarking. Each machine is characterized by several attributes, such as its unique identifier (`id`), the network interface that PTP should run on (`ptp_interface`), the IP address of the machine to use with PTP (`ptp_address`), and the role of the machine in the PTP cluster (`endpoint_type`), among others.

In the context of the EtherTime project, a `Machine` instance represents a physical or virtual machine that is part of the PTP cluster being benchmarked. The `Machine` class provides a way to manage and interact with these machines programmatically, which is essential for automating the benchmarking process and analyzing the results.

### Log Record

The `LogRecord` class represents a log record captured during a Precision Time Protocol (PTP) benchmarking run. Log records are messages generated by the PTP daemon or other processes running on the machine and are used to diagnose issues with the PTP cluster, identify performance bottlenecks, and track the progress of the benchmarking run.
Each log record is characterized by several attributes, such as its unique identifier (`id`), the timestamp when the log record was created (`timestamp`), the endpoint associated with the log record (`endpoint`), and the source of the log record (`source`).

Here's a brief description of its attributes:

- `id`: The unique identifier of the log record. This is an auto-incrementing primary key.
- `timestamp`: The timestamp when the log record was created.
- `endpoint`: The `PTPEndpoint` associated with the log record. This is a foreign key that references the `PTPEndpoint` model.
- `source`: The source of the log record. This could be the PTP daemon, SSH, or other processes running on the machine.
- `message`: The actual content of the log record.

### Sample

The `Sample` class represents a sample collected during a Precision Time Protocol (PTP) benchmarking run. Samples are generated from log records and are used to calculate summary performance metrics such as clock difference and path delay for each endpoint. They can also be used to generate time series data for visualization and analysis.

Each sample is characterized by several attributes, such as its unique identifier (`id`), the endpoint associated with the sample (`endpoint`), the timestamp when the sample was collected (`timestamp`), the type of sample (`sample_type`), and the value of the sample (`value`).

Samples types include clock difference, path delay, faults, and system resource consumption metrics. The value of the sample depends on the type of sample being collected.


## License

The EtherTime dataset is distributed under the Open Data Commons Open Database License (ODbL) v1.0. The full text of the license can be found in the `LICENSE.txt` file in the root directory of the dataset.

Below is a summary of the terms of the license:

You are free:

- To share: To copy, distribute and use the database. 
- To create: To produce works from the database.
- To adapt: To modify, transform and build upon the database.

As long as you:

- Attribute: You must attribute any public use of the database, or works produced from the database, in the manner specified in the ODbL. For any use or redistribution of the database, or works produced from it, you must make clear to others the license of the database and keep intact any notices on the original database.
- Share-Alike: If you publicly use any adapted version of this database, or works produced from an adapted database, you must also offer that adapted database under the ODbL.
- Keep open: If you redistribute the database, or an adapted version of it, then you may use technological measures that restrict the work (such as DRM) as long as you also redistribute a version without such measures.
