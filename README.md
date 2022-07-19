# Soma-Matriz

Exercício 3: Soma Matriz
Gabarito do Exercício 3
Exercício 3: Faça uma função que receba como parâmetro uma matriz A(5,5) preenchida com números reais e retorne a soma de seus elementos.

programa
{
    funcao inicio()
    {
        real matriz[5][5]
        escreva("Informe os números: \n")
        para(inteiro i=0; i<5; i++){
            para(inteiro j=0; j<5; j++){
                escreva("Posição [",(i+1),"][",(j+1),"]: ")
                leia(matriz[i][j])
            }
        }
        escreva("A soma é: ",somaMatriz(matriz))
    }

    funcao real somaMatriz(inteiro mat[][])
    {
        real soma = 0
        para(inteiro i=0; i<5; i++){
            para(inteiro j=0; j<5; j++){
                soma = soma + mat[i][j]
            }
        }
        retorne soma
    }

}
