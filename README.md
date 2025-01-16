# Solokey Config

A [solokey](https://solokeys.com) is an open-source security key that supports FIDO2. The solokeys represent a passwordless future on the internet where authenticating is user-friendly and secure - two things that are usually mutually exclusive.

![Sad Spongebob](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExdHdpbG8zd25lcDBnYnl3ODFlazF3aGJxdXF4ODhkMjJoMjY1cmxiMyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/ISOckXUybVfQ4/giphy.gif)

Unfortunatly, the keys come out-of-the-box without multi-factore authentication - there is not pin or extra step of authenticating yourself apart from actually having the key on your person which means that if anyone can physically grab the key from you **and** knows which accounts are linked to it [the solokkey], then they can authenticate as you with little effort.

The purpose of this repo is to help users to configure their solokeys with a basic set of security features:

- updating your key
- setting a pin

## Installation

There are two solokey cli tools that you can use, [solo1 cli](https://pypi.org/project/solo1/) and [solo2 cli](https://github.com/solokeys/solo2-cli), depending on the solokey that you have. 

The `solo1` cli is built in python and the `solo2` cli is built in rust which means that you may need to setup the following environments:

- [install python3](https://www.python.org/downloads/) for `solo1`
- [install rust](https://www.rust-lang.org/tools/install) for `solo2`

```bash
# setup solo1 key
python3 -m pip install -r requirements.txt

# setup solo2 key
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
