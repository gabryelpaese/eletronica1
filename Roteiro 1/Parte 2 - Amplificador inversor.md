# Roteiro 1

## Parte 02: Amplificador Inversor

##### OBJETIVOS:

Medir o ganho de um amplificador inversor e verificar o efeito da saturação.

##### EXPERIMENTO:

Utilizando um Amp.OP. Lm324N e um TL082 monte dois amplificadores inversores utilize o resistor de realimentação com valor 20 kΩ e a resistência de entrada de 2kΩ. Utilize a alimentação simétrica de +/-12V. (limite a corrente em 0,05A)

##### PROCEDIMENTO:

1. Monte o circuito em uma matriz de contatos (protoboard) e antes de ligar as fontes chame o professor.
2. Configure no gerador de função um sinal senoidal com 0,5Vp @ 1 kHz e mostre o mesmo no canal 1 do osciloscópio.
3. Mostre a saída do amplificador no canal 2 do osciloscópio e chame o professor novamente e mostre os resultados.
4. Verifique o valor do ganho obtido;
5. Aumente o valor da tensão de entrada lentamente e verifique para qual valor da tensão de entrada ocorre à saturação do sinal.
6. Qual o valor da queda de tensão com relação a tensão de alimentação?
7. Não desmonte o circuito!!

### CALCULO PARA O GANHO DE TENSÃO (AV):

![calculoganhodetensao](/resources/imagens/relatorio1/parte2/calculoganhodetensao.jpeg)

### DE ACORDO COM O CIRCUITO AMPLIFICADOR INVERSOR O FORMATO DE ONDA DA TENSÃO DE ENTRADA:

![ondatensaoentrada](/resources/imagens/relatorio1/parte2/ondatensaoentrada.png)
![cursorentrada](/resources/imagens/relatorio1/parte2/cursorentrada.png)

### CIRCUITO AMPLIFICADOR INVERSOR COM O AMPOP LM324M

![circuitoinversorlm324m](/resources/imagens/relatorio1/parte2/circuitoinversorlm324m.png)

Tensão de saída do circuito:

![tensaosaidalm324m](/resources/imagens/relatorio1/parte2/tensaosaidalm324m.png)
![cursorsaidalm324m](/resources/imagens/relatorio1/parte2/cursorsaidalm324m.png)

Comparação entre tensão de entrada e saída do circuito:

![comparacaosaidaentradalm324m](/resources/imagens/relatorio1/parte2/comparacaosaidaentradalm324m.png)

### CIRCUITO AMPLIFICADOR INVERSOR COM O AMPOP TL082

![circuitoinversortl082](/resources/imagens/relatorio1/parte2/circuitoinversortl082.png)

Tensão de saída do circuito:

![tensaosaidatl082](/resources/imagens/relatorio1/parte2/tensaosaidatl082.png)

Comparação entre tensão de entrada e saída do circuito:

![comparacaosaidaentradatl082](/resources/imagens/relatorio1/parte2/comparacaosaidaentradatl082.png)

### RESULTADOS SIMULAÇÕES

Nos dois circuitos simulados anteriormente a amplitude do sinal da tensão de saída é de 5V e possuindo um ganho de -10.

### ANÁLISE DE SATURAÇÃO: CIRCUITO COM LM324N

Sinal de tensão de saída do circuito com 1,08V de amplitude na tensão de entrada (saturação positiva):

![saturacaolm324m](/resources/imagens/relatorio1/parte2/saturacaolm324m.png)
![2saturacaolm324m](/resources/imagens/relatorio1/parte2/2saturacaolm324m.png)
![cursorsaturacaolm324m1](/resources/imagens/relatorio1/parte2/cursorsaturacaolm324m1-2.png)

Na tensão 10,77V ocorreu saturação positiva tendo um valor de queda de tensão de 1,23V.


Sinal de tensão de saída do circuito com 1,14V de amplitude na tensão de entrada (saturação negativa e positiva):

![3saturacaolm324m](/resources/imagens/relatorio1/parte2/3saturacaolm324m.png)
![4saturacaolm324m](/resources/imagens/relatorio1/parte2/4saturacaolm324m.png)
![cursorsaturacaolm324m2](/resources/imagens/relatorio1/parte2/cursorsaturacaolm324m1-2.png)
![5saturacaolm324m](/resources/imagens/relatorio1/parte2/5saturacaolm324m.png)
![cursorsaturacaolm324m3](/resources/imagens/relatorio1/parte2/cursorsaturacaolm324m3.png)

Na tensão -11,32V ocorreu saturação negativa, tendo um valor de queda de tensão de -0,68V. Saturação positiva continua sendo 10,77V.

### ANÁLISE DE SATURAÇÃO: CIRCUITO COM TL082

Sinal de tensão de saída do circuito com 1,06V de amplitude na tensão de entrada (saturação positiva e negativa):

![saturacaotl082](/resources/imagens/relatorio1/parte2/saturacaotl082.png)
![2saturacaotl082](/resources/imagens/relatorio1/parte2/2saturacaotl082.png)
![cursorsaturacao](/resources/imagens/relatorio1/parte2/cursorsaturacaotl082.png)
![3saturacaotl082](/resources/imagens/relatorio1/parte2/3saturacaotl082.png)
![cursorsaturacao2](/resources/imagens/relatorio1/parte2/cursorsaturacaotl082-2.png)

Na tensão 10,38V ocorreu saturação positiva e na tensão de -10,38V ocorreu a saturação negativa, tendo um valor de queda de tensão de 1,62V e -1,62V.

### RESULTADOS SATURAÇÃO

Nessa simulação foi observado que o sinal de saída foi amplificado e invertido por causa do circuito do AmpOp Inversor. Também foi observado que o sinal de saída teve uma amplitude dez vezes maior do que o sinal de entrada e os ciclos positivos do sinal de saída coincidiam com os ciclos negativos do sinal de entrada.

Como foi esperado para essa simulação o sinal de tensão de saída dependente da tensão de alimentação que nesse caso foi de 12V. Testando os AmpOp LM324M observamos que o mesmo apresenta tensões de saturação diferentes (10,77V e -11,32V) e o AmpOp TL082 as tensões de saturação foram as mesmas (+-10,38V). Isso mostra que as especificações técnicas entre esses dois elementos são diferentes, possuindo diferenças na zona de saturação.
