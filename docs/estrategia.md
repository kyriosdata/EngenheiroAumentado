### O Desafio do Engenheiro Aumentado

Temos um desafio: "Como podemos nos tornar 'Engenheiros de Software Aumentados', usando LLMs para sermos mais rápidos, criativos e estratégicos?". 

### Boas-vindas

Nesta disciplina, vocês "não serão estudantes", mas pioneiros explorando a Engenharia de Software empoderada pelo uso de LLMs
para executar várias [atividades](possibilidades.md) divididas em fases e organizadas nas missões abaixo.

---

### Missão 1: A Simulação de Consultoria (Fases 0 e 1)

Toda grande inovação começa com uma ideia. Frequentemente, essa ideia é vaga e caótica. A sua primeira missão é identificar uma ideia de uso de hemogramas em um contexto estadual e transformar o caos (ideia) em clareza.

* Atividade: vocês serão divididos em equipes de "consultoria de inovação". Uma "gravação" de cerca de 30 minutos, de uma reunião caótica com o "cliente", será disponibilizada para inspirar trabalhos (ideias). A gravação não foi criada artificialmente para dificultar, de fato, é cenário comum e, em particular, nesse caso, real. Veja aqui a [ideia](ideia.md).

* Primeiro: qual o trabalho (ideia) que o grupo tem para o domínio dos hemogramas?

* Segundo. Sua Missão com LLM: atuem como consultores de ponta com base em uma ideia que o grupo deverá identificar e trabalhar. Usem LLMs para:
    1.  Analisar o Mercado: realizar a Fase 0, pesquisando o cenário, concorrentes e tendências para validar a ideia.
    2.  Decifrar o Cliente: transcrever a gravação da reunião e extrair os requisitos funcionais, não funcionais e as restrições do projeto.
    3.  Propor Soluções: gerar uma lista de perguntas inteligentes para esclarecer as dúvidas e escrever as primeiras Histórias de Usuário.

* Critério de Sucesso: a sua avaliação será a qualidade do Relatório de Viabilidade que vocês apresentarão ao "cliente". Sua capacidade de usar o LLM para encontrar insights e depois validar e refinar esses insights criticamente será a chave para o sucesso.

