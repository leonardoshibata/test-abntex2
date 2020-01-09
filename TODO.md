O Pandoc não conseguia converter corretamente um arquivo Markdown em um outro Latex no formato abntex2.

Isso porque ele não conseguia incluir corretamente a fonte das figuras. Em Latex, isso é feito com a macro \legend

Para resolver esse problema, outro desenvolvedor criou o programa em Ruby pandoc_abnt que é um filtro do Pandoc. Com esse filtro, e uma pequena mudança na maneira de escrever o código, é possível incluir a fonte (\legend) no arquivo.

---

Utilizando o descrito acima, eu consegui criar um markdown que é convertido corretamente para o Latex.


# TODO

Tentar criar o mesmo arquivo utilizando o RStudio