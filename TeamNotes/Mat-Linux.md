SW process - Matt suggestions on linux

# Linux? Should we use it??

This is a complex topic, so I'll try to break it down.

Terms:
Distro/Distribution: A version of Linux in the form of an operating system 
DX: Developer Experience

## Why we might

### Stability

Many distros can guarantee stability. Windows is volatile in a sense, because you never know if/when an update will be needed/forcefully installed. Updates can break things, so a distro that stays at a stable environment is perfect for keeping flow going and stopping distractions

Distro Possibilities: NixOS (Flakes), Debian, Ubuntu, Linux Mint

### Freedom

Linux is "Free as in free samples, and free as in freedom" which means that it can be used for almost anything. It can't be revoked, or taken away.  

### Lightweight

Linux can be extremely lightweight in terms of system resources, meaning older computers might still be able to be transformed into fully functional Dev Machines

### Reproducible

This is mostly just a shill for NixOS, but we can make Dev Machines have the exact software/version. This could also be possible using Home Manager (based on Nix) to make a reproducible environment on any Linux Distro.

## Why we might not

### Different UI -> Different DX

Devs like Leo have strongly opposed Linux. Presumably due to it being different from Windows.

### Software Compatibility

I'm not too worried about this, seeing as a lot of software already works. The only thing that doesn't work (afaik) is the NI Driver Station. This means that we'd probably need at least two computers to be driver stations. I digress just something to keep in mind.

### District Approval?

Not sure if Linux would be approved by the district. Maybe it would, maybe it wouldn't.


## Software Support

### Git

100% Works. Git was made specifically to track changes made to Linux, so it definitely works

### Elastic Dashboard

It does run. I haven't tested it out on the robot, but we can at least make changes to the layouts.

### Pathplanner

It works really well. I will note on my NixOS machine, it does not want to build when put in my packages list, however it does work when using `nix run` so ymmv.

### NI Driver Station

Unfortunately, this is the one thing that doesn't work on Linux. I think there are Third Party Driver Stations, but these are not able to be used in comps

### VSCode

It works perfectly fine. No notes.

### WPILib Extension

WPILib actually has really great support on Linux. Since VSCode is on Linux, they can use the WPILib Extension the same.
Show less
