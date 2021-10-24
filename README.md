[![C/C++ CI](https://github.com/nimbus9inc/ZiGate/actions/workflows/jn5168-coordinator.yml/badge.svg)](https://github.com/nimbus9inc/ZiGate/actions/workflows/jn5168-coordinator.yml)

# ZiGate

ZiGate Gateway Repository


# ModuleRadio

Contains source code and build configurations for compiling coordinator firmware to NXP's
JN516x series chips. The JN5168 chip is the primary focus of this fork.

## Building

This repository utilizes [GitHub Actions](https://docs.github.com/en/actions) for builds on each
commit. Thus, by far the easiest way to build the radio firmware for this project is to utilize
[Act](https://github.com/nektos/act), which is a local GitHub Actions runner which runs the same
configuration found in the `.github` folder in a local Docker container. If you have Docker
installed, you can simply run:

```shell
act -v
```

The `-v` flag mounts this repository into the Docker container, with the result that all build
artifacts can be found in `./ModuleRadio/Firmware/src/ZiGate/Build/ZigbeeNodeControlBridge/` upon
successful build.

# ModuleWiFi
