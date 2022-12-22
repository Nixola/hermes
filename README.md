Hermes
======

Quickly send messages to a configured Telegram chat on the command line.

Installation
------------

### Cargo

```bash
$ cargo install --git=https://github.com/darkwater/hermes
```

### Nix Flake

```bash
$ nix profile install github:darkwater/hermes
```

Or, to try it out without installing:

```bash
$ export HERMES_TOKEN="..."
$ export HERMES_CHAT_ID="..."
$ nix run github:darkwater/hermes send "Hello, world!"
```

Configuration
-------------

While in early development, this readme will probably not be complete. See
`src/config.rs` for the full list of configuration options, and the exact
mechanism for loading them.

Put a `config.toml` in a config directory such as `~/.config/hermes/` or
`/etc/hermes/` with the following contents:

```toml
token = "1234567890:AAHpq9Lj5jGR2PXpbH5KG6RBrYp4WJaYJo5"
chat_id = 63987654
```

Usage
-----

```bash
$ hermes send "Hello, world!"
```
