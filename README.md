# My NCS setup
This repository is an outline of my nRF Connect SDK setup (NCS).

# Installing
Make sure you have the toolpath for nRF connect SDK installed on your computer. This can be done via the nRF connect Toolchain manager. Go to your desired folder and run the following command:

```
git clone https://github.com/Solidedge/ncs_setup .
```
Note that the folder must be empty!

Adjust my_projects/west.yml to satisfy your needs, before you follow up by updating west:
```
west update
```


## NCS Directory
```
ncs
├── .west
│   └── config
├── bootloader/...
├── mbedtls/...
├── modules/...
|
├── my_projects
│   ├── ncs_project_template
│   │   ├── applications
│   │   │   └── app_template
│   │   │   │   ├── include/...
│   │   │   │   ├── src
│   │   │   │   │   └── main.c
│   │   │   │   ├── CMakeLists.txt
│   │   │   │   ├── dts.overlay
│   │   │   │   ├── Kconfig
│   │   │   │   ├── prj.conf
│   │   │   │   └── README.md
│   │   ├── drivers/...
│   │   ├── include/...
│   │   ├── zephyr/...
│   │   ├── CMakeLists.txt
│   │   ├── Kconfig.prjtemp
│   │   ├── README.md
│   │   └── west.yml
│   ├── .gitignore
│   └── west.yml
|
├── nrf/...
├── nrfxlib/...
├── test/...
├── tools/...
├── zephyr/...
├── .gitignore
└── README.md (the one you're reading)
```
