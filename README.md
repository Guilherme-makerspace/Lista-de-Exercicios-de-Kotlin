# ***Lista-de-Exercicios-de-Kotlin***

## ***Questão 1***

Construa um programa que calcule o IMC. Índice de Massa Corporal e ainda exiba a  classificação de acordo com a tabela de classificação da OMS. 
  Classificação do IMC: 
- Menor que 18,5 - Abaixo do peso 
- Entre 18,5 e 24,9 - Peso normal 
- Entre 25 e 29,9 - Sobrepeso (acima do peso desejado) 
- Igual ou acima de 30 – Obesidade

### *Resolução*
```kotlin
import kotlin.math.pow
fun main() {
    println("Digite seu peso em kilos")
    val peso = readln().toDouble()
    println("Digite sua altura em metros")
    val altura = readln().toDouble()
    
    var imc = peso / altura.pow(2)
    
    if(imc < 18.5){
        println("Abaixo do peso")
    } else if(imc >= 18.5 && imc < 24.9){
        println("Peso normal")
    } else if(imc >= 24.9 && imc < 29.9){
        println("Sobrepeso")
    } else {
        println("Obesidade")
    }
    println(imc)
}
```

## ***Questão 2***
 A construtora Prudente S.A atua no segmento de construção civil, e recentemente  fechou contrato para construção de casas para um novo lançamento que terá  diversas plantas diferentes. Para auxiliar no cálculo de despesas e mão de obra, construa um programa que: 
- A. Calcule a área do terreno 
- B. Calcule quantos profissionais serão necessários na obra a partir da tabela. A  construtora só realiza contrato a partir de 10M². 
Aqui está o código Markdown prontinho para você copiar e colar onde precisar. Coloquei tudo dentro deste bloco de código para facilitar o processo:

### Tabela de Dimensionamento de Pessoal
| Profissional | Critério de Contratação |
| :--- | :--- |
| 1 Metre de obra | A partir de 10 m² |
| 2 Serventes | A cada 10 m² |
| 1 Engenheiro | A cada 100 m² |

---

- C. Calcule ainda o valor da obra a partir da tabela abaixo: 

### Valores da Obra por Item
| Descrição | Valor |
| :--- | :--- |
| A cada 10 m² | R$ 4.500,00 |
| 1 quarto sem suíte | Acrescentar R$ 12.000,00 |
| 1 área de serviço | Acrescentar R$ 15.000,00 |
| 1 piscina | Acrescentar R$ 27.550,00 |
| 1 quarto com suíte | Acrescentar R$ 17.000,00 |
| 1 banheiro | Acrescentar R$ 5.000,00 |

---


- D. Calcule o valor a ser pago com mão de obra de acordo com a tabela 


### Valor da Mão de Obra
| Profissional | Valor Unitário |
| :--- | :--- |
| 1 Metre de obra | R$ 3.500,00 |
| 1 Serventes | R$ 1.900,00 |
| 1 Engenheiro | R$ 11.000,00 |


Calcule o valor total da obra e exiba o relatório. 
- 1. Subtotal por item (Conforme tabela) 
- 2. Total da obra (Sem mão de obra) 
- 3. Total da obra (Com mão de obra) 
- 4. O lucro da empresa é de 25% sobre o total da obra, calcule quanto a  empresa receberá ao final e quanto ela deverá destinar ao custo da  obra considerando o desconto da folha de pagamento.
