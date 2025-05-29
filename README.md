# Dungeon Keeper - Medieval Game

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
git clone https://github.com/bugijo/dungeon-keeper.git
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

3. Execute os testes:
```bash
pytest
```

## Uso

### Exemplo básico de personagem:

```python
from src.systems.character.character import Character
from src.systems.character.attributes import Attributes

# Criar um personagem
attributes = Attributes(strength=15, dexterity=14, constitution=13)
character = Character("Aragorn", attributes)

# Subir de nível
character.gain_experience(1000)
print(f"Nível: {character.level}")
```

### Exemplo de combate:

```python
from src.systems.combat.combat_state import CombatState
from src.systems.combat.actions import AttackAction

# Iniciar combate
combat = CombatState([character1, character2])
combat.start_combat()

# Executar ação
action = AttackAction(character1, character2)
combat.execute_action(action)
```

## Contribuição

Veja [CONTRIBUTING.md](CONTRIBUTING.md) para detalhes sobre como contribuir.

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.