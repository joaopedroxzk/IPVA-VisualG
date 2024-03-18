# IPVA-VisualG


Var
// Seção de Declarações das variáveis

   anofab: inteiro
   IPVA: real
   valor: real
   anoatual: inteiro
   idade: inteiro
   modelo:inteiro

Inicio
// Seção de Comandos, procedimento, funções, operadores, etc...

   ESCREVAL ("Qual o ano atual?")
   leia (anoatual)
   ESCREVAL ("Qual o ano de fabricação do seu carro?")
   leia (anofab)
   idade <- anoatual - anofab
   
   Se (idade > 19)  entao
   Escreval ("Você não paga IPVA, pois seu carro tem mais de 20 anos.")
   Senao
   ESCREVAL ("QUAL O SEU VEICULO?")
   ESCREVAL ("1= CARRO FLEX")
   ESCREVAL ("2= CARRO ELÉTRICO")
   ESCREVAL ("3= CARRO GNV")
   ESCREVAL ("4= MOTO")
   LEIA (modelo)
   fimse
   Se (modelo < 1)  entao
   Escreval ("Obrigado por participar da pesquisa")
   senao
   SE (modelo < 2) entao
   Escreval ("Qual o valor do seu carro?")
   Leia (valor)
   Escreval ("O valor do seu IPVA é de R$", valor * 0.04)
   senao
        SE (modelo < 3) entao
        Escreval ("Qual o valor do seu carro?")
        Leia (valor)
        Escreval ("O valor do seu IPVA é de R$", valor * 0.005)
        Senao
             SE (modelo < 4) entao
             Escreval ("Qual o valor do seu carro?")
             Leia (valor)
             Escreval ("O valor do seu IPVA é de R$", valor * 0.015)
             senao
                  SE (modelo < 5) entao
                  Escreval ("Qual o valor da sua moto?")
                  Leia (valor)
                  Escreval ("O valor do seu IPVA é de R$", valor * 0.02)
                  Senao
                       Se (modelo > 4) entao
                       Escreval "Modelo inexistente Tente Novamente:"
                       Leia (modelo)
                       fimse
                  fimse
             fimse
        fimse
   fimse
   fimse

Fimalgoritmo
