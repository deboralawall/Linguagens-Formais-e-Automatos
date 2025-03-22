Este programa simula o funcionamento de um Autômato Finito Determinístico (AFD), um modelo matemático usado para reconhecer padrões em sequências de símbolos. Na prática, ele funciona como um "verificador" que decide se uma determinada sequência de símbolos pertence ou não a um conjunto de palavras válidas. O programa começa pedindo ao usuário algumas informações para definir o autômato:
- O alfabeto, que são os símbolos permitidos (por exemplo, letras ou números).
- Os estados, que representam diferentes "situações" do sistema.
- O estado inicial, que é por onde a leitura da sequência começa.
- Os estados finais, que indicam se a sequência foi aceita ou não.
- As regras de transição, que dizem para qual estado o programa deve ir ao encontrar cada símbolo.

Depois que o autômato está configurado, o usuário pode inserir uma palavra (sequência de símbolos) para verificar se ela é válida. O programa lê essa sequência, seguindo as regras definidas. Se, ao final da leitura, ele estiver em um estado final, a palavra é aceita; caso contrário, ela é rejeitada.
Esse conceito é muito usado em computação para validar senhas e interpretar comandos, por exemplo. O trabalho faz parte da disciplina de Linguagens Formais e Autômatos, que estuda como máquinas podem reconhecer padrões e processar informações automaticamente.
