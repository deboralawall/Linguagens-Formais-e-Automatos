#Automato Finito Determinístico
#M = {alfabeto, estados, funcao, estadoInicial, estadoFinal} -> quintupla

#Definição:
alfabeto = []
estados = []
validacao = {}
estadoInicial = ""
estadosFinais = []

#Dados:
#Usamos o split pq ele transforma a entrada em uma lista
print("Digite o alfabeto: ", end="")
alfabeto = input().split()

print("Digite os estados: ", end="")
estados = input().split()

print("Digite o estado inicial: ", end="")
estadoInicial = input()

print("Digite os estados finais: ", end="")
estadosFinais = input().split()

#Cria o automato, funcao
print("Digite as transições do automato: ")
for estado in estados :
    for simbolo in alfabeto :
        print(f"\t {simbolo}")
        print(f"{estado}\t ---> \t", end="")
        proximoestado = input()

#Verifica se o simbolo esta na linguagem, caso nao esteja coloca como vazio 
        if proximoestado == "." :
            print("Não reconhece a linguagem", end="")
            validacao[(estado, simbolo)] = None
        else :
            validacao[(estado, simbolo)] = proximoestado

#Reconhecendo linguagens
print("Digite a linguagem a ser reconhecida")
linguagem = input()

#Recebe o estado inicial da linguagem 
estado_atual = estadoInicial 

#Passa por todos os simbolos na linguagem e atualiza o estado_atual 
for simbolo in linguagem :
    estado_atual = validacao[(estado_atual, simbolo)]
    
    #Verifica se não é um síbolo que foi setado como vazio por nao fazer parte do alfabeto
    if estado_atual == None :
        print("Linguagem não reconhecida")
        break

#Caso o simbolo chegue ao fim da fita reconhece a linguagem 
if estado_atual in estadosFinais :
    print("Linguagem Reconhecida")
else :
    print("Linguagem não reconhecida")
    
