---
title: Sobre wikis
intro: Você pode hospedar a documentação para seu repositório em um wiki para que outras pessoas possam usar e contribuir com seu projeto.
redirect_from:
  - /articles/about-github-wikis
  - /articles/about-wikis
  - /github/building-a-strong-community/about-wikis
product: '{% data reusables.gated-features.wikis %}'
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Community
---

Todos os repositórios em {% ifversion ghae %}{% data variables.product.product_name %}{% else %}{% data variables.product.product_location %}{% endif %} são equipados com uma seção para a documentação de hospedagem denominada wiki. Você pode usar o wiki do repositório para compartilhar conteúdo longo sobre seu projeto, por exemplo, como usá-lo, como ele foi projetado ou seus princípios básicos. Um arquivo README informa rapidamente o que seu projeto pode fazer, enquanto você pode usar um wiki para fornecer documentação adicional. Para obter mais informações, consulte "[Sobre README](/articles/about-readmes)".

Com wikis, é possível gravar conteúdo assim como em qualquer outro lugar no {% data variables.product.product_name %}. Para obter mais informações, consulte "[Começando a escrever e formatar no {% data variables.product.prodname_dotcom %}](/articles/getting-started-with-writing-and-formatting-on-github)". Usamos [nossa biblioteca de markup de código aberto](https://github.com/github/markup) para converter diferentes formatos em HTML, de modo que seja possível optar por escrever em markdown ou qualquer outro formato compatível.

{% ifversion fpt or ghes or ghec %}Se você criar um wiki em um repositório público, o wiki ficará disponível para {% ifversion ghes %}qualquer pessoa com acesso para {% data variables.product.product_location %}{% else %}o público{% endif %}. {% endif %}Se você criar um wiki em um repositório privado{% ifversion ghec or ghes %} ou interno,{% endif %} apenas {% ifversion fpt or ghes or ghec %}as pessoas{% elsif ghae %}integrantes da empresa{% endif %} com acesso ao repositório poderão acessar o wiki. Para obter mais informações, consulte "[Configurar visibilidade do repositório](/articles/setting-repository-visibility)".

Você pode editar wikis diretamente no {% data variables.product.product_name %} ou editar arquivos wiki localmente. Por padrão, somente as pessoas com acesso de gravação ao repositório podem fazer alterações no wikis, embora você possa permitir que todos em {% data variables.product.product_location %} contribuam para um wiki em {% ifversion ghae %}um repositório interno{% else %}público{% endif %}. Para obter mais informações, consulte "[Alterar permissões de acesso para wikis](/communities/documenting-your-project-with-wikis/changing-access-permissions-for-wikis)."

{% note %}

**Observação:** Os mecanismos de pesquisa não indexam o conteúdo de wikis. Para que seu conteúdo seja indexado por mecanismos de busca, você pode usar [{% data variables.product.prodname_pages %}](/pages) em um repositório público.

{% endnote %}

## Leia mais

- "[Adicionar ou editar páginas wiki](/communities/documenting-your-project-with-wikis/adding-or-editing-wiki-pages)"
- "[Criar um footer ou uma barra lateral para seu wiki](/communities/documenting-your-project-with-wikis/creating-a-footer-or-sidebar-for-your-wiki)"
- "[Editar conteúdo do wiki](/communities/documenting-your-project-with-wikis/editing-wiki-content)"
- "[Exibir histórico de alterações de um wiki](/articles/viewing-a-wiki-s-history-of-changes)"
- "[Pesquisar wikis](/search-github/searching-on-github/searching-wikis)"
