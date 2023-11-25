


# Diagrama

+-------------------------------+   +-------------------------------------------+
|      Main                     |   |   ModelTermo                              |
+-------------------------------+   +-------------------------------------------+
| - model: ModelTermo           |   | - palavraSorteada: String                 |
| - ctrl: Controller            |   | - palavraArray: String[]                  |
| - view: JFrameTermo           |   | - letraDigitada: String                   |  
+-------------------------------+   | - indiceLetra: int                        |
| + main(args: String[]): void  |   | - isPalavraCorreta: int                   |  
+-------------------------------+   | + ModelTermo()                            |
                                    | + sorteiaPalavra(): String                |
                                    | + verificaPalavra(linha: int): void       |
                                    | + verificaFinalizado(linha: int): boolean |
+-------------------------------+   | + isGanhou(): boolean                     |
|   JFrameTermo                 |   | + temCaractereRepetido(): boolean         |
+-------------------------------+   +-------------------------------------------+
| - panelBarra: JPanel          |   +-------------------------------------------+
| - panelCampo: JPanel          |   |   Controller                               |
| - panelBotao: JPanel          |   +--------------------------------------------+
| - labelNomeBarra: JLabel      |   | - model: ModelTermo                        |
| - btnEnter: JButton           |   +--------------------------------------------+
| - matriz: JTextFieldTermo[][] |   | + Controller(model: ModelTermo)            |
| - ctrl: Controller            |   | + verificaPalavra(linha: int): void        |
| - espacoLateral: int          |   | + verificaFinalizado(linha: int): boolean  |
| - fonte: Font                 |   | + isGanhou(): boolean                      |
| - fonteBtn: Font              |   +--------------------------------------------+
| - corFundo: Color             |
| - corBtn: Color               |
| - contadorLinha: int          |
| - teclaBackSpacePress: boolean|
+-------------------------------+

+-------------------------------------------+       +--------------------------------------+
| JTextFieldTermo                           |       | FiltrarPalavrasPorQuantidadeDeLetras |
+-------------------------------------------+       +--------------------------------------+
| - corFundo: Color                         |       | - nomeArquivoEntrada: String         |
| - corBordaPadrao: Color                   |       | - nomeArquivoSaida: String           |
| - corBordaFoco: Color                     |       +--------------------------------------+
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

