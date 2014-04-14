To deploy the root file system, you are going to need a micro SD card.

1. Copy the root file system to your SD card

.. host::

 | sudo dd if=~/architech_sdk/architech/@board-alias@/yocto/tmp/deploy/images/@quickstart-image@-@machine-name@.sdcard of=/path/to/your/sd/card/device

.. warning::

 Be very careful when you use *dd* to write to a device to pick up the right device, otherwise you can mess up another disk you have on your machine, destroying its content forever!

.. warning::
 
 The content of the SD card will be lost forever!

.. important::

 Be sure you **unmount the device** from the filesystem before using **dd** program, you sure don't want to have the operating system interfere during the write process.

2. After *dd* completes, make sure everything has been really written to the SD card:

.. host::

 | sync

3. Unmount the micro SD card from your computer

4. Plug the micro SD in the board socket.

