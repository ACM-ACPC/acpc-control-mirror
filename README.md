# acpc-control-mirror
# Introduction
ACPC system installation based on installing a fresh copy of the OS followed by installing the required IDE, Debuggers, Judging s/w, and other administrative environment. Installing any package needs a configured mirror for downloading the package and its dependencies. The default mirror location is the Internet mirror. Installing simultaneous devices in the same time requires a stable and huge internet bandwidth specially at the required packages installation. Internet access also is not allowed in the contest hall at any time. A local mirror required to speed up the installation process. Creating a local mirror needs a storage, and a syncing process from Internet mirror to the local mirror.

# Why using mirror
As mentioned, eliminates the need for a huge internet bandwidth, and speed up the installation, and update processes.

# What about mirror updates
Also, there is a script to update the local mirror to contains tha newly added packages, remove obsolete one, and update the existing pakcages if any.

# Prerequisites
  1. Ubuntu box
  2. Sufficient space to hold the mirror
  3. python v.3 
  4. ansible
  5. Internet connection
  6. Downloading privileges.

# How does it work?
The mirror sync is a process of cloning the internet ubuntu mirror to a local storage, which will be typically the ACPC Control Server. By default, it syncs the mirror for the ACPC Control server architecture. If you want to download the mirror for different architecture(s) you have to mention that in the configuration file ansible.cfg

# What is included and what is not included?
The local mirror includes main, restricted, and universe sections of Ubuntu. Does not include security updates, and sources.
