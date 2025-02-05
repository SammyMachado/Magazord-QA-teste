# Magazord-QA-teste

<div align='center'>

![Magazord](LogoMagazord.png)

</div>

# Teste para vaga de Analista de Qualidade no Magazord.com.br
Este repositório tem como fim testar os candidatos para vaga de analista de qualidade na empresa [Magazord](https://magazord.com.br).

# 1º Cenário:

Você está trabalhando como Analista de Qualidade em um projeto de integração de marketplaces de terceiros, como Amazon e Mercado Livre, em um grande e-commerce. A equipe de desenvolvimento concluiu a implementação da integração e você é responsável por realizar os testes para garantir que a funcionalidade esteja funcionando corretamente.
Um detalhe importante, nessa integração, temos integração de estoque, anúncios, faturamento, pedidos e preço.

## Sua tarefa:

Descrever detalhadamente o plano de testes que você implementaria para validar a integração com o marketplace. Inclua no seu plano:

**1. Documentação e Materiais de Apoio:**

  - **Identificação da documentação:** No primeiro momento eu tentaria entender como a integração deveria funcionar e para que ela iria ser utilizada no dia a dia do cliente. Para isso seriam usadas todas as informações repassadas pela equipe de desenvolvimento, regras específicas sobre o funcionamento da integração, requisitos vinculados ao projeto, documentação oficial sobre os marketplaces, análise realizada pelo Analista de Sistemas, tudo que estivesse atrelado e documentado no projeto.

  - **Análise da documentação:** Através das informações acima seria possível entender o funcionamento da nova integração assim como a regra aplicada durante o seu uso, a partir disso eu definiria o que precisaria ser testado.

  - **Mapeamento dos requisitos:** Eu iria mapear de forma geral as especificações da integração, como ela será utilizada, como deverá funcionar, as validações aplicadas, os locais onde a mesma iria ser usada. 

  - **Utilização de ferramentas:** Seriam utilizadas as ferramentas disponibilizadas e usadas no dia a dia pela empresa. (Ex: Software Interno de Gerenciamento de Demandas, Ferramenta onde ficam gravadas as informações referente ao projeto).

**2. Abrangência dos Testes:**

  - **Funcionalidades:** Seria testada a integração de estoque, anúncios, faturamento, pedidos e preço e todos os demais locais onde essa integração seria utilizada.

  - **Casos de uso:** Eu iria considerar todos os casos de uso para todas as funcionalidades, para garantir que a integração está  de acordo em todos os locais impactados.

  - **Priorização dos testes:** Risco, Complexidade, Frequência de uso, Mudanças recentes.

**3. Execução dos Testes:**

  - **Ambiente de teste:** Seria utilizado o Ambiente de Homologação para garantir que a integração está de acordo em todos os locais antes de fato de liberar para o cliente.

  - **Dados de teste:** Utilizaria as informações de um cliente onde essa integração seria  implementada.

  - **Ferramentas de automação:** Iriam ser usadas as ferramentas que geralmente a empresa utiliza para esse tipo de projeto.

  - **Registro de resultados:** Os resultados dos testes seriam registrados em um documento word para depois utilizar as informações na criação dos casos de teste e na conclusão do projeto onde seria documentada toda a funcionalidade desenvolvida.

# 2º Cenário:

Você está trabalhando como Analista de Qualidade em um projeto de integração com a ferramenta de gerenciamento de estoque Bling em um grande e-commerce. A equipe de desenvolvimento concluiu a implementação da integração e você é responsável por realizar os testes para garantir que a funcionalidade esteja funcionando corretamente.

## Sua tarefa:

Descrever detalhadamente o plano de testes que você implementaria para validar a integração com a ferramenta Bling. Inclua no seu plano:

**1. Documentação e Materiais de Apoio:**

  - **Identificação da documentação:** Primeiramente eu tentaria entender como a integração com a ferramenta de gerenciamento de estoque deveria funcionar e como ela iria ser utilizada no dia a dia do cliente. Para isso seriam usadas todas as informações repassadas pela equipe de desenvolvimento, regras específicas sobre o funcionamento da integração, requisitos vinculados ao projeto, documentação oficial sobre a Bling, análise realizada pelo Analista de Sistemas, tudo que estivesse atrelado e documentado no projeto.

  - **Mapeamento dos requisitos:** Eu iria mapear de forma geral as especificações da integração com a ferramenta de gerenciamento, como ela será utilizada, como deverá funcionar, as validações aplicadas, os locais onde a mesma iria ser usada. 

  - **Utilização de ferramentas:** Seriam utilizadas as ferramentas disponibilizadas e usadas no dia a dia pela empresa. (Ex: Software Interno de Gerenciamento de Demandas, Ferramenta onde ficam gravadas as informações referente ao projeto).

**2. Abrangência dos Testes:**

  - **Funcionalidades:** Seriam realizados testes diretamente relacionados a integração com a ferramenta de gerenciamento de estoque (Cadastro de Produtos, Gerenciamento de Estoque, Controle de Compras, Emissão de Boletos) e todos os demais locais onde essa integração seria utilizada.

  - **Priorização dos testes:** Risco, Complexidade, Frequência de uso, Mudanças recentes.

**3. Execução dos Testes:**

  - **Dados de teste:** Utilizaria as informações de um cliente onde essa integração seria  implementada.

  - **Ferramentas de automação:** Iriam ser usadas as ferramentas que geralmente a empresa utiliza para esse tipo de projeto.

  - **Registro de resultados:** Os resultados dos testes seriam registrados em um documento word para depois utilizar as informações na criação dos casos de teste e na conclusão do projeto onde seria documentada toda a funcionalidade desenvolvida.

# 3º Cenário:

O cliente entrou em contato devido a uma questão relacionada aos seus anúncios. Quando os itens ficam sem estoque, em vez de serem marcados como "Pausado (sem estoque)", eles estão apenas sendo marcados como "Pausado", o que faz com que os anúncios permaneçam disponíveis para venda no Mercado Livre, mesmo sem estoque real. Isso está resultando em pedidos sendo feitos para itens sem estoque disponível, o que prejudica a reputação do cliente, pois ele precisa cancelar as vendas devido à falta de estoque.

Atualmente, o cliente possui 38 anúncios com a situação "Pausado", e ele relata que não os marcou manualmente como pausados.Quando enviamos uma atualização manual de estoque, o anúncio muda para a situação "Pausado sem estoque" e fica indisponível para venda no Mercado Livre.
Ao verificar o log dos anúncios, não encontramos registros de envio de informação de estoque igual a zero quando o estoque se esgota no Magazord.
Um exemplo de anúncio afetado é o seguinte: [MLB3097510082](https://produto.mercadolivre.com.br/MLB-3097510082-escultura-em-pedra-pirita-com-cupula-de-acrilico-_JM).
Envio em anexo um print do anúncio e um print do log, mostrando que não foram encontradas informações registradas na abertura da atividade.

Para o caso acima, descreva quais seriam os passos para analise e identificação do problema tendo em vista a documentação do próprio ML. Visto que não possui acesso ao painel seller do cliente e nem ao painel do mesmo no ERP Magazord, quais seriam as possíveis hipóteses do erro.

![anúncios pausado no magazord e sem estoque](aa.png)

Primeiramente eu iria verificar qual a validação aplicada para que os anúncios sejam definidos como ‘Pausado (sem estoque)’ para isso seria necessário procurar a documentação sobre o funcionamento dessa rotina. Depois disso eu tentaria simular a situação em um ambiente de testes para entender a origem do erro, caso não fosse possível eu solicitaria ajuda a equipe de desenvolvimento para verificar no código fonte o que poderia estar causando esse problema. Se isso fosse demandar muito tempo seria aberto um chamado para uma verificação aprofundada do problema.

# 4º Cenário:

Você está encarregado de testar a validação de dados cadastrais em um sistema de gerenciamento de usuários. O sistema possui os seguintes campos de cadastro:

- Nome completo
- E-mail
- Número de telefone
- Data de nascimento
- Endereço (com campos para rua, cidade, estado e CEP)

Houve alterações nos campos mencionados acima no cadastro do cliente, quais testes você faria para validar que o(s) campo(s) esta(ão) funcionando conforme esperado?

![Alterar pessoa](AlterarPessoa.png)

- Informar apenas o primeiro Nome no campo ‘Nome Completo’.
- Informar um E-mail inválido no referido campo.
- Informar uma data inválida no campo ‘Data de Nascimento’.
- Informar um Número de Telefone inválido no referido campo.
- Informar um Número de Telefone com mais de nove dígitos.
- Informar um CEP inválido.
- Informar uma Cidade sem relacionamento com as demais informações do Endereço.
- Informar uma Rua sem relacionamento com as demais informações do Endereço.
- Informar um Estado sem relacionamento com as demais informações do Endereço.
- Preencher todos os campos corretamente e verificar se o sistema gravou as informações.

**Orientação:** Crie casos de teste para validar a entrada de dados nos campos modificados.

## Avaliação

> [!IMPORTANT]
> **Os candidatos serão avaliados com base na clareza, precisão e detalhamento das respostas.**

> [!IMPORTANT]
> **A capacidade de compreender e comunicar efetivamente requisitos e problemas é fundamental.**

> [!IMPORTANT]
> **A organização e a estrutura das respostas também serão consideradas na avaliação.**

## Envio do teste

> [!NOTE]
> **Suba o repositório no seu Github e envie o link diretamente para o seu recrutador.**

> [!WARNING]
> **Não serão aceitos alterações após o envio, caso precise de mais tempo para implementação do projeto alinhe com o seu recrutador com antecedência.**
