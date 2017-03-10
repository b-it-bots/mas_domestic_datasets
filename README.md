## Git Large File Storage (LFS)
This repository has git LFS enabled for .pcd files (specified in [.gitattributes](./.gitattributes)
).

By default, cloning the respository will only fetch the .pcd files in `generic/mds_pointclouds/objects/workspace_setups/objects_laying`. This is specified by `fetchinclude` in [.lfsconfig](.lfsconfig).

You will have to install git-lfs to use lfs commands. (See [here](https://github.com/git-lfs/git-lfs/wiki/Installation))

Clone repository and fetch only paths specified in `fetchinclude`:

     git clone gitgate@mas.b-it-center.de:mas-group/mas_datasets.git

Fetch all LFS objects:

     git lfs fetch --all
