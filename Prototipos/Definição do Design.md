# Definição do Design

Este documento define o padrão de design das janelas para garantir a consistência de cores, ícones, fontes e outros elementos visuais.

- **Tamanho das fontes**:
	- **Título** (H1): 40px
	- **Sub-título** (H2): 27px
	- **Sub-título** (H3): 18px
	- **Corpo**: 12px
- **Fontes**:
	- **Títulos** (H1-3): Arial
	- **Corpo**: Roboto
- **Ícones**: https://fonts.google.com/icons (`Material Symbols (new)`)

## Cores

### Cores de categoria
- `#F2CE16` - Amarelo principal
- `#F2BD1D` - Amarelo secundário
- `#F28322` - Laranja de categoria
```palette
#F2CE16
#F2BD1D
#F28322
```

### Cores de ação
- `#1473e6` - Azul para links
- `#ff0033` - Preços e textos de ofertas
- `#F26E22` - Laranja para botões que levem para a finalização da compra
```palette
#1473e6
#ff0033
#F26E22
```

### Cores de texto
- `#030303` - Preto para texto no geral
- `#F2F2F2` - Cinza para textos riscados ou itálico
```palette
#F2F2F2
#030303
```

# Regras de Design

## Ícones
- `#030303` ou `#F2F2F2` - Os ícones devem usar apenas preto ou branco, dependendo do contraste com o fundo
- Tamanho padrão: 24px para ícones de interface
- Usar apenas ícones do **Material Symbols** para manter consistência

## Botões
- `#F26E22` - Apenas botões de ação primária (confirmar compra, adicionar ao carrinho) devem ter cor de destaque
- Botões secundários devem usar apenas bordas ou texto colorido
- Botões desabilitados usam `#F2F2F2` com 50% de opacidade

## Hierarquia Visual
- Elementos mais importantes recebem maior contraste e cores vibrantes
- Textos secundários usam `#F2F2F2` para reduzir peso visual
- Máximo de 3 cores por tela para evitar poluição visual