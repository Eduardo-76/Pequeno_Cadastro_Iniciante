import os

lista_pessoas = []

class Pessoa:
    def __init__(self, nome, idade):
        self.nome = nome
        self.idade = idade

    def ChamarPessoa(self):
        print(f'Nome: {self.nome} - Idade: {self.idade} anos')

def adicionar(nome, idade):
    nova_pessoa = Pessoa(nome, idade)
    lista_pessoas.append(nova_pessoa)

os.system('cls' if os.name == 'nt' else 'clear')

while True:
    try:
        print()
        nome = input('Digite seu nome: ').capitalize()

        while True:
            idade= input('Digite sua idade: ')
            if not idade.isdigit():
                print('Idade dever ser um número')
            else:
                idade = int(idade)
                break
                        
        os.system('cls' if os.name == 'nt' else 'clear')

        adicionar(nome, idade)

        print("Lista de pessoas:")
        for index, pessoa in enumerate(lista_pessoas, start=1):
            print(f'{index}. ', end='')
            pessoa.ChamarPessoa()


    except Exception as e:
        print(f'Ocorreu um erro {e}')
