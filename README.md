# Random Password Generator#

Este é um simples gerador de senhas aleatórias em Python. O programa solicita ao usuário o tamanho desejado para a senha e utiliza caracteres alfanuméricos, símbolos e pontuações para criar uma senha aleatória.

## Como Usar

1. Execute o script em um ambiente Python.
2. Digite o tamanho desejado para a senha quando solicitado.

O programa gerará e exibirá uma senha aleatória que pode ser utilizada conforme necessário.

## Detalhes do Código

O código utiliza a biblioteca `random` e `string` do Python para gerar senhas aleatórias. Ele inclui letras maiúsculas e minúsculas, números e alguns caracteres especiais. A função `random.SystemRandom()` é utilizada para garantir uma fonte de aleatoriedade mais segura.

```python
import random
import string

tamanho = int(input('Digite o tamanho de senha que você deseja: '))

chars = string.ascii_letters + string.digits + 'ç!@#$%&*()-=+,.;:/?'

rnd = random.SystemRandom()

print(''.join(rnd.choice(chars) for i in range(tamanho)))
```

Sinta-se à vontade para modificar ou incorporar este código em seus projetos, se necessário.
