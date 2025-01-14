---
title: Adicionar um tema ao site do GitHub Pages com o seletor de temas
intro: 'É possível adicionar um tema ao site do {% data variables.product.prodname_pages %} para personalizar a aparência dele.'
redirect_from:
  - /articles/creating-a-github-pages-site-with-the-jekyll-theme-chooser
  - /articles/adding-a-jekyll-theme-to-your-github-pages-site-with-the-jekyll-theme-chooser
  - /articles/adding-a-theme-to-your-github-pages-site-with-the-theme-chooser
  - /github/working-with-github-pages/adding-a-theme-to-your-github-pages-site-with-the-theme-chooser
product: '{% data reusables.gated-features.pages %}'
versions:
  fpt: '*'
  ghec: '*'
topics:
  - Pages
shortTitle: Adicionar tema a um site de Páginas
permissions: 'People with admin permissions for a repository can use the theme chooser to add a theme to a {% data variables.product.prodname_pages %} site.'
---

## Sobre o seletor de temas

{% ifversion pages-custom-workflow %}

{% note %}

**Note**: The Jekyll theme chooser is not supported for {% data variables.product.prodname_pages %} sites that are published with a custom {% data variables.product.prodname_actions %} workflow. If you build your site with Jekyll and publish your site with a custom {% data variables.product.prodname_actions %} workflow, you can add a theme by editing the `_config.yml` file. For more information, see "[Adding a theme to your GitHub Pages site using Jekyll](/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll)."

{% endnote %}

{% endif %}

O seletor de temas adiciona um tema do Jekyll ao repositório. Para obter mais informações sobre o Jekyll, consulte "[Sobre o {% data variables.product.prodname_pages %} e o Jekyll](/articles/about-github-pages-and-jekyll)".

O funcionamento do seletor de temas depende de o repositório ser público ou privado.
  - Se o {% data variables.product.prodname_pages %} já estiver habilitado para o repositório, o seletor de temas adicionará o tema à fonte de publicação atual.
  - Se o repositório for público e o {% data variables.product.prodname_pages %} estiver desabilitado para ele, o uso do seletor de temas habilitará o {% data variables.product.prodname_pages %} e definirá o branch-padrão como fonte de publicação.
  - Se o repositório for privado e o {% data variables.product.prodname_pages %} estiver desabilitado para ele, será preciso habilitar o {% data variables.product.prodname_pages %} definindo uma fonte de publicação para poder usar o seletor de temas.

Para obter mais informações sobre fontes de publicação, consulte "[Sobre o {% data variables.product.prodname_pages %}](/articles/about-github-pages#publishing-sources-for-github-pages-sites)".

Caso você tenha adicionado manualmente um tema do Jekyll ao repositório no passado, esses arquivos poderão ser aplicados mesmo depois que você usar o seletor de temas. Para evitar conflitos, remova todas as pastas e arquivos de temas adicionados manualmente antes de usar o seletor de temas. Para obter mais informações, consulte "[Adicionar um tema ao site do {% data variables.product.prodname_pages %} usando o Jekyll](/articles/adding-a-theme-to-your-github-pages-site-using-jekyll)".

## Adicionar um tema com o seletor de temas

{% data reusables.pages.navigate-site-repo %}
{% data reusables.repositories.sidebar-settings %}
{% data reusables.pages.sidebar-pages %}
3. No "{% data variables.product.prodname_pages %}", clique em **Escolher um tema** ou **Alterar tema**. ![Botão Choose a theme (Escolher um tema)](/assets/images/help/pages/choose-a-theme.png)
4. No topo da página, clique no tema desejado e depois em **Selecionar tema**. ![Opções de tema e botão Select theme (Selecionar tema)](/assets/images/help/pages/select-theme.png)
5. Talvez seja necessário editar o arquivo *README.md* do site.
   - Para editá-lo mais tarde, clique em **Cancelar**. ![Link Cancel (Cancelar) ao editar um arquivo](/assets/images/help/pages/cancel-edit.png)
   - Para editar o arquivo agora, consulte "[Editando os arquivos](/repositories/working-with-files/managing-files/editing-files)".

O tema escolhido será aplicado automaticamente aos arquivos markdown no repositório. Para aplicar o tema a arquivos HTML no repositório, é preciso adicionar a página inicial YAML que especifica um layout para cada arquivo. Para obter mais informações, consulte "[Página inicial](https://jekyllrb.com/docs/front-matter/)" no site do Jekyll.

## Leia mais

- [Temas](https://jekyllrb.com/docs/themes/) no site do Jekyll
