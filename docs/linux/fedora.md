# Install the GStreamer binarie builds

In order to install the SDK on Fedora, it is required that the public repository where the SDK resides is added to the yum sources list.

To do so, download the appropriate definition file for your distribution:

Fedora 17
Fedora 18
And copy it to the /etc/yum.repos.d/ directory on your system:

``` bash
su -c 'cp gstreamer-sdk.repo /etc/yum.repos.d/'
```

After adding the repositories, the yum repository list needs to be refreshed. This can be done by running:

``` bash
su -c 'yum update'
```

Now that the new repositories are available, install the SDK with the following command:

``` bash
su -c 'yum install gstreamer-sdk-devel' # Enter the superuser/root password when prompted.
```
