# wsl-kernel
![kernel-build](https://github.com/devbens/wsl-kernel/actions/workflows/build.yml/badge.svg)

This adds USB (usbip) and USB-CAN support to WSL2 Kernel.

+ Download one of the [Kernels](https://github.com/devbens/wsl-kernel/actions) (click the latest workflow run)
+ Create a `.wslconfig` file on `/mnt/c/Users/<user>/` and add a reference to the created image with the following.[^1]
    ```ini
    [wsl2]
    kernel=c:\\users\\<user>\\linux-msft-wsl-5.10.y-usbip-can
    ```

[^1]: [usbipd-win](https://github.com/dorssel/usbipd-win)
