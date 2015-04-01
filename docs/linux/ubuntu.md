# Install the GStreamer binarie builds

In order to install the SDK on Ubuntu, it is required that the public repository where the SDK resides is added to the apt sources list.

Ubuntu Precise Pangolin (12.04) i386 amd64
Ubuntu Quantal Quetzal (12.10) i386 amd64
Ubuntu Raring Ringtail (13.04) i386 amd64


``` bash
$ sudo cp gstreamer-sdk.list /etc/apt/sources.list.d/
```

And copy it to the /etc/apt/sources.list.d/ directory on your system:


``` bash
$ wget -q -O - http://www.freedesktop.org/software/gstreamer-sdk/sdk.gpg | sudo apt-key add -
$ sudo apt-get update
```

After adding the repositories, the GPG key of the apt repository has to be added and the apt repository list needs to be refreshed. This can be done by running:


``` bash
$ sudo apt-get install gstreamer-sdk-dev # Enter the superuser/root password when prompted.
```

Now that the new repositories are available, install the SDK with the following command:
