Projeto de uma biblioteca em Python para realizar algumas ações com arquivos .txt





1° COMO INSTALAR A BIBLIOTECA ?

Para instalar a biblioteca no seu projeto Python, acesse o link: https://pypi.org/project/SearchInFile/1.0.0/ e siga as intruções.

Ou você pode simplesmente digitar <b>pip install SearchInFile</b> no seu terminal.

Após isso, a biblioteca será instalada no seu projeto.




2° COMO USAR A BIBLIOTECA ?

Para você usar a biblioteca, é necessário realizar o import dela.

Há diversas formas de realizar o import de uma biblioteca e usá-la, veja os exemplos a seguir:

______________________________________________________________________________________________________________________________________________________

         import search.find
  
         arquivo = search.find.MyFile('exemplo.txt')  # instancia a classe MyFile(), passando como parâmetro o nome do arquivo .txt
         
_______________________________________________________________________________________________________________________________________________________
  
  
        from search import find
  
        arquivo = find.MyFile('exemplo.txt')
  
_______________________________________________________________________________________________________________________________________________________
  
        from search.find import *
        
        arquivo = MyFile("exemplo.txt")



3° Métodos/funções disponíveis para você usar:
_______________________________________________________________________________________________________________________________________________________

        from search import find
  
        arquivo = find.MyFile('exemplo.txt')
        
        if arquivo.exist():
          print("A conexão com o arquivo foi realizada com sucesso.")
        else:
          print("A conexão com o arquivo não foi realizada.")
_______________________________________________________________________________________________________________________________________________________
      
      quantidadeDePalavras = arquivo.qtdPalavras()
      print(quantidadeDePalavras)
      
_______________________________________________________________________________________________________________________________________________________
      
      CincoMaioresPalavras = arquivo.maioresPalavras()
      print(CincoMaioresPalavras)
      
_______________________________________________________________________________________________________________________________________________________
      
      vogalMaisFrequente = arquivo.vogalFrequente()
      print(vogalMaisFrequente)
      
_______________________________________________________________________________________________________________________________________________________
      
      linhaComString = arquivo.findString("exemplo") # Essa função vai encontrar as linhas nas quais tem a string exemplo
      print(linhaComString)
      
_______________________________________________________________________________________________________________________________________________________
