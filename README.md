# DungeonKeeper Medieval Game

Um jogo de RPG com sistemas modulares e extensíveis para personagens, combate, inventário e magia.

## Sistemas Implementados

### Sistema de Personagens
- Atributos básicos
- Sistema básico de níveis
- Gerenciamento de recursos
- Classes e habilidades (em progresso)

### Sistema de Combate
- Sistema de iniciativa
- Condições e efeitos
- Tipos de dano e resistências
- Sistema de rounds e ações
- Reações e oportunidades

### Sistema de Inventário
- Sistema básico de itens
- Gerenciamento de inventário
- Sistema de equipamentos (em progresso)

### Sistema de Magias
- Sistema básico de magias
- Efeitos e condições
- Sistema de custos (em progresso)

## Estrutura do Projeto

```
src/
  systems/
    character/       # Sistema de personagens
    combat/         # Sistema de combate
    inventory/      # Sistema de inventário
    magic/         # Sistema de magias
```

## Instalação

1. Clone o repositório:
```bash
git clone https://github.com/bugijo/DungeonKeeper-Medieval-Game.git
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

3. Execute os testes:
```bash
pytest
```

## Frontend Medieval

O projeto inclui uma interface web completa com temática medieval:

- **Interface Medieval**: Design com texturas de madeira e pedra
- **Ícones SVG**: Ícones temáticos (espada, escudo, moedas, gemas)
- **Sistema de Recursos**: Ouro, diamantes e gemas
- **Páginas Completas**: Home, inventário, missões, loja, criações
- **Configurações**: Página completa de configurações com múltiplas seções

### Executar o Servidor Web

```bash
node server.js
```

Acesse: http://localhost:8080

## Contribuição

Veja [CONTRIBUTING.md](CONTRIBUTING.md) para diretrizes de contribuição.

## Licença

Este projeto está licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para detalhes.