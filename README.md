# Validador de CPF 🕵️‍♂️

## Descrição
Ferramenta para validar números de Cadastro de Pessoas Físicas (CPF) utilizando o algoritmo oficial de verificação.

## Funcionalidades
- Valida CPFs com ou sem formatação
- Verifica dígitos verificadores
- Impede validação de sequências numéricas repetidas

## Algoritmo de Validação 🧮

### Etapas de Validação
1. Remove caracteres não numéricos
2. Verifica se não é uma sequência repetida
3. Calcula primeiro dígito verificador:
   - Multiplica 9 primeiros dígitos por pesos regressivos
   - Aplica cálculo específico
4. Calcula segundo dígito verificador:
   - Usa 9 dígitos originais + primeiro dígito
   - Multiplica por pesos regressivos
   - Aplica cálculo específico
5. Compara CPF original com CPF calculado

## Exemplo de Uso
```python
# Execute o script e insira um CPF
python validador_cpf.py
# Siga as instruções no prompt
```

## Casos de Teste
- ✅ CPF válido: `746.824.890-70`
- ❌ CPF inválido: `111.111.111-11`

## Regras de Validação
- Aceita entrada formatada e não formatada
- Rejeita sequências numéricas
- Calcula dígitos verificadores rigorosamente

## Tecnologias
- Linguagem: Python
- Bibliotecas: `re`, `sys`

## Contribuição
Contribuições são bem-vindas! Abra issues ou envie pull requests.

## Licença
MIT License
