<h3 align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
	Catppuccin for <a href="https://github.com/abenz1267/walker">Walker</a>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
	<a href="https://github.com/catppuccin/template/stargazers"><img src="https://img.shields.io/github/stars/catppuccin/template?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
	<a href="https://github.com/catppuccin/template/issues"><img src="https://img.shields.io/github/issues/catppuccin/template?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
	<a href="https://github.com/catppuccin/template/contributors"><img src="https://img.shields.io/github/contributors/catppuccin/template?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
</p>

<p align="center">
	<img src="https://raw.githubusercontent.com/Krymancer/walker/refs/heads/main/assets/preview.webp"/>
</p>

## Previews

<details>
<summary>🌻 Latte</summary>
<img src="https://raw.githubusercontent.com/Krymancer/walker/refs/heads/main/assets/latte.webp"/>
</details>
<details>
<summary>🪴 Frappé</summary>
<img src="https://raw.githubusercontent.com/Krymancer/walker/refs/heads/main/assets/frappe.webp"/>
</details>
<details>
<summary>🌺 Macchiato</summary>
<img src="https://raw.githubusercontent.com/Krymancer/walker/refs/heads/main/assets/macchiato.webp"/>
</details>
<details>
<summary>🌿 Mocha</summary>
<img src="https://raw.githubusercontent.com/Krymancer/walker/refs/heads/main/assets/mocha.webp"/>
</details>

## Usage

### Manual

1. Copy the `catppuccin-{flavor}` directory to `~/.config/walker/themes/`.
2. Set `theme = "catppuccin-{flavor}"` in `~/.config/walker/config.toml`.

Example for Mocha:
```sh
cp -r themes/catppuccin-mocha ~/.config/walker/themes/
```
```toml
# ~/.config/walker/config.toml
theme = "catppuccin-mocha"
```

### Home Manager (NixOS)

```nix
programs.walker = {
  enable = true;
  config.theme = "catppuccin-mocha";
  themes."catppuccin-mocha" = {
    style = builtins.readFile ./themes/catppuccin-mocha/style.css;
  };
};
```

> **Note:** The old `.css` + `.toml` flat-file format is no longer supported as of walker's theme system rewrite.
> Themes now live in a directory under `~/.config/walker/themes/{name}/style.css`.

## 💝 Thanks to

- [Krymancer](https://github.com/Krymancer)

&nbsp;

<p align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/footers/gray0_ctp_on_line.svg?sanitize=true" />
</p>

<p align="center">
	Copyright &copy; 2021-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>
</p>

<p align="center">
	<a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=363a4f&colorB=b7bdf8"/></a>
</p>
