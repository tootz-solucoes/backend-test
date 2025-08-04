# Teste Técnico para Desenvolvedor Backend na [TTZ.](https://ttz.dev.br)

_Dá uma lida com calma em cada parágrafo, **todos** são importantes._

Este é um teste técnico para a vaga de Desenvolvedor Backend. Você deve ter recebido esse link após ter sido aprovado nas etapas iniciais do nosso processo seletivo. Se chegou aqui por acaso, sinta-se à vontade para realizar o teste e nos enviar o resultado, ficamos felizes com o seu interesse em fazer parte do nosso time.

A [**TTZ.**](https://ttz.dev.br) é uma fábrica de software especializada no desenvolvimento e manutenção de produtos digitais de várias áreas. Nos tornamos a equipe de tecnologia dos projetos dos nossos clientes. Sendo assim, nosso dia a dia envolve a resolução de problemas e implementação de novas funcionalidades trazidas por eles. Além disso, nossa equipe de desenvolvimento também é responsável por manter dois produtos "da casa".

## O problema que você precisa resolver

Você recebeu um **log bruto** gerado por um servidor do jogo *BattleQuest*.
Esse log contém **centenas de milhares de eventos** representando interações entre jogadores, combate, coleta de itens, progressão em quests e mensagens do sistema.

Sua tarefa é **processar esses dados e construir uma API** que permita consultas e dashboards sobre o que aconteceu no jogo.

---

### **Objetivo**

* Criar um **serviço backend** que:

  1. **Carregue e armazene** os eventos do log em um banco de dados.
  2. Disponibilize **endpoints REST** para consultas e estatísticas.
  3. Permita **filtros e agregações** úteis para análise.

---

### **Tarefas obrigatórias**

1. **Processamento e persistência**

   * Ler o arquivo de log e extrair campos relevantes.
   * Normalizar dados (datas, números, strings).
   * Armazenar em banco relacional ou NoSQL.

2. **API mínima**

   * `GET /players` → lista de jogadores com dados básicos.
   * `GET /players/:id/stats` → estatísticas de um jogador (pontuação, mortes, itens coletados, quests concluídas).
   * `GET /leaderboard` → ranking de jogadores por pontuação.
   * `GET /events?limit=50` → últimos eventos.
   * `GET /items/top` → itens mais coletados.

---

### **Desafio extra (opcional)**

* Endpoint `/dashboard` com:

  * Total de jogadores ativos no intervalo.
  * Pontuação total acumulada.
  * Itens mais coletados.
  * Jogadores com mais mortes.
  * Chefes derrotados.
* Atualização contínua: permitir adicionar novos logs sem duplicar dados.
* Autenticação simples (token via header).
* Documentação (Swagger ou README).
* Testes automatizados

---

### **Critérios de avaliação**

| Critério                                         | Peso |
| ------------------------------------------------ | ---- |
| Modelagem de dados clara e escalável             | 20%  |
| Qualidade do código (organização, boas práticas) | 20%  |
| Corretude funcional (respostas corretas)         | 20%  |
| Eficiência no processamento e consultas          | 15%  |
| API bem projetada e documentada                  | 15%  |
| Extras / Criatividade                            | 10%  |

---

📄 **Arquivo de entrada:**
[Log](./assets/game_log_large.txt)

---

## Como você deve entregar seu teste

Nos envie um e-mail para backend@tootz.com.br contendo:

- Seu nome;
- URL do repositório público;
- Observações e comentários que julgar relevante sobre o seu código;

> **"Mas eu estou trabalhando atualmente e não posso publicar esse repositório no meu perfil público"**

A forma como você escreve e organiza os seus _commits_ também é avaliada no teste, mas se realmente é um impedimento para você nos envie o seu código fonte compactado.

## O que esperamos do seu teste

A forma como você organiza seus arquivos, estrutura seus métodos, nomeia variáveis e gerencia seu código como um todo também será avaliada. Portanto, seja cuidadoso e adote boas práticas e padrões.

Precisamos saber como rodar seu projeto, por isso, garanta que o conteúdo do README seja suficiente para nos guiar neste momento.

**Leia o teste inteiro, pelo menos 3 vezes até o final, e adicione "NANDATÊ" no final do seu e-mail de entrega.**

## O que vai nos impressionar no seu teste

Se encontrarmos testes unitários e/ou de aceitação com certeza você vai ganhar uns pontinhos a mais na seleção.

---

Vamos revisar seu código, testar e avaliar o resultado. Aproveite o tempo indicado para fazer o teste e mostre suas habilidades!

Se tiver alguma dúvida não se acanhe e envie um e-mail para backend@tootz.com.br.
