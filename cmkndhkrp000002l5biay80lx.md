---
title: "The Promise of “Disposable Software”"
datePublished: Wed Jan 21 2026 01:57:13 GMT+0000 (Coordinated Universal Time)
cuid: cmkndhkrp000002l5biay80lx
slug: the-promise-of-disposable-software
cover: https://raw.githubusercontent.com/ricardotrevisan/ricardotrevisan.github.io/master/images/image_1_20260120.png
tags: ai, reliability, softwareengineering, techtrends, enterprisesoftware, cognitiveload, disposablesoftware

---

**What changes when software becomes easy to create, but hard to eliminate? When the real cost stops being in the build and moves to the carry — plural, non-standardized, and poorly mastered — what becomes fragile?**

Quando o custo da atenção não acompanha a queda do custo do código, o valor inevitavelmente se desloca. Migra da geração para o controle, da velocidade para a previsibilidade, da automação bruta para a redução da carga cognitiva. O gargalo deixa de ser técnico e passa a ser humano.

Nesse cenário, a atenção torna-se o principal fator limitante. A aceleração técnica começa a produzir retornos decrescentes. Sistemas rápidos, porém opacos, perdem valor estrutural diante de sistemas previsíveis, compreensíveis e governáveis. A confiabilidade passa a superar a inovação como critério econômico.

O custo do software, portanto, não desaparece — ele se torna cumulativo e menos visível. Como a atenção não escala, formam-se estoques crescentes de código pouco compreendido, elevando a dívida técnica, o risco operacional e o custo futuro. Tudo isso ocorre mesmo quando o custo inicial de geração tende a zero.

É a partir dessa assimetria — código barato, atenção cara — que o discurso do *Disposable Software* precisa ser analisado.

---


A noção de *Disposable Software* vem ganhando traction como mais um hype da era dos modelos generativos. Ela se apoia em uma mudança real: a democratização de uma expertise que, historicamente, esteve concentrada na engenharia. Pela primeira vez, o custo e o tempo necessários para transformar uma ideia em algo executável caem de forma dramática.

Essa inflexão força uma pergunta central: **o que acontece quando a curva de custos para desenvolver software começa a tender a zero?**

À primeira vista, a conclusão parece direta. Se o software pode ser criado rapidamente, ele perde importância como ativo? Torna-se algo descartável, recriável sob demanda? A narrativa é sedutora, mas parte de uma extrapolação perigosa. O conceito se sustenta sobre uma base econômica e tecnológica específica, frequentemente tratada como universal quando, na prática, é contextual.

---

## The Real Basis for Disposability

O conceito emerge da convergência de três fatores.

Primeiro, modelos generativos reduziram drasticamente o custo de sair da ideia para “algo rodando”. Construir deixou de ser o gargalo.

Segundo, os ambientes de execução tornaram-se baratos e efêmeros. Cloud, containers, serverless e ambientes locais descartáveis permitem criar, executar e eliminar software com fricção operacional mínima.

Terceiro, há públicos com alta tolerância ao erro — desenvolvedores e times *AI-native* que aceitam instabilidade e mudanças frequentes em troca de velocidade.

Nesse contexto específico, planejar menos e iterar mais parece racional. É aqui que o hype encontra sua força — e também seu limite.

---

## The Cost Displacement

O erro fundamental está em confundir custo de geração com custo total. Código barato não implica atenção barata. Especificar corretamente, supervisionar agentes, compreender efeitos colaterais, lidar com comportamentos divergentes e manter sistemas continuam sendo atividades escassas.

Na prática, o custo não desapareceu; ele apenas mudou de lugar.

Hoje, o esforço está menos em escrever código e mais em decidir o que gerar, validar se está correto e entender por que falhou. Esse deslocamento desmonta a ideia de descartabilidade em qualquer contexto no qual o erro é caro.

O custo marginal de geração caiu drasticamente. O custo da decisão, da validação e da responsabilização permaneceu alto e inelástico. A limitação deixou de ser escrever código e passou a ser **assumir consequências**.

---

## Iterating Is Not a Substitute for Planning

Outra distorção recorrente do discurso é a afirmação de que “iterar é mais barato do que planejar”. Isso é parcialmente verdadeiro para experimentos pequenos, provas de conceito e ferramentas internas. Torna-se tóxico quando aplicado a sistemas que precisam existir no tempo.

Décadas de aprimoramento metodológico e práticas de redução de complexidade não surgiram por acaso. Elas são respostas diretas ao custo cognitivo de sistemas que crescem sem controle.

Abandonar essa musculatura organizacional em nome da velocidade tem um preço alto e, muitas vezes, irreversível — novamente pago em atenção.

---

## Software Easy to Create, Hard to Remove

Há uma contradição estrutural na ideia de descartabilidade.

Remover software exige atenção. Justificar a remoção exige consenso. Entender impactos exige tempo. Na retórica, o software é efêmero; na prática, ele persiste.

Sistemas em produção sobrevivem por inércia organizacional. Dependências técnicas, culturais e contratuais impedem descartes limpos. Em ambientes regulados, “jogar fora” não é uma opção sem rastreabilidade, auditoria e explicabilidade. O resultado é o acúmulo de sistemas pouco compreendidos, mas operacionalmente críticos.

Isso se estende a agentes e artefatos gerados por eles — relatórios, análises, visualizações que passam a influenciar decisões sem que sua origem, validade ou limitações sejam plenamente entendidas.

---

## Error Tolerance Is Economic

A tolerância ao erro não acompanha automaticamente a aceleração tecnológica. Ela varia por setor, contexto e tipo de usuário.

Ambientes *AI-native* aceitam instabilidade como parte do jogo. Já contextos financeiros, industriais, de saúde ou regulados endurecem requisitos à medida que o impacto do erro cresce.

É justamente nas camadas de menor conhecimento técnico que esse hype ganhou mais tração. Nelas, a confusão entre um MVP e um sistema de produção ocorre com facilidade. Modelos de IA podem gerar código, mas não garantem continuidade nem assumem responsabilidade.

A atenção de quem precisará operar e responder pelos ativos gerados em escala não é escalável.

---

## Operation as a Constraint

A filosofia de ship contínuo funciona porque desenvolvedores entendem as falhas, conseguem reagir e aceitam quebras temporárias. Isso não é descartabilidade; é domínio técnico aliado à responsabilidade operacional.

No fim, a ideia de *Disposable Software* descreve corretamente uma mudança estrutural no custo do código, mas falha ao confundi-lo com o custo total do software. Ignora atenção, manutenção e confiança. Extrapola casos de nicho para contextos onde confiabilidade é o próprio produto.

A conclusão é econômica, não ideológica. Velocidade e descartabilidade fazem sentido em ambientes *AI-native* e ferramentas de desenvolvedores. Para o *enterprise*, confiabilidade precede autonomia.

O erro não está na ideia — está em tratá-la como universal.

O hype aponta corretamente para um *hard trend* mal interpretado: **o código ficou barato, mas o software, definitivamente, não.**

Onde a atenção é escassa, vence quem reduz a demanda cognitiva — independentemente de quão barato seja gerar código.

#DisposableSoftware #AI #SoftwareEngineering #Reliability #CognitiveLoad #EnterpriseSoftware #TechTrends