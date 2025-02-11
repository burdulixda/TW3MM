# The Witcher 3 Mod Manager

Mod Manager for The Witcher 3.

Supports the Steam and GOG releases on Windows and the Steam Proton release on Linux.

## Description

The Witcher 3 Mod Manager is an application that simplifies installing and managing The Witcher 3 mods, originally developed by [stefan3372](https://github.com/stefan3372) and now being continued here.

See the [Nexus Mods page](https://www.nexusmods.com/witcher3/mods/2678) for releases, screenshots and more information.

## Usage

### Release Versions (Windows)

Download and unpack the latest release from Nexus Mods or from the GitHub releases. If you are upgrading from version 0.6 or later, directly overwrite the previous installation. Existing configuration files wll be searched in the same directory as the executable first, in `Documents\The Witcher 3 Mod Manager` second.

On the first run, if no configuration can be found, configuration files will be created under `Documents\The Witcher 3 Mod Manager`. They can be freely relocated between the two searched locations as preferred.

### Python (Windows and Linux)

Download the source and install the requirements with `pipenv install --python 3.10`. `pipenv` and either Python 3.10 or `pyenv` have to be installed. Afterwards run with `pipenv run python main.py`.

On Linux, the configuration files will be created in `~/.config/TheWitcher3ModManager`, and `wine` has to be available to run Script Merger.

### Build Release (Windows)

Download the source and install the requirements with `pipenv install --python 3.10 --dev`. `pipenv` and either Python 3.10 or `pyenv` have to be installed. Afterwards run with `pipenv run python setup.py build_exe`.

> [!NOTE]
> `pyenv-win` might not work with `pipenv` out of the box. Either install Python 3.10 manually, or [use `pyenv-win` to install Python 3.10 first](https://github.com/pyenv-win/pyenv-win#quick-start) and [specify its path.](https://github.com/pypa/pipenv/issues/4508#issuecomment-718987911)

The files will be created in `build/exe.[platform identifier].[python version]`.
