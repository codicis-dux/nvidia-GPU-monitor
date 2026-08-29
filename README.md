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

```bash
chmod +x GPUMonitor
```

Then:

```bash
./GPUMonitor
```

## Desktop integration

The application icon is provided separately and can be used for desktop
integration.

## Size

The Linux release executable is under 200 KB in its compressed form for
release 1.0.0.

## Third-party software

GPU Monitor uses Qt 6 under the GNU Lesser General Public License v3.

Qt is not bundled with GPU Monitor and must be provided by the target
system.

The LGPLv3 license text is provided in
`tiers_licenses/LGPL-3.0.txt`.

## License

Copyright © 2026 

GPU Monitor is proprietary software and is provided free of charge for
personal and commercial use.

The software is provided "as is", without warranty of any kind.

See `LICENSE` for the complete terms.


## Release

**v1.0.0 — Linux x86-64**

Initial public release.

## Known limitations

- Linux x86-64 only
- NVIDIA GPU and compatible driver required
- Qt 6 must be available on the target system
- Windows version not yet available

## Roadmap

- Windows support
- Simplified installation
- Linux desktop integration
- Additional GPU statistics and session analysis

## Bug reports and feedback

Bug reports, suggestions and feature requests are welcome.

When reporting a problem, please provide your Linux distribution,
NVIDIA GPU model, NVIDIA driver version and relevant error messages.
