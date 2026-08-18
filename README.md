# Desafio técnico — Desenvolvedor(a) Júnior

E aí Dev!

Que bom que você chegou aqui! A próxima etapa consiste em um desafio técnico para validar seus conhecimentos.

O desafio não é grande, mas tem algumas decisões de verdade dentro dele. É exatamente isso que queremos ver: como você pensa quando o problema não tem uma resposta única.

## Stack

Para esta vaga, a stack é requisito:

- **Front-end: React**
- **Back-end: C# / .NET**
- **Banco de dados relacional** (o de sua preferência)

## O desafio

Um coworking precisa de uma aplicação web para gerenciar as reservas das suas salas de reunião.

A aplicação deve:

- **Listar as reservas**, agrupadas por dia e em ordem cronológica, com **filtro por sala e por intervalo de datas**;
- **Criar uma reserva**, informando: sala, título, horário de início e horário de fim;
- **Cancelar uma reserva**.

Regras de negócio:

- Sala, título, início e fim são obrigatórios;
- O horário de fim precisa ser depois do horário de início;
- **Duas reservas na mesma sala não podem se sobrepor no tempo.** Essa validação é responsabilidade do back-end;
- As salas podem ser fixas no código ou criadas por um seed. Você **não** precisa construir um cadastro de salas.

## Os três pontos que mais vamos olhar

### 1. Concorrência

Duas pessoas clicam em "reservar" para a mesma sala, no mesmo horário, no mesmo instante.

**Sua aplicação não pode aceitar as duas.** Resolva isso e explique no README qual abordagem você escolheu e qual o trade-off dela.

### 2. Testes automatizados

Escreva testes cobrindo a regra de sobreposição, **incluindo os casos de borda**.

Não precisa cobrir o projeto inteiro. Precisa cobrir bem o que importa.

### 3. Cancelamento

Decida se cancelar deve **remover o registro do banco** ou apenas **marcar a reserva como cancelada** — e justifique sua escolha no README.

Não existe resposta certa aqui. Existe resposta bem pensada.

## Uma questão de projeto (sem implementar)

O coworking já avisou que, no futuro, vai querer **reservas recorrentes** — por exemplo, "toda terça-feira às 14h, durante 8 semanas".

**Não implemente isso.** Apenas descreva no README como você evoluiria seu modelo de dados para suportar recorrência, e o que aconteceria ao cancelar uma única ocorrência de uma série.

## Sobre o uso de IA

Você pode usar IA à vontade.

Não vamos avaliar se você usou — vamos avaliar se **você entende o que entregou**. No vídeo, e depois numa conversa ao vivo, você vai precisar explicar as decisões do seu código.

Então use como quiser, mas garanta que você entende cada parte do que está entregando.

## Entrega

São **duas** entregas: o código e um vídeo.

### 1. Código

Publique o código-fonte em um repositório público no GitHub, com um README explicando:

- Como rodar o projeto;
- Sua abordagem para o problema de concorrência e o trade-off dela;
- Sua justificativa para a decisão do cancelamento;
- Como você evoluiria o modelo para reservas recorrentes.

### 2. Vídeo (máximo 7 minutos)

Grave um vídeo de **no máximo 7 minutos** apresentando o que você construiu.

**O vídeo deve ser uma gravação contínua, sem cortes e sem edição.** Não precisa ficar perfeito — travar, se enrolar ou refazer uma frase faz parte, e não é problema nenhum. Queremos ouvir você pensando, não um vídeo produzido.

Siga esta ordem:

| # | O que mostrar | Tempo |
|---|---|---|
| 1 | **Overview do projeto.** Estrutura de pastas do back-end e do front-end, como você organizou as responsabilidades e por que dessa forma. | ~2min |
| 2 | **A aplicação rodando.** Crie uma reserva. Depois tente criar outra que conflita com ela e mostre o que acontece. | ~1min |
| 3 | **A regra de sobreposição.** Abra o arquivo onde ela vive, explique a lógica e mostre os testes que a cobrem. | ~1min30 |
| 4 | **Concorrência.** Como você garantiu que duas requisições simultâneas não criam reservas conflitantes, e por que escolheu essa abordagem. | ~1min30 |
| 5 | **Recorrência.** Como você evoluiria o modelo de dados para suportar reservas recorrentes. | ~1min |

Você pode gravar com a ferramenta que preferir (Loom, OBS, Google Meet, gravador de tela do sistema). Suba em algum lugar com link compartilhável — YouTube como "não listado", Google Drive ou o próprio Loom.

### Envio

Envie um e-mail para **danilo@spedy.com.br** com:

- O link do repositório;
- O link do vídeo.

**Prazo: 23/08/2026 (domingo), às 23h59.**

## Recomendações

- **Capriche na qualidade e organização do código.** Esse é o principal ponto que analisamos;
- **Comece o quanto antes.** Não deixe para fazer perto da data de entrega, isso pode te atrapalhar;
- **Visual é importante.** Uma aplicação com um bom design te diferencia;
- **Prefira entregar menos, mas entendendo tudo.** Uma solução simples que você sabe explicar vale mais aqui do que uma solução elaborada que você não sabe defender.

#### Um abraço e boa sorte!
