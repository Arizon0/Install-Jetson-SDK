Jetson SDK Installation:

A Desktop with Ubuntu installed is required to download the Nvidia SDK and its other files for installation on the Jetson
https://developer.nvidia.com/sdk-manager

After installing the SDK Manager on the Desktop, connect the Jetson via USB-C cable (Front) to the Desktop and start it in format mode (By clicking the Power and Force Restart Buttons (Power and Middle Buttons) at the same time)

After that, the SDK Manager software on the Desktop will recognize the Jeton model.
Just below select to install the desired version, confirm and NEXT Step!
Accept the terms and click install.

ATTENTION!!
There is a high chance that even if you select to install Jetson Tools and CUDA in Step 2 they will not be installed, the link below may help!
https://docs.nvidia.com/sdk-manager/install-with-sdkm-jetson/index.html

If CUDA is still not successfully installed, 

I recommend formatting again and installing the SDK on the Jetson without any additional components!
and Install after it starts, manually with the command:

$ sudo apt update 
$ sudo apt upgrade
$ sudo apt install nvidia-jetpack

After finishing the installation, check the installed version:
$ sudo apt show nvidia-jetpack
