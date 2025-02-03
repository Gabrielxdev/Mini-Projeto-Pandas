# Desafio - Mini Projeto de Análise de Dados

Vamos fazer um exercício completo de pandas para um miniprojeto de análise de dados.

Esse exercício vai nos obrigar a usar boa parte dos conhecimentos de pandas e até de outros módulos que já aprendemos ao longo do curso.

## O que temos?

Temos os dados de 2019 de uma empresa de prestação de serviços:

- CadastroFuncionarios
- CadastroClientes
- BaseServiçosPrestados

**Obs1:** Para ler arquivos csv, usamos o `read_csv`.  
**Obs2:** Para ler arquivos xlsx (arquivos em excel normais, que não são padrão csv), usamos o `read_excel`.

## O que queremos saber/fazer?

1. **Valor Total da Folha Salarial**  
   Qual foi o gasto total com salários de funcionários pela empresa?  
   **Sugestão:** Calcule o salário total de cada funcionário (salário + benefícios + impostos) e depois some todos os salários.

2. **Qual foi o faturamento da empresa?**  
   **Sugestão:** Calcule o faturamento total de cada serviço e depois some o faturamento de todos.

3. **Qual o % de funcionários que já fechou algum contrato?**  
   **Sugestão:** Na base de serviços temos o funcionário que fechou cada serviço. Mas nem todos os funcionários que a empresa tem já fecharam algum serviço.
   - Na base de funcionários temos uma lista com todos os funcionários.
   - Queremos calcular `Qtde_Funcionarios_Fecharam_Serviço / Qtde_Funcionários_Totais`.
   - Para calcular a quantidade de funcionários que fecharam algum serviço, use a base de serviços e conte quantos funcionários tem ali. Mas lembre-se, cada funcionário só pode ser contado uma única vez.

   **Dica:** Se você aplicar o método `.unique()` em uma variável que é apenas 1 coluna de um dataframe, ele vai excluir todos os valores duplicados daquela coluna.
   ```python
 
