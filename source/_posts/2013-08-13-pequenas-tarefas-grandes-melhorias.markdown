---
layout: post
title: "Pequenas tarefas, grandes melhorias"
date: 2013-02-27 09:09
comments: true
categories: [agile, rails, leadership]
---

Ultimamente, venho pensado muito em como melhorar a parte interna das aplicações em que trabalho, de forma que não atrapalhe a entrega de valor ao cliente.

Cheguei a uma solução a longo prazo baseada nas quests existentes em RPGs.

# Quests

Eu joguei [MMORPG](http://en.wikipedia.org/wiki/MMORPG), mais precisamente [World of Warcraft](http://en.wikipedia.org/wiki/WoW), por muitos anos.

Em praticamente todos os "[role-play games](http://en.wikipedia.org/wiki/Role-playing_game)", há diversas tarefas, conhecidas como quests. Essas quests são uma lista de "metas" a serem cumpridas para se conseguir uma pequena recompensa.

Em alguns jogos, existem as chamadas "daily quests", que se resume em fazer a mesma quest todos os dias em busca de uma grande recompensa a longo prazo.

# Realidade no desenvolvimento de software

Nos sistemas da [IntegraGRP](http://integragrp.com.br/) nós temos diversas melhorias a serem feitas.

Como nós somos um grupo de desenvolvedores que adora código limpo, bem testado e rápido, gostamos de manter tudo atualizado para ter acesso as principais vantagens de cada ferramenta.

Isso tudo é muito bonito, mas não é tarefa fácil conseguir, pois temos muitos sistemas e cada um deles de tamanho considerável.

## Exemplos de melhorias:

* Atualização para o [Capybara](https://github.com/jnicklas/capybara) 2.0;
* Troca do [Machinist](https://github.com/notahat/machinist) pelo [FactoryGirl](https://github.com/thoughtbot/factory_girl);
* Verificar testes de aceitação que podem ser rodados com [rack-test](https://github.com/brynary/rack-test) ao invés do [poltergeist](https://github.com/jonleighton/poltergeist), em favor performance;
* Junção de cenários que fazem [CRUD](http://en.wikipedia.org/wiki/Create,_read,_update_and_delete) (ao invés de um cenário para criar, outro para editar e outro para apagar, usar apenas um, diminuindo o tempo dos testes).

## Vamos supor um caso:

* atualização do Capybara;
* criamos um branch para esta alteração, e lá aplicamos o básico;
* o servidor de [integração contínua](http://en.wikipedia.org/wiki/Continuous_integration) irá rodar os testes;
* 100 testes quebram;
* temos 4 desenvolvedores.

### Resultado não exato:

Nós sabemos que em planejamento de desenvolvimento de software a matemática não é exata... mas... digamos que seja.

Em aproximadamente 25 dias de trabalho, com apenas alguns minutos por dia para cada dev arrumar um teste, teríamos uma app melhorada.

Com tudo pronto, temos desenvolvedores satisfeitos e motivados para um próximo desafio.

# Conclusão

Acredito que pequenas tarefas diárias, para resolver grandes problemas não prioritários é um ótimo caminho para aperfeiçoar o software, sem ter de sacrificar o mais importante, a entrega de valor ao cliente.

Lembre-se, para grandes mudanças, pequenos atos!
