# Polymath

Polymath is a web server designed to host resource packs of the Oraxen plugin.

## How to use Polymath

- Clone the project
``git clone git@github.com:oraxen/Polymath`` or ``git clone https://github.com/oraxen/Polymath``

- Cd in the directory
``cd ./Polymath``

- Install nix
Follow this tutorial (you only need nix, not nixos): https://nixos.org/download.html
On linux this is just this command:
``sh <(curl -L https://nixos.org/nix/install) --daemon``
On macos:
``sh <(curl -L https://nixos.org/nix/install)``
You can check the website to get it working on windows or docker.

- Install the required libs
If you installed nix, just type:
``nix-shell``
If you didn't install nix, you need to install Python 3.8 with those packages:
```
cython
aiohttp
toml
```

- Build polymath
```sh
./build.sh
```

- Run a first time
``sh
./run``

- Configure the file ``polymath/config/settings.toml``

- Run a second time
``sh
./run``

- Polymath should now be running

## Pterodactyl
This fork also has an egg for Pterodactyl so you can use it with a Pterodactyl instance.

You can find this egg at [egg-poly-math.json](https://github.com/PlasHost/polymath/blob/master/egg-poly-math.json)