Caso queira um exemplo: [Sistema de previsão de demanda hematológica](./previsao-demanda-hematologia.md).
É fácil encontrar vários modelos de hemograma disponíveis na internet. Caso queira uma lista dos 24 "itens de informação" coletados,
você pode identificá-los [aqui](https://fhir.saude.go.gov.br/r4/exame/hemograma.html#exames-simples-todos-eles).

Talvez seja útil comparar seu uso de LLMs para realizar a missão 1 com as sugestões abaixo. Talvez você possa "turbinar"
sua forma de interação com estes modelos.

#### Prompt Engineering for Generative AI, James Phoenix, Mike Taylor, O’Reilly, 2024.

Abaixo seguem 6 princípios de prompts, sendo os 5 primeiros da referência acima. O sexto é um acréscimo considerado oportuno por muitos.

- _Dê direcionamento_. Descreva o estilo desejado em detalhes, ou referencie uma persona relevante. Exemplo: "Responda como um médico experiente explicando para um paciente leigo, usando linguagem simples e empática."
- _Especifique o formato_. Defina quais regras seguir e a estrutura obrigatória da resposta. Exemplo: "Forneça a resposta em 3 parágrafos: 1) Definição, 2) Causas principais, 3) Soluções práticas."
- _Forneça exemplos_. Insira um conjunto diverso de casos de teste onde a tarefa foi executada corretamente. Exemplo: "Classifique estas emoções: 'Estou radiante hoje!' → Alegria | 'Que decepção terrível' → Tristeza"
- _Avalie a qualidade_. Identifique erros e classifique respostas, testando o que impulsiona o desempenho. Exemplo: "Avalie sua resposta de 1-10 considerando clareza, precisão técnica e utilidade prática."
- _Divida o trabalho_. Fragmente tarefas em múltiplas etapas, encadeadas para objetivos complexos. Exemplo: "Primeiro analise o problema, depois liste 3 soluções, então compare prós e contras de cada uma."
- _Estabeleça restrições_. Defina claramente limitações, escopo e o que NÃO deve ser feito na resposta. Exemplo: "Responda em máximo 100 palavras, sem usar jargões técnicos ou mencionar marcas específicas."

---

### Missão 2: Hackathon "Do Requisito ao Protótipo em 48h" (Fases 2, 3 e 4)

Com os requisitos ou parte deles, possivelmente aprovados, é hora de construir. Mas vocês farão isso em velocidade máxima.

* Atividade: bem-vindos ao nosso hackathon! Usando os requisitos que sua equipe registrou (missão anterior), vocês terão 48 horas para dar vida a uma parte essencial do sistema. É possível que você tenha uma "visão clara" de um produto, mas a documentação dos requisitos não esteja completa. Nesse caso, será necessário identificá-los, pelo menos um conjunto suficiente para a primeira iteração.
* Sua Missão com LLM: o desafio é claro: projetar e codificar uma funcionalidade central, usando LLMs de forma intensiva para acelerar cada etapa:
    1.  Planejamento Ágil: transformem suas Histórias de Usuário em um backlog inicial e um plano de sprints. Sem uma lista de requisitos não terá muito o que fazer aqui. Para ajudar aqui, alguns possíveis prompts...
        1. "crie uma lista de histórias de usuário a partir da descrição da ideia (descreva ela aqui)".  
        2. "Verifique minha lista de histórias de usuário. O conjunto está coerente?"
        3. "crie um plano de sprints para a implementação das histórias de usuário. Este plano deve considerar uma equipe de 3 colaboradores, trabalhando 4 horas por semana perfazendo um total de 48 horas. Se for o caso, identifique quais histórias de usuário não podem ser implementadas tendo em vista o esforço disponível."
    2.  Arquitetura Inteligente: gerem diagramas de arquitetura (usando formatos como PlantUML ou Mermaid) e o esquema do banco de dados. A arquitetura, naturalmente, deve ser uma proposta de software que satisfaz os requisitos. 
        1. "crie um diagrama de arquitetura que identifique os principais componentes necessários para implementação das histórias de usuário"
        2. "gere a documentação correspondente para cada um dos componentes identificados".
    3.  Revise o planejamento. Provavelmente o planejamento deve ser atualizado para refletir o conhecimento acumulado com a definição da arquitetura e dos componentes.
    4.  Codificação Aumentada: gerem o código-fonte da funcionalidade, scripts de integração e a documentação técnica.
* Critério de Sucesso: além do software funcional e os artefatos gerados para os demais itens acima, cada equipe deverá manter um "Diário de Bordo do Engenheiro Aumentado", registrando os prompts utilizados, os resultados (bons e ruins!), as lições aprendidas e uma estimativa do tempo economizado (caso não possua uma estimativa, deixe em branco). A criatividade e a eficiência no uso das ferramentas serão celebradas!

---

### Missão 3: Cenário de "Aceitação ampla" (Fases 5, 6 e 7)

Antes de ir para produção é necessário verificar de forma criteriosa se a solução atende o esperado.
Também é imprescindível que possa ser implantada com certa facilidade e acompanhada de um
plano de manutenção. 

* Atividade: é preciso assegurar que o que foi realizado atende o que é esperado, conforme esperado.
* Sua Missão com LLM: usem LLMs para:
    1.  Caçar os Bugs: analisar o código para gerar casos de teste (unitários e de integração) que exponham as falhas, inclusive testes funcionais, possivelmente para gerar dados em saúde, eventuais relatórios adequados para consumo de profissionais de saúde.
    2.  Diagnosticar a Causa Raiz: analisem os logs de erro para identificar a origem dos problemas e peçam sugestões de correção.
    3.  Entregar a Solução: após corrigir os bugs, gerem scripts para automatizar o deploy da nova versão e criem uma documentação clara para o usuário final sobre as melhorias.
* Critério de Sucesso: a sua capacidade de resolver um problema real sob pressão. Vocês serão avaliados pela eficácia das correções e pela qualidade dos artefatos gerados (testes, scripts, documentação), comparando a cobertura de testes e a estabilidade do sistema antes e depois da sua intervenção.

---

### Nosso Legado: Construindo o Mapa Mental e o Repositório `EngenheiroAumentado`

Esta disciplina é uma construção coletiva. Todo o conhecimento gerado se tornará um legado para futuras turmas.

* Ferramentas e Experimentação: juntos, vamos alimentar nosso repositório no GitHub, a "Awesome List do Engenheiro Aumentado". Sua contribuição é fundamental: cataloguem ferramentas, compartilhem prompts eficazes para cada fase e criem pequenos tutoriais.
* Debates Éticos e Estratégicos: a tecnologia é mais do que código. Preparem seus argumentos! Teremos debates sobre os dilemas e o futuro que os LLMs trazem. "Um LLM pode substituir um Product Owner?". "Quais as implicações de segurança de usar código gerado para um sistema crítico?".
* O Mapa Mental como seu Portfólio: o mapa mental que você irá construir não é apenas um trabalho, é o seu portfólio vivo como Engenheiro Aumentado. Ele deve conter não apenas a teoria, mas evidências concretas de suas missões: snippets de código, diagramas, análises e, o mais importante, suas reflexões sobre os sucessos, os fracassos e o que você aprendeu no processo.
