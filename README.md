# CIRCUITOS-LOGICOS

RELATÓRIO  - AULA 2 (LOGIC GATES)

# INICIO:
Para realização do projeto com portas lógicas AND, OR, XOR, NAND e NOR, usaremos o código a seguir: 

![PreparacaoCodigo](https://github.com/yrflx/CIRCUITOS-LOGICOS/raw/master/Printscreens/preparacao2_codigo.png)

# CONFIGURAÇÃO - SOFTWARE QUARTUS II

Como no projeto anterior, é preciso configurar o projeto no software QuartusII para executar a tarefa com precisão.
Isso pode ser feito importanto as configurações do projeto anterior ou da seguinte forma:

1. Cria-se um novo projeto com nomes identicos aos utilizados em sala;
2. Seleciona-se o FPGA presenta na placa de família Cyclone II: EP2C5T144C6;
3. Adiciona-se o código VHDL, salvando-o no arquivo sillyfunction_gates.vhd
4. Em Settings->EDA Tools Settings->Simulation, define-se:

 a.Tool Name: ModelSim-Altera;
 
 b.Na aba EDA Netlist whiter setting, Output Directory:simulation/modelsim
 
 c.Na aba NativeLink Settings, inclui-se o testbench localizado em testbench_sillyfunction_gates/testbench_sillyfunction_gates.vhd


5. Criar um arquivo de nome example.tv contendo a tabela da verdade do circuito.


Trecho do arquivo testbench_sillyfunction_gates.vhd
![testbench_sillyfunction_gates](https://github.com/yrflx/CIRCUITOS-LOGICOS/raw/master/Printscreens/trecho_sillyfunction_gates.png)


# RESULTADOS

Clicando em Tools-> Netlist Views-> RTL Views, obtemos o circuito:

![rtl_gates](https://github.com/yrflx/CIRCUITOS-LOGICOS/raw/master/Printscreens/rtl_gates.png)

Realizando os testes com o ModelSim, clicando em RTL Simulation e Gate Level Simulation, obtemos os resultados:

RTL SIMULATION:

![rtl_simulation](https://github.com/yrflx/CIRCUITOS-LOGICOS/raw/master/Printscreens/rtl_simulation.png)

GATE LEVEL SIMULATION:

![level_gates_simulation](https://github.com/yrflx/CIRCUITOS-LOGICOS/raw/master/Printscreens/level_gates_simulation.png)


# OBSERVAÇÕES

Foi necessário, porém, fazer algumas alterações no clock, definindo-o da seguinte maneira:

![alteracoes](https://github.com/yrflx/CIRCUITOS-LOGICOS/raw/master/Printscreens/alteracoes.png)

