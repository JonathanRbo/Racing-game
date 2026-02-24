# Racing-game 3D — Jogo de Corrida

Jogo de corrida 3D rodando no browser, renderizado via Three.js sem nenhum motor de jogo externo.

## Como jogar

| Tecla | Ação |
|---|---|
| `W` / `↑` | Acelerar |
| `S` / `↓` | Frear / Ré |
| `A` / `←` | Virar esquerda |
| `D` / `→` | Virar direita |
| `Space` | Freio de mão |
| `C` | Trocar câmera |
| `R` | Resetar posição |

## Tecnologias

| Recurso | Detalhe |
|---|---|
| Renderização 3D | Three.js r128 |
| Linguagem | JavaScript puro |
| Canvas | HTML5 Canvas (minimap) |
| Estilo | CSS puro (sem framework) |

## Funcionalidades

- Tela de início com instruções de controles
- Contagem regressiva animada antes da largada
- **HUD completo:**
  - Velocímetro circular (km/h)
  - Contador de voltas (3 ao total)
  - Cronômetro por volta e melhor tempo
  - Indicador de posição (1º–4º)
  - Indicador de marcha (N, 1–6)
  - Minimapa da pista
  - Aviso "SENTIDO ERRADO!"
- 4 corredores (1 jogador + 3 IAs)
- Tela de resultado ao finalizar as 3 voltas

## Estrutura do código

```
racing-game.html
├── CSS — HUD, telas de início/fim, estilos do jogo
├── HTML — elementos do HUD e telas
└── JavaScript
    ├── CONFIG — velocidade, física, câmera
    ├── Three.js setup — cena, câmera, renderer
    ├── Pista — geração da geometria
    ├── Carros — jogador e IAs
    ├── Física — aceleração, frenagem, colisão
    ├── HUD — atualização em tempo real
    └── Game loop — requestAnimationFrame
```

## Como abrir

Abra `racing-game.html` diretamente no navegador com **internet ativa** (necessário para carregar o Three.js via CDN).

> Recomendado: Chrome, Edge ou Firefox. Não funciona offline.
