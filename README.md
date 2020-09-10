# configure-raspberry-pi

Script to automatically configure a Raspberry Pi boot volume

![Screen recording of configure-raspberry-pi in action](preview.gif)

## Functionality

The following options can be configured:

- WiFi
- SSH

This initial functionality comes from a personal need; I expect to add more over time, and willingly accept pull requests.

## Installation

Simply clone the repository:

```bash
git clone git@github.com:jbmorley/configure-raspberry-pi.git
```

You can optionally add it to the path for convenience:

```bash
export PATH=$PATH:~/path/to/configure-raspberry-pi
```

## Usage

Run the following command, and answer the various commands:

```bash
configure-rasbperry-pi
```

The script currently expects to be run on macOS and assumes your Raspberry Pi `boot` partition will be mounted at `/Volumes/boot`. If you're using a different location, or operating system, you can specify this by passing the `--root` flag. For example,

```bash
configure-raspberry-pi --boot /mnt/boot
```

