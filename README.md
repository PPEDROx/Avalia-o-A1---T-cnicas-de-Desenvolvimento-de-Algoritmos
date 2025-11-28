# Avalia-o-A1---T-cnicas-de-Desenvolvimento-de-Algoritmos
Atividade da professora Kadidja

📘 Avaliação A1 – Técnicas de Desenvolvimento de Algoritmos
Este repositório reúne quatro programas em Python desenvolvidos para a Avaliação A1 da
disciplina Técnicas de Desenvolvimento de Algoritmos.
Cada exercício aborda um dos conteúdos fundamentais da programação em Python:
Estruturas Condicionais, Estruturas de Repetição, Listas e Dicionários.
Os códigos seguem as orientações da avaliação:
✔ Simples
✔ Claros
✔ Bem comentados
✔ Organizados
✔ Fáceis de compreender
🧩 01. Estruturas Condicionais –
Verificação de Nota
Arquivo: 1-estruturas-condicionais/verificacao_nota.py
Este programa solicita a nota de um aluno e usa if, elif e else para verificar se ele foi
aprovado (nota ≥ 6).
Também verifica se a entrada é válida e se a nota está dentro do intervalo permitido (0 a
10).

📌 Código utilizado
# Programa para verificar se o aluno foi aprovado ou reprovado
# Entrada: usuário informa a nota
nota = input("Digite a nota do aluno (0 a 10): ")
# Verifica se a entrada é numérica
if nota.replace('.', '', 1).isdigit():
nota = float(nota) # Converte para número decimal
# Verifica se a nota está dentro do intervalo permitido
if 0 <= nota <= 10:
# Média de aprovação = 6
if nota >= 6:
print("Aprovado! A nota atingiu ou superou a média.")
elif nota < 6:
print("Reprovado! A nota ficou abaixo da média.")
else:
print("Nota inválida! Digite um número entre 0 e 10.")
else:
print("Entrada inválida! Digite apenas números.")

🔁 02. Estruturas de Repetição
Esta pasta contém dois programas que exibem os números pares de 1 a 100, utilizando os
dois principais laços de repetição: for e while.
2.1 – Usando FOR
Arquivo: pares_for.py
# Imprime números pares de 1 a 100 usando for
for numero in range(1, 101):
# Verifica se o número é par
if numero % 2 == 0:
print(numero)
2.2 – Usando WHILE
Arquivo: pares_while.py
# Imprime números pares de 1 a 100 usando while
numero = 1 # Começa no 1
while numero <= 100:
# Se o número for par, imprime
if numero % 2 == 0:
print(numero)
numero += 1 # Incrementa o contador

📝 03. Listas – Soma de Números
Arquivo: 3-listas/soma_numeros.py
Este programa permite que o usuário digite números livremente.
Cada número válido é adicionado a uma lista.
Quando o usuário digita "sair", o programa soma todos os valores e exibe o resultado.

📌 Código utilizado
# Programa para receber números, armazenar em uma lista e exibir a
soma final
lista_numeros = [] # Lista para guardar os números
while True:
valor = input("Digite um número (ou 'sair' para finalizar): ")
# Condição para encerrar o programa
if valor.lower() == "sair":
break
# Verifica se o valor digitado é um número
if valor.replace('.', '', 1).isdigit():
valor = float(valor) # Converte para número
lista_numeros.append(valor) # Adiciona à lista
else:
print("Valor inválido! Digite apenas números.")
# Soma todos os valores da lista
soma_total = sum(lista_numeros)
# Exibe a soma final
print("\nSoma total dos números digitados:", soma_total)
🛒 04. Dicionários – Cadastro de
Contatos
Arquivo: 4-dicionarios/cadastro_contatos.py
Neste programa, o usuário digita nomes e telefones para montar uma lista de contatos.
Cada contato é armazenado em um dicionário e depois exibido no final.

📌 Código utilizado
# Programa para cadastrar contatos usando dicionários
lista_contatos = [] # Lista que irá guardar cada dicionário de
contato
while True:
nome = input("Digite o nome do contato (ou 'sair' para
finalizar): ")
# Condição para encerrar o programa
if nome.lower() == "sair":
break
telefone = input("Digite o telefone do contato: ")
# Cria o dicionário com as informações do contato
contato = {
"nome": nome,
"telefone": telefone
}
# Adiciona o dicionário à lista
lista_contatos.append(contato)
# Exibe todos os contatos cadastrados
print("\nLista de contatos cadastrados:")
for pessoa in lista_contatos:
print(f"Nome: {pessoa['nome']} | Telefone:
{pessoa['telefone']}")

▶️ Como Executar os Programas
1. Instale o Python 3.
2. Abra o terminal na pasta do arquivo desejado.
3. Execute:
python nome_do_arquivo.py
Exemplo:
python verificacao_nota.py
