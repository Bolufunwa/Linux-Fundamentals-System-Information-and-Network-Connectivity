# Linux Fundamentals: System Information and Network Connectivity

This project covers system information gathering, hardware and storage inspection, Linux kernel identification, and basic network connectivity testing using ping commands. The project demonstrates practical command-line skills for system administration and network troubleshooting.

## Table of Contents
- [Project Overview](#project-overview)
- [Network Topology](#network-topology)
- [Tools and Technologies](#tools-and-technologies)
- [Configuration Steps](#configuration-steps)
- [Results and Findings](#results-and-findings)
- [Author](#author)

## Project Overview

The purpose of this project is to develop practical Linux command-line skills by examining system information and testing network connectivity.

The main objectives were to:

- Identify the current username and system hostname.
- Determine the current working directory.
- Inspect system memory and available disk space.
- Identify the installed Linux kernel version.
- Test network connectivity using the `ping` command.
- Analyze packet loss and round-trip response times.
- Compare connectivity results between different destinations.

The project was completed in a Kali Linux environment on September 23, 2026.

## Network Topology

The project used a Kali Linux machine to perform basic connectivity tests against external network destinations.

### Network Layout

- **Client machine:** Kali Linux
- **Hostname:** `kali`
- **Username:** `kali`
- **External connectivity test destinations:** `8.8.8.8` and Google
- **Reported IP address for Google:** `192.178.192.100`

### System Specifications

- **RAM:** 1.9 GB
- **Available space on the main partition:** 60 GB
- **Operating system:** Kali Linux
- **Kernel version:** `Linux kali 6.19.14+kali-amd64 #1 SMP PREEMPT_DYNAMIC Kali 6.19.14-1kali1 (2026-05-05) x86_64 GNU/Linux`

### Network Connectivity Tests

The `ping` command was used to send packets to external destinations and measure connectivity.

- **Test 1:** Ping `8.8.8.8`, with an average round-trip time of 23.150 ms and 0% packet loss.
- **Test 2:** Ping Google, with a reported IP address of `192.178.192.100` and a round-trip time of 3045 ms.

The document reports different response times for the two destinations. These results illustrate how network latency can vary depending on the destination and network conditions.

## Tools and Technologies

- **Kali Linux:** Linux operating system used for the practical exercises.
- **Linux command line:** Interface for executing system inspection and network diagnostic commands.
- **`whoami`:** Used to identify the current username.
- **`hostname`:** Used to identify the machine's hostname.
- **`pwd`:** Used to display the current working directory.
- **System information commands:** Used to inspect memory, disk space, and kernel information.
- **`ping`:** Used to test network reachability and measure round-trip times.
- **Google:** External destination used for a connectivity test.
- **`8.8.8.8`:** IP address used as an external connectivity test destination.

## Configuration Steps

1. **Access the Kali Linux environment.**
   - Open a terminal in the Kali Linux system.
   - Begin the system information and network connectivity exercises.

2. **Identify the current username.**
   - Run `whoami`.
   - Confirm that the username displayed is `kali`.

3. **Identify the machine hostname.**
   - Run `hostname`.
   - Confirm that the hostname is `kali`.

4. **Check the current working directory.**
   - Run `pwd`.
   - Observe the directory displayed by the terminal.

5. **Inspect system memory and disk space.**
   - Use the system information commands to examine available memory and storage.
   - Record the reported RAM of 1.9 GB and main partition space of 60 GB.

6. **Identify the Linux kernel version.**
   - Run `uname -a`.
   - Record the reported kernel information: `Linux kali 6.19.14+kali-amd64 #1 SMP PREEMPT_DYNAMIC Kali 6.19.14-1kali1 (2026-05-05) x86_64 GNU/Linux`.

7. **Test connectivity to `8.8.8.8`.**
   - Run `ping 8.8.8.8`.
   - Observe the packet responses and round-trip times.
   - Record the average round-trip time of 23.150 ms and 0% packet loss.

8. **Test connectivity to Google.**
   - Run `ping google.com`.
   - Observe the IP address reported in the document: `192.178.192.100`.
   - Record the reported round-trip time of 3045 ms.

9. **Use a limited number of ping packets.**
   - Use the `-c` option to specify the number of packets sent.
   - For example, run `ping -c 4 8.8.8.8` to send four ping packets.
   - Review the responses and the summary showing packet loss and response times.

10. **Compare the connectivity results.**
    - Compare the recorded response times for `8.8.8.8` and Google.
    - Note the differences in latency and the packet loss reported in the test results.

## Results and Findings

The project successfully documented basic system information and performed network connectivity tests in Kali Linux.

### System Information Results

- The current username was identified as `kali`.
- The machine hostname was identified as `kali`.
- The system reported 1.9 GB of RAM.
- The available space on the main partition was reported as 60 GB.
- The Linux kernel version was recorded for system identification.

### Network Connectivity Results

- The connectivity test to `8.8.8.8` reported an average round-trip time of 23.150 ms.
- The same test reported 0% packet loss.
- The Google connectivity test reported an IP address of `192.178.192.100`.
- The document recorded a round-trip time of 3045 ms for Google, compared with 1002 ms for `8.8.8.8` in its comparison notes.
- The `-c 4` option was identified as a way to send four ping packets and obtain a summary of packet loss and response times.

### Key Findings

- Linux commands provide a straightforward way to identify system configuration details.
- The `ping` utility helps evaluate network reachability and measure response times.
- Different destinations can produce different latency measurements.
- Packet loss and round-trip time are useful indicators when investigating network connectivity.

**Note:** The source document contains different reported timing values for the connectivity tests. The figures above preserve the reported results rather than assuming they were measured under identical conditions.

## Author

**Name:** Bolarinwa Olufunwa

**Date:** September 23, 2026

