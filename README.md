# spack-externals
Storage for `package.yaml` files for various systems.

# How to use
  1. If you are on a cluster (not your personal machine):
     1. Create a `~/.profile` file if does not exist already
     1. Add the line `export SPACK_USER_CONFIG_PATH=$HOME/.spack/$CLUSTER`. This tells Spack to look for `package.yaml` files in `~/.spack/[system_name]`
  1. Navigate to `~/.spack/[system_name]/packages.yaml`. (Possible system names: tuolumne, tioga, hopper, dane) If the `packages.yaml` file does not exist, create the file.
  1. Copy the contents of the appropriate `packages.yaml` file in this repository into the `packages.yaml` on the system you are using.
  1. Use Spack normally. Spack will now find packages already installed on the system and prefer those over installing duplicate libraries.
