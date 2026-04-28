# FM Modular

FM Modular nasceu da refatoracao dos seus temas antigos, principalmente `FM/Niku`, para uma base reutilizavel de temas de Discord. A proposta e simples: parar de repetir um arquivo gigante e passar a montar temas por composicao.

## Mapeamento do estilo FM

O bloco original do tema foi quebrado nestas partes:

- `background`
- `variables`
- `discord-vars`
- `layout-glass`
- `server-list`
- `channels`
- `messages`
- `input-area`
- `popouts`
- `profiles`
- `emoji-picker`
- `buttons`
- `animations`
- `scrollbars`
- `badges`
- `forum`
- `codeblocks`
- `tooltips`
- `watermark`
- `fixes`
- `overrides`

## Estrutura

```text
FM-Modular/
  core/
  modules/
  plugins/
  animations/
  palettes/
  presets/
  features.css
  performance-mode.css
  builder.theme.css
  overrides.css
  LICENSE.md
```

## Paletas

- `preto.css`
- `purple.css`
- `strawberry.css`
- `blue.css`
- `red.css`
- `cyberpunk.css`
- `dark-minimal.css`

## Presets

- `trojan-purple.theme.css`
- `niku-strawberry.theme.css`
- `chill-glass.theme.css`
- `cyberpunk.theme.css`
- `dark-clean.theme.css`
- `preto.theme.css`

## Como montar um tema

Ordem recomendada:

1. `core/variables.css`
2. `features.css`
3. uma paleta
4. um preset de animacao
5. `core/reset.css`
6. `core/discord-vars.css`
7. `core/background.css`
8. `core/layout-glass.css`
9. modulos
10. plugins opcionais
11. `performance-mode.css`, se quiser
12. `overrides.css`

## Feature flags

`features.css` controla:

- `--fm-enable-glow`
- `--fm-enable-animations`
- `--fm-enable-blur`
- `--fm-enable-transparency`

## Plugins

- `animated-glow.css`
- `neon-cursor.css`
- `custom-logo.css`
- `animated-background.css`
- `hover-effects.css`
- `typing-effects.css`
- `ripple-click.css`
- `parallax.css`

## Custom logo

`custom-logo.css` usa:

- `--fm-logo-url`
- `--fm-logo-hover-url`
- `--fm-logo-size`
- `--fm-logo-glow`

## Presets de animacao

- `smooth.css`
- `fast.css`
- `dramatic.css`
- `minimal.css`

## Builder

`builder.theme.css` serve como ponto de montagem rapida. Ele ja traz a ordem certa de imports e deixa plugins opcionais comentados.

## Exemplos de combinacao

Cyberpunk:

- `palettes/cyberpunk.css`
- `animations/fast.css`
- `plugins/animated-glow.css`
- `plugins/neon-cursor.css`

Clean:

- `palettes/dark-minimal.css`
- `animations/minimal.css`

Preto:

- `palettes/preto.css`
- `animations/minimal.css`

Niku:

- `palettes/strawberry.css`
- `animations/smooth.css`

## Nota

`overrides.css` deve ficar sempre por ultimo.
