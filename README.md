A set of [tinted-theming](https://github.com/tinted-theming/home) (base16) templates for the TUI file manager [Yazi](https://github.com/sxyazi/yazi). It generates yazi's [flavors](https://yazi-rs.github.io/docs/flavors/overview/) from base16 schemes.

## Usage

You can manually copy a theme file into your yazi's `theme.toml` file, or into a flavor directory.

### With Tinty

For convenient, we recommend using [tinty](https://github.com/tinted-theming/tinty). An example config is 

```toml
[[items]]
path = "https://github.com/tinted-theming/tinted-yazi"
name = "tinted-yazi"
themes-dir = "flavors"
hook = '''
cp -f "$TINTY_THEME_FILE_PATH" "$HOME/.config/yazi/flavors/tinted-scheme.yazi/flavor.toml"
'''
```

in your tinty's `config.toml` file. Then put

```toml
[flavor]
dark = "tinted-scheme"
```

in your `theme.toml`.

