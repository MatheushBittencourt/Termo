


# Diagrama

+-------------------------------------------+
|   ModelTermo                              |
+-------------------------------------------+
| - palavraSorteada: String                 |
| - palavraArray: String[]                  |
| - letraDigitada: String                   |  
| - indiceLetra: int                        |
| - isPalavraCorreta: int                   |  
| + ModelTermo()                            |
| + sorteiaPalavra(): String                |
+ verificaPalavra(linha: int): void         |
+ verificaFinalizado(linha: int): boolean   |
| + isGanhou(): boolean                     |
| + temCaractereRepetido(): boolean         |
+-------------------------------------------+




+-------------------------------+
|      Main                     |
+-------------------------------+
| - model: ModelTermo           |
| - ctrl: Controller            |
| - view: JFrameTermo           |  
+-------------------------------+
| + main(args: String[]): void  |  
+-------------------------------+

+-------------------------------+
|   JFrameTermo                 |
+-------------------------------+
| - panelBarra: JPanel          |
| - panelCampo: JPanel          |
| - panelBotao: JPanel          |
| - labelNomeBarra: JLabel      |
| - btnEnter: JButton           |
| - matriz: JTextFieldTermo[][] |
| - ctrl: Controller            |
| - espacoLateral: int          |
| - fonte: Font                 |
| - fonteBtn: Font              |
| - corFundo: Color             |
| - corBtn: Color               |
| - contadorLinha: int          |
| - teclaBackSpacePress: boolean|
+-------------------------------+

+-------------------------------------------+
|   Controller                               |
+--------------------------------------------+
| - model: ModelTermo                        |
+--------------------------------------------+
| + Controller(model: ModelTermo)            |
| + verificaPalavra(linha: int): void        |
| + verificaFinalizado(linha: int): boolean  |
| + isGanhou(): boolean                      |
+--------------------------------------------+


+--------------------------------------+
| FiltrarPalavrasPorQuantidadeDeLetras |
+--------------------------------------+
| - nomeArquivoEntrada: String         |
| - nomeArquivoSaida: String           |
+--------------------------------------+

+-------------------------------------------+
| JTextFieldTermo                           |
+-------------------------------------------+
| - corFundo: Color                         |
| - corBordaPadrao: Color                   |
| - corBordaFoco: Color                     |
| - corCerta: Color                         |
| - corLugarErrado: Color                   |
| - corErrado: Color                        |
| - linha: int                              |
| - coluna: int                             |
| - letra: String                           |
+-------------------------------------------+
| + JTextFieldTermo()                       |
| + verificarLetra(n: int): void            |
| + setPosicao(linha:int, coluna: int):void |
+-------------------------------------------+

