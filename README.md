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

1. Negrito - \*\*This is bold text\*\* - **This is bold text**
2. Negrito - \_\_This is bold text\_\_ - __This is bold text__
3. Itálico - \*This text is italicized\* - *This text is italicized*
4. Itálico - \_This text is italicized\_ - _This text is italicized_
5. Tachado - \~\~This was mistaken text\~\~ - ~~Este texto contém um error~~

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
