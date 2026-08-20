# Atividade Prática – Integração Contínua

## 1. Nome do aluno / dupla

Nome completo: Gabriel Santos da Silva

## 2. Repositório

Link: https://github.com/gbrsntz/atividade-devops-ci-

## 3. Ferramentas utilizadas

- Git
- GitHub
- GitHub Actions
- Python
- Pytest

## 4. O que foi desenvolvido?

Desenvolvi uma aplicação simples em Python com funções para realizar soma, subtração e multiplicação de dois números. Também criei testes automatizados para verificar se cada função retorna o resultado correto.

## 5. Como funciona a pipeline?

Após um `git push` para a branch `main`, o GitHub Actions inicia a pipeline automaticamente. Ela baixa o código do repositório, configura o Python 3.12, instala as dependências do `requirements.txt` e executa os testes com o Pytest. Se todos os testes passarem, a execução fica verde. Se algum teste falhar, a execução fica vermelha e apresenta o erro no log.

## 6. Teste realizado

Foram criados três testes automatizados: um para soma, um para subtração e um para multiplicação.

## 7. Falha proposital

Introduzi temporariamente um erro no teste da soma, alterando o resultado esperado de 5 para 6.

## 8. Resultado

Sim. A pipeline identificou o erro, marcou a execução como falha e mostrou no log que o resultado retornado pela função era diferente do valor esperado. Depois da correção, os três testes passaram novamente.

## 9. Conclusão

Entendi que Integração Contínua é uma prática que verifica automaticamente as alterações enviadas ao repositório. A cada `git push`, a pipeline executa os testes e ajuda a encontrar erros rapidamente, antes que eles cheguem a outras etapas do projeto. Isso torna o desenvolvimento mais organizado, confiável e seguro.
