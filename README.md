# Sintaxe básica de gravação e formatação no GitHub

## Títulos

Para criar um título, adicione de um a seis símbolos `#` antes do texto do título. O número 
de `#` que você usará para determinar o tamanho do título.
```md
# The largest heading 
## The second largest heading
###### The smallest heading
```

# The largest heading 
## The second largest heading
###### The smallest heading




Ao usar dois ou mais cabeçalhos, o GitHub gera automaticamente uma tabela de conteúdo que você pode acessar clicando em `📄` dentro do cabeçalho do arquivo. Cada título do cabeçalho está listado na tabela de conteúdo e você pode clicar em um título para acessar a seção selecionada.

![](https://docs.github.com/assets/cb-47415/images/help/repository/headings_toc.png)

## Estilo do texto

Você pode indicar ênfase com texto em negrito, itálico, tachado, subscrito ou sobrescrito em campos de comentários e arquivos `.md`.

- Negrito - \*\*This is bold text\*\* - **This is bold text**
* Negrito - \_\_This is bold text\_\_ - __This is bold text__
+ Itálico - \*This text is italicized\* - *This text is italicized*
- Itálico - \_This text is italicized\_ - _This text is italicized_
* Tachado - \~\~This was mistaken text\~\~ - ~~Este texto contém um error~~

## Texto de referência

Você pode citar um texto com `>`.

```md
Text that is not a quote
 > Text that is a quote
```

Text that is not a quote
 > Text that is a quote



## Citar código

Você pode chamar código ou um comando em uma frase com aspas simples. O texto entre as aspas não será formatado. Você também pode pressionar o atalho de teclado `Comando+E (Mac)` ou `Ctrl+E (Windows/Linux)` para inserir os acentos graves para um bloco de código dentro de uma linha de Markdown.

```md
Use `git status` to list all new or modified files that haven't yet been committed.
```

Use `git status` to list all new or modified files that haven't yet been committed.


Para formatar código ou texto no próprio bloco distinto, use aspas triplas.

```md
Some basic Git commands are:
\```
git status
git add
git commit
\```
```

Some basic Git commands are:
```
git status
git add
git commit
```
 

## Modelos de cores com suporte

Em problemas, solicitações de pull e discussões, você pode chamar cores dentro de uma frase usando aspas invertidas. Um modelo de cor com suporte em aspas invertidas exibirá uma visualização da cor.

```md
The background color should be `#ffffff` for light mode and `#0d1117` for dark mode.
```
The background color should be `#ffffff` for light mode and `#0d1117` for dark mode.



## Links
Você pode criar um link embutido colocando o texto do link entre colchetes `[ ]` e colocando a URL entre parênteses `( )`. Você também pode usar o atalho de teclado `Command+K` para criar um link. Depois de selecionar o texto, você poderá colar uma URL da área de transferência para criar um link automaticamente com base na seleção.

Você também pode criar um **hiperlink Markdown** realçando o texto e usando o atalho de teclado `Command+V`. Se você quiser substituir o texto pelo link, use o atalho de teclado `Command+Shift+V`.

```md
This site was built using [GitHub Pages](https://pages.github.com/).
```

This site was built using [GitHub Pages](https://pages.github.com/).

## Links de seleção

Você pode vincular diretamente a uma seção de um arquivo interpretado, passando o mouse sobre o título da seção para expor o link:

![](https://docs.github.com/assets/cb-25655/images/help/repository/readme-links.png)

## Links relativos

É possível definir links relativos e caminhos de imagens em seus arquivos representados para ajudar os leitores a acessar outros arquivos no repositório.

Um link relativo é um link que é relativo ao arquivo atual. Por exemplo, se você tiver um arquivo *LEIAME* na raiz do repositório e tiver outro arquivo em *docs/CONTRIBUTING.md*, o link relativo para *CONTRIBUTING.md* no *LEIAME* poderá ter esta aparência:

```md
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```

GitHub transformará automaticamente o seu link relativo ou caminho da imagem baseado em qualquer branch em que você estiver no momento para que o link ou caminho sempre funcione. O caminho do link será relativo ao arquivo atual. Links que começam com */* serão relativos à raiz do repositório. Você pode usar todos os operandos de link relativos, como *./* e *../*.

Os links relativos são mais fáceis para usuários que clonam o seu repositório. Os links absolutos podem não funcionar em clones do seu repositório - recomendamos usar links relativos para referir-se a outros arquivos no seu repositório.


## Imagens

Você pode exibir uma imagem adicionando `!` e colocando o texto Alt entre `[ ]`. Em seguida, coloque o link da imagem entre parênteses `()`.

```md
![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)
```
![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)



## Especificando um tema para o qual uma imagem será exibida

Você pode especificar o tema para o qual uma imagem é exibida no Markdown usando o elemento HTML `<picture>` em combinação com o recurso de mídia _prefers-color-scheme_. Nós distinguimos entre os modos de cores claro e escuro. Portanto, há duas opções disponíveis. Você pode usar essas opções para exibir imagens otimizadas para fundos escuros ou claros. Isso é particularmente útil para imagens PNG transparentes.

Por exemplo, o seguinte código exibe uma imagem de sol para temas claros e uma lua para temas escuros:

```md
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>
```

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>

O método antigo de especificar imagens com base no tema, usando um fragmento acrescentado à URL (**#gh-dark-mode-only** ou **#gh-light-mode-only**), foi preterido e será removido em favor do novo método descrito acima.


## Listas

Você pode criar uma lista não ordenada precedendo uma ou mais linhas de texto com `-`, `*` ou `+`.

```md
- George Washington
* John Adams
+ Thomas Jefferson
```

- George Washington
* John Adams
+ Thomas Jefferson

Para ordenar a lista, coloque um número na frente de cada linha.

```md
1. James Madison
2. James Monroe
3. John Quincy Adams
```

1. James Madison
2. James Monroe
3. John Quincy Adams


# Listas aninhadas

Você pode criar uma lista aninhada recuando um ou mais itens da lista abaixo de outro item.

Para criar uma lista aninhada usando o editor Web do GitHub ou um editor de texto que use uma fonte monoespaçada, como o Visual Studio Code, você pode alinhar a lista visualmente. Digite caracteres de espaço na frente do item de lista aninhada até que o caractere de marcador da lista `(- ou *)` fique diretamente abaixo do primeiro caractere do texto no item acima dele.

```md
1. First list item
   - First nested list item
     - Second nested list item
```

1. First list item
   - First nested list item
     - Second nested list item


Para criar uma lista aninhada no editor de comentários do GitHub, que não usa uma fonte monoespaçada, você pode observar o item da lista logo acima da lista aninhada e contar o número de caracteres que aparecem antes do conteúdo do item. Em seguida, digite esse número de caracteres de espaço na fonte do item da linha aninhada.

Neste exemplo, você pode adicionar um item de lista aninhada no item de _lista 100_. First list item recuando o item de lista aninhada no mínimo cinco espaços, pois há cinco caracteres *(100. )* antes de First list item.

```md
100. First list item
     - First nested list item
```

100. First list item
     - First nested list item


Você pode criar vários níveis de listas aninhadas usando o mesmo método. Por exemplo, como o primeiro item de lista aninhada tem sete caracteres _(␣␣␣␣␣-␣)_ antes do conteúdo da lista aninhada First nested list item, você precisa recuar o segundo item de lista aninhada com sete espaços.

```md
100. First list item
     - First nested list item
       - Second nested list item
```

100. First list item
     - First nested list item
       - Second nested list item



## Listas de tarefas

Para criar uma lista de tarefas, coloque um hífen e um espaço seguidos de `[ ]` antes dos itens de lista. Para marcar uma tarefa como concluída, use `[x]`.

```md
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
```
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:

Se a descrição de um item da lista de tarefas começar com parênteses, você precisará fazer escape dele com `\`:

```md
- [ ] \(Optional) Open a followup issue
```


## Mencionar pessoas e equipes

Você pode mencionar uma pessoa ou uma equipe no GitHub digitando `@` mais seu nome de usuário ou o nome da equipe. Isto desencadeará uma notificação e chamará a sua atenção para a conversa. As pessoas também receberão uma notificação se você editar um comentário para mencionar o respectivo nome de usuário ou da equipe. Para obter mais informações sobre as notificações, confira *“Sobre notificações.”*

```md
@github/support What do you think about these updates?
```
@superkake What do you think about these updates?

Quando você menciona uma equipe principal, os integrantes de suas equipes secundárias também recebem notificações, simplificando a comunicação com vários grupos de pessoas. Para obter mais informações, confira *"Sobre as equipes"*.

Se você digitar um símbolo `@`, uma lista de pessoas ou de equipes em um projeto será exibida. A lista é filtrada à medida que você digita. Portanto, assim que você achar o nome da pessoa ou da equipe que está procurando, use as teclas de seta para selecioná-lo e pressione tab ou enter para completar o nome. Para equipes, insira o `@organization/team-name` e todos os membros dessa equipe serão inscritos na conversa.

Os resultados do preenchimento automático são restritos aos colaboradores do repositório e qualquer outro participante no thread.

## Alerts
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advices about risks or negative outcomes of certain actions.
