# Troubleshooting

This guide is for troubleshooting software on Linux platforms.

## Fail to launch the software


* You might see `dlopen(): error loading libfuse.so.2` where some distros does not have `fuse` library by default, try manually install `libfuse2` by using the following command

    ```
        sudo apt install libfuse2
    ```

    **_NOTE:_** Do not by any chance remove or purge fuse library which comes with the system. Many immportant packages depends on it, so you may end up completely crash your system.
