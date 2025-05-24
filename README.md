# Task 7: Monitor System Resources Using Netdata

## Objective:
Install and run Netdata via Docker to monitor system resources such as CPU, memory, disk usage, and Docker containers.

## Steps Followed:

1. Pulled and ran the Netdata Docker image:
   ```bash
   docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
