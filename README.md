# Projeto-Poo
#2º Informática Matutino
#Disciplina:Programação Orientada a Objetos 
#integrantes: Amanda Vitória e Kevelyn Maria

main.py
from Pessoa import Pessoa
from Pizza import Pizza
from Pedido import Pedido

pessoa=Pessoa()

pizza= Pizza()

pedido=Pedido()


pedido.valor(pizza)

pedido.comprar(pessoa,pizza)

Pedido.py
class Pedido:
  def __init__(self):
    self._pessoa=None
    self._pizza=None

  def valor(self,pizza):
    self._pizza=pizza

  def comprar(self,pessoa,pizza):
    self._pessoa=pessoa
    self._pizza=pizza
    
   Pessoa.py
    def leiaint(msg):
  while True:
    try:
      n=int(input(msg))
    except (ValueError, TypeError):
      print("Por favor apenas números!")
      continue
    else:
      return n 

def nop (msg):
  while True:
    try:
      nome = input(msg)

      for letra in nome:
          if letra.isdigit():
              raise ValueError

    except ValueError: 
      print("O nome não deve ter número!")
      continue
    else:
      return nome

class Pessoa:
    def __init__(self):
        self.id_pessoa = leiaint("Insira o Id_pessoa:")
        self._nome =nop("Insira seu nome:")
        self._data_nasc =input("Insira a data de nascimento:")
        self._end= input("Insira o seu endereço:")
        self._telefone =leiaint("Insira o telefone:")
       
   Pizza.py 
 class Pizza:
  def __init__(self):
    self.tamanho=(pessoa['tamanho'])
    self.sabor= (pessoa['sabor'])

restau=list()
pessoa= dict()
while True:
  pessoa.clear()
  pessoa['Pedido-->']=input("***FAÇA SEU PEDIDO***")
  pessoa['sabor']=str(input("Escolha até dois sabores:"))
  while True:
    pessoa['tamanho']=str(input("Escolha um tamanho G/P/M: "))
    if pessoa ['tamanho'] in 'GPM':
      break
    print ("Por favor digite apenas G, P ou M!")
  restau.append(pessoa.copy())
  while True:
    per=str(input("Quer fazer mais um pedido?"))
    if per in 'SN':
      break
    print ("Responda apenas S ou N!")
  if per=='N':
    break 
print(restau)   
