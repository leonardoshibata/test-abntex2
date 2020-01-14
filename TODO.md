O Pandoc não conseguia converter corretamente um arquivo Markdown em um outro Latex no formato abntex2.

Isso porque ele não conseguia incluir corretamente a fonte das figuras. Em Latex, isso é feito com a macro \legend

Para resolver esse problema, outro desenvolvedor criou o programa em Ruby pandoc_abnt que é um filtro do Pandoc. Com esse filtro, e uma pequena mudança na maneira de escrever o código, é possível incluir a fonte (\legend) no arquivo.

---

Utilizando o descrito acima, eu consegui criar um markdown que é convertido corretamente para o Latex.

Posteriormente, criei também um arquivo R Markdown que obtém o mesmo resultado.


# TODO

* O R Markdown ou o Pandoc utiliza a macro \ref para as referências cruzadas. A classe abntex2 preconiza o uso do \autoref, que já inclui o tipo de referência (ex.: figura, tabela, etc.). Ver como conseguir incluir como \autoref e não ref.

