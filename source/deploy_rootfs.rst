To deploy the root file system, you are going to need a micro SD card.

1. Copy the root file system to your SD card

.. host::

 sudo dd if=~/architech_sdk/architech/@board-alias@/yocto/tmp/deploy/images/@quickstart-image@-@machine-name@.sdcard of=/your/sd/card/device

.. warning::

 Be very careful when you use **dd** to write to a device to pick up the right device, otherwise you can mess up another disk you have on your machine, destroying its content forever!

2. Unmount the micro SD card from your computer

3. Plug the micro SD in the board socket.

