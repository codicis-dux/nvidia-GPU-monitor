# NVIDIA GPU Monitor

Lightweight NVIDIA GPU monitor for LLM benchmarking, development, gaming and
general GPU monitoring.

![GPU Monitor](screenshot.png)

## Overview

GPU Monitor is a lightweight graphical monitoring tool for NVIDIA GPUs.

It provides a real-time view of GPU resources while running applications
or workloads, with a particular focus on LLM inference, development and
benchmarking.

It can also be used for general GPU monitoring, including gaming.

## Features

- Real-time GPU monitoring
- GPU utilization
- GPU memory / VRAM usage
- GPU power consumption
- GPU temperature
- Session monitoring
- Session reset
- Support for NVIDIA GPUs
- Lightweight graphical application

The information available depends on the NVIDIA GPU and the capabilities
provided by the installed NVIDIA driver.

## LLM benchmarking and development

GPU Monitor is designed to be useful when developing and testing
GPU-accelerated applications and Large Language Models (LLMs).

The session function allows a workload to be monitored as a distinct
measurement period.

A typical workflow is:

1. Start GPU Monitor.
2. Start or reset a session.
3. Run the LLM inference or other workload.
4. Monitor GPU resource consumption during the workload.
5. Stop or reset the session when the measurement is complete.

This can be useful when comparing models, configurations, quantization
levels or other inference parameters.

GPU Monitor is a monitoring tool and is not intended to replace dedicated
profiling or benchmarking software.

## Gaming

GPU Monitor can also be used for general GPU monitoring while gaming.

For example, it can help monitor GPU resource consumption during a gaming
session and observe power usage over an extended period.

## Requirements

### Current platform

The current release is available for:

- Linux x86-64

Windows support is planned for a future release.

### NVIDIA GPU and driver

An NVIDIA GPU with a compatible NVIDIA driver is required.

GPU Monitor uses the NVIDIA Management Library (NVML) to obtain GPU
information.

The NVIDIA driver and NVML are not bundled with GPU Monitor.

### Qt

GPU Monitor uses Qt 6 for its graphical user interface.

Qt is not bundled with GPU Monitor and must be provided by the target
system.

## Installation

The current release does not require a traditional installation.

Download the release archive, extract it and run:

```bash
./GPUMonitor
```

If necessary, make the executable file executable:

chmod +x GPUMonitor

Then:

./GPUMonitor

A dedicated installation procedure may be provided in a future release.

Desktop integration
The application icon is provided separately from the executable.

It can be used for desktop integration and by a future installation
procedure.

Size
The Linux release executable is under 200 KB in its compressed form for
release 1.0.0.

System libraries and third-party runtime components are not bundled with
the application.

NVIDIA Management Library (NVML)
GPU Monitor uses NVIDIA's NVIDIA Management Library (NVML) to retrieve
GPU information.

NVML is provided as part of the NVIDIA driver environment.

GPU Monitor does not distribute the NVIDIA driver or NVML library.

Third-party software
GPU Monitor uses Qt 6 under the GNU Lesser General Public License
version 3 (LGPLv3).

Qt is not bundled with GPU Monitor and must be provided by the target
system.

The LGPLv3 license text is provided in:

tiers_licenses/LGPL-3.0.txt

Third-party license information is kept separate from the GPU Monitor
license.

License
Copyright © 2026 [YOUR NAME]

GPU Monitor is proprietary software.

GPU Monitor is provided free of charge for personal and commercial use.

The software is provided "as is", without warranty of any kind.

See LICENSE for the complete terms.

Source code
The source code is not currently included in the public release.

Release
v1.0.0
Initial public release.

Platform: Linux x86-64

Known limitations
Linux x86-64 only
NVIDIA GPU required
Compatible NVIDIA driver required
Qt 6 must be available on the target system
Windows version not yet available
Reported GPU information depends on the installed NVIDIA driver and NVML
Roadmap
Possible future improvements include:

Windows support
simplified installation
Linux desktop integration
automatic dependency checking
additional GPU statistics
improved session analysis
additional benchmarking-oriented measurements
possible removal of the Qt dependency in a future Linux version
The roadmap is subject to change.

Bug reports and feedback
Bug reports, suggestions and feature requests are welcome.

When reporting a problem, please provide:

Linux distribution and version
desktop environment
NVIDIA GPU model
NVIDIA driver version
Qt version
error messages, if any
steps required to reproduce the problem
