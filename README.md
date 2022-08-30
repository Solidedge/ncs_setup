# My NCS setup
This repository is an outline of my nRF Connect SDK setup (NCS), and is setup in conjunction with my [NCS project template](https://github.com/Solidedge/ncs_project_template).

# Installing
Make sure you have the toolpath for nRF connect SDK installed on your computer. This can be done via the nRF connect Toolchain manager. Go to your desired folder, I prefer a folder named "ncs", and run the following command:

```
git clone https://github.com/Solidedge/ncs_setup .
```
Note that the folder must be empty!

Adjust my_projects/west.yml to satisfy your needs, before you follow up by updating west:
```
west update
```
If the ncs_project_template and ncs_setup is succesfully downloaded, comment out or remove the mention of this repo in the west.yml file found in the my_projects folder:
```
    # Project Templates, remove before running west build to avoid troubles:
    #- name: ncs_project_template
    #  path: my_projects/ncs_project_template
    #  url: https://github.com/Solidedge/ncs_project_template
    #  revision: main
```

## NCS Directory
```
ncs (the folder you should run the clone in)
├── .west
│   └── config
├── bootloader/...
├── mbedtls/...
├── modules/...
|
├── my_projects
│   ├── ncs_project_template/...
│   ├── ncs_project_01/...
│   ├── ncs_project_02/...
│   ├── ncs_project_03/...
│   ├── ...
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
