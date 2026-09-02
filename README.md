# NVIDIA GPU Monitor

A lightweight desktop GPU monitor for NVIDIA GPUs.

Designed for:
- LLM inference and benchmarking
- AI / ML development
- GPU-intensive workloads
- Gaming monitoring
- General GPU monitoring

![NVIDIA GPU Monitor](screenshot.png)

## Overview

It provides a real-time view of GPU resources and is particularly useful for:
- LLM inference testing and development
- GPU benchmarking
- monitoring resource consumption during workloads

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


## LLM benchmarking

GPU Monitor is designed to help monitor GPU resource consumption during
LLM inference and other GPU-intensive workloads.

The session function makes it possible to isolate a workload and observe
its resource consumption over a defined period.

This can be useful when comparing models, configurations, quantization
levels or inference parameters.

## Gaming

GPU Monitor can also be used to monitor GPU usage and power consumption
during gaming sessions.

For example, it can help answer a simple question:

> How much GPU power does my game actually consume during a six-hour
> gaming session?


## Requirements

### Current platform

The current release is available for:

- Linux x86-64

Windows support is planned for a future release.


## Installation

The current release does not require a traditional installation.

Just download the release archive, extract it and run:

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

Note :
The NVIDIA driver, NVML and Qt are not bundled with GPU Monitor
and must be provided by the target system.


## Desktop integration

The application icon is provided separately and can be used for desktop
integration.

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
