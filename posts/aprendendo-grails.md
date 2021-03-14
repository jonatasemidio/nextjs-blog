---
title: "Aprendendo Grails"
date: "2012-06-26"
categories: 
  - "basico"
tags: 
  - "agil"
  - "grails"
  - "groovy"
---

Primeiramente, gostaria deixar claro o porquê de iniciar este blog e o motivo de iniciar nesta jornada grails.

Tudo começou com uma proposta para trabalhar em um projeto que já estava utilizando Grails. Assim que soube da proposta fui dar uma olhada na net mais a fundo sobre este framework que eu já tinha ouvido falar, mas por já utilizar Java em minhas aplicações complexas e python/Django em aplicações rápidas me via bem equipado para qualquer situação. Até que eu notei uma grande semelhança na sintaxe do Grails com Python e Java. Foi quase amor a primeira vista.

Ok… Mas não foi tão simples assim. Como de costume, comecei a pesquisar exemplos práticos da linguagem para ter maior noção se eu me adaptaria com facilidade.

Achei um exemplo simples, mas, completo. Criei um sistema inteiro de cadastro de produtos, incluindo tela, acesso ao banco e todo o CRUD completo com apenas quatro linhas de comando simples e uma pequena alteração na classe de modelo gerada.

Detalhamento do procedimento executado:

1 – comando para a criação do projeto loja: grails create-app loja;

2 – comando para a criação da classe de domínio Produto: grails create-domain-class Produto;

3 – declaração os atributos de produto na classe gerada no diretório (“projeto” /grails-app/domain/ “package”/”classe”): String nome, double valor e Date dataCadastro;

4 – comando para a geração da estrutura lógica inicial do negócio para o domínio Produto, ou seja, (CRUD): grails generate-all loja.Produto;

5 – Pronto, agora é só executar e testar: grails run-app.

Por incrível que pareça o projeto já está pronto e funcional utilizando os templates default do grails e acesso ao HSQLDB para persistência.

[![](/images/app.png?w=300)](https://santograils.files.wordpress.com/2012/06/app.png)

_Print do resultado após a execução da aplicação._

Por fim, esta foi apenas uma descrição de como é simples a criação de um projeto utilizando grails. Lembrando que ao final e gerado o bytecode do projeto, ou seja, o seu sistema terá o mesmo desempenho que os criados em Java. Espero que vocês estejam tão interessados quanto eu fiquei ao finalizar este exemplo, pois os próximos posts serão para a criação do mesmo projeto, porem detalhando cada comando.

Até a próxima.
