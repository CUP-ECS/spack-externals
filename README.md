# spack-externals
Storage for `package.yaml` files for various systems.

# How to use
  1. Navigate to `~/.spack/[system_name]/packages.yaml`. (Possible system names: tuolumne, tioga, hopper, dane) If the `packages.yaml` file does not exist, create the file.
  2. Copy the contents of the appropriate `packages.yaml` file in this repository into the `packages.yaml` on your system.
  3. Use Spack normally. Spack will now find packages already installed on the system and prefer those over installing duplicate libraries.
