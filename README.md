# Solokey Config

Shortcuts:

- [solo1 cli](https://pypi.org/project/solo1/) (you'll need [fido2](https://pypi.org/project/fido2/0.9.3/) for setting a key pin)
- [solo2 cli](https://github.com/solokeys/solo2-cli)

## Getting Started

Depending on the cli you're using, you'll need to install the appropriate package.

### Solo1

Pre-requisites:

- [install python3](https://www.python.org/downloads/)

```bash
python3 -m pip install -r requirements.txt
```

### Solo2

Pre-requisites:

- [install rust](https://www.rust-lang.org/tools/install)

```bash
cargo install solo2
```

## Usage

This section will cover the basic usage of the solokey cli for both solo1 and solo2.

Updating your key:

```bash
# Solo1 cli
solo1 key update

# Solo2 cli
solo2 update
```

Setting a key pin (*solo1 cli also works for solo2*):

```bash
# Solo1 cli
solo1 key set-pin
```
