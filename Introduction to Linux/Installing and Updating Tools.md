# Installing and Updating Tools
## Package Manager
For Kali, this is `apt` but this could be different for other distros (e.g. Fedora uses `dnf`)  

`apt update && apt upgrade` - Update and upgrade your installed software and OS  

You can install specific packages with the package manager, e.g.:
`apt install python-pip`

You can also search for a package, e.g.:
`apt search golang`


## GitHub
`git clone` - this will download a specific repo from GitHub to your current directory, provided with the GitHub URL for the code

It is recommended you install new applications in the `/opt` directory

**Note:** It is recommended you download and run a script called `pimpmykali` from GitHub to fix a few issues with standard Kali installations.