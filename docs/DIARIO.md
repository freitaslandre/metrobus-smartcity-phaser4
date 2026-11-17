# Diário de Desenvolvimento — MetroBus: Smart City

- **Unidade Curricular:** Sistemas Multimédia (2026–2027)
- **Curso:** Engenharia da Computação Gráfica e Multimédia (UNIPVC – ESTG)
- **Estudante:** André Freitas (N.º 33782)
- **Tema:** Cidades Inteligentes e Mobilidade Autónoma
- **Repositório Git:** https://github.com/freitaslandre/metrobus-smartcity-phaser4

---

## Sessão 1 — 17 de novembro de 2026

**Objetivo:** Conceção do jogo, definição dos requisitos técnicos do tema, elaboração dos protótipos de baixa fidelidade, criação do repositório Git e redação do Relatório Inicial.

**Atividades realizadas:**
- Analisei o enunciado do trabalho prático e alinhei a mecânica principal do jogo (MetroBus: Smart City) com o tema sorteado (Cidades Inteligentes e Mobilidade Autónoma).
- Defini os dois conceitos técnicos obrigatórios a implementar nas regras do jogo:
  1. **Infraestrutura Inteligente (V2I e Smart Grid):** semáforos adaptativos que dão prioridade ao transporte público mediante sensores de zona, e gestão dinâmica da bateria do autocarro elétrico com postos de carregamento.
  2. **Mobilidade Autónoma (Tráfego Conectado V2V e Roteamento Dinâmico):** veículos autónomos com manutenção automática de distância de segurança e recálculo de rotas alternativas em tempo real no minimapa perante bloqueios aleatórios na via.
- Estruturei a progressão em 2 níveis base (Cidade Calma e Muita Gente), prevendo um 3.º nível (Hora de Ponta) como extra, a mecânica de passageiros sob pedido (On-Demand) e a arquitetura modular em classes JavaScript (`Bus`, `TrafficCar`, `TrafficLight`, `Pedestrian`, `RoutePlanner`, `HUD`).
- Desenhei à mão os protótipos de baixa fidelidade (Menu Inicial e Ecrã de Jogo) e fotografei-os para inclusão no relatório.
- Criei o repositório remoto no GitHub (`metrobus-smartcity-phaser4`) e concluí a redação do Relatório Inicial para submissão até 18 de novembro.

**Problemas:**
- Dúvida inicial sobre como garantir que o jogo não fosse apenas visualmente temático, mas que integrasse mecânicas reais de cidades inteligentes sem comprometer a jogabilidade nem o prazo.
- Necessidade de ajustar a orientação e a legibilidade das fotografias dos esboços no documento final.

**Solução:**
- Integrei os sistemas V2I, V2V e Smart Grid diretamente nas condições de vitória/derrota e na pontuação (prioridade nos semáforos, necessidade estratégica de carregamento e desvio de bloqueios).
- Optei por utilizar o motor Arcade Physics em vez de Box2D, por ser mais simples para um jogo 2D top-down e facilitar a deteção de zonas/sensores.

**Decisões:**
- Fixar a arquitetura base antes da entrega do Relatório Inicial, uma vez que não são permitidas alterações ao jogo após 18 de novembro.
- Iniciar na próxima sessão a configuração base do projeto em Phaser 4, a estrutura de Scenes (`MainMenu`, `Game`, `GameOver`) e o mapa da cidade.

**Utilização de Inteligência Artificial:**

| Ferramenta | Finalidade | Resultado utilizado e decisões do estudante |
|---|---|---|
| Google Gemini | Validação dos requisitos para a ideia. | Adaptei o conceito para condução de autocarro elétrico com câmara de seguimento e minimapa, desenhei os meus próprios protótipos à mão e ajustei o texto para refletir as funcionalidades que pretendo implementar. |
| Claude (Anthropic) | Revisão do Relatório Inicial face ao enunciado, correção de gralhas e do texto da secção do protótipo, e apoio na criação do repositório, do README e deste diário. | Aceitei as correções (regras de pontuação e vidas, conceitos 1 e 2 mais claros, Nível 3 como extra, indicação do VirtualJoystick). |