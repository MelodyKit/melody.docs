# Config

MelodyKit configuration file is located at `~/.config/melody/kit.toml`.

The default config can be found [here][config].

## `melody`

`melody` is the root table for all configurations.

It contains several fields:

- `name`, the *name* of the platform; used when sending emails and in API documentation.
- `domain`, the *domain* where MelodyKit is hosted.
- `open`, the *subdomain* where MelodyKit application is hosted.
  An *open* URL looks like `https://{config.open}.{config.domain}/`.
- `images`, the *path* to the *images* directory; playlist covers and profile images are stored there.

Example configuration:

```toml
[melody]
name = "MelodyKit"
domain = "melodykit.app"
open = "open"

images = "~/.melody/kit/images"
```

[config]: https://github.com/MelodyKit/melody.web/blob/main/melody/kit.toml
