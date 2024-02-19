# TratamentoerroProz

nome = input("Digite o seu nome: ")

while True:
    try:      
        ano = int(input("Digite o ano de seu nascimento (entre 1922 e 2021): "))
        if (1922 <= ano <= 2021):
            idade = 2022 - ano
            print("Nome:", nome, "Idade:", idade)
            break
        else:
            print("Ano fora do intervalo especificado. Por favor, digite novamente.")
    except ValueError:
        print("Valor inválido. Por favor, digite um ano válido.")
