# EXAME FINAL LPAA

### INSTRUÇÕES

- Junto com esta atividade serão fornecidos arquivos de dados (cotações de ativos), que você usará para desenvolver a atividade. Você deverá usar o preço de fechamento para todos eles.

1. Faça o processamento dos arquivos fornecidos. Identifique se há dados faltantes, ou dados discrepantes. Analise cada arquivo como uma série de dados, e resolva eventuais problemas que aparecerem.

Observação: Como a negociação do Bitcoin não para de funcionar até nos finais de semana, você terá mais pontos no arquivo. As outras demais cotações são para ativos que só funcionam em dias úteis. Portanto use apenas dados para dias úteis. Priorize também a menor série (série mais jovem), ou seja, se outras forem maiores, você precisa nivelá-las pela menor, e alinhá-las de acordo com as datas. Após todo o processamento, organize-os em um DataFrame.

2. Para compara todas as séries a partir da data D0, pode utilizar a seguinte equação:
```
mydata_norm = (mydata/mydata.iloc[0])*100
```
3. Para calcular  o retorno diário dos ativos utilizando o seguinte comando. Use a cotação de fechamento
```
returns = (mydata/mydata.shift(1))-1
```
4. Calcule os seguintes parâmetros relacionados a cada ativo

4.1. média de retornos anual;

4.2. Variância anual;

4.3. desvio padrão anual;

4.4. módulo da amplitude entre máxima e mínima (diária e anual) módulo da amplitude entre abertura e fechamento (diária e anual);

4.5. média de variação entre máxima e mínima diária;

4.6. média de variação entre abertura e fechamento diária;

4.7. retorno acumulado total;

4.8. retorno acumulado nos últimos 12 meses; 

4.9. retorno ano a ano;

4.10. Correlação entre os ativos;

4.11. Correlação com uma janela móvel de 45 dias;

5. Calcule quantas vezes houve Gap (espaço), que é o espaço entre o fechamento do dia anterior e a abertura do dia posterior. Determine de quanto foi esses gaps (o módulo) e a média deles por ano.

6. Calcule quantas vezes houve fechamento de Gap, ou seja, se houver gap, o fechamento do dia posterior tem que acontecer acima ou abaixo do dia anterior.

7. Apresente gráficos com subplots das correlações entre os ativos.

8. Apresente um gráfico normalizado comparando todos os ativos e usando toda a série. Faça também um gráfico do drawdown de toda a série para cada ativo. Coloque como subplots (acima os gráficos normalizados, abaixo os de drawdown).

9. Apresente um gráfico normalizado comparando todos os ativos, porém separado por anos. Ou seja, o ponto zero da série será o primeiro ponto daquele ano. Apresente também como suplot o drawdown de cada ano para cada ativo para cada janela de ano.

10. Apresente um gráfico com o histograma dos retornos de todos os ativos. Use um binning adequado.

Faça uma tabela comparativa entre os ativos designados para você, onde deverão constar além dos parâmetros estatísticos:

i) drawdown máximo por ano;

ii) retorno por ano;

iii) desvio padrão por ano;

iv) drawdown máximo da série histórica.


### Os datasets estão na pasta "datasets_exame_final", disponíveis em:

pasta: https://canvas.instructure.com/courses/7864832/files/folder/dataset_exame_final

BTC: https://canvas.instructure.com/files/248635691/download?download_frd=1

ETH: https://canvas.instructure.com/files/248635682/download?download_frd=1

RUSSEL 2000: https://canvas.instructure.com/files/248636557/download?download_frd=1

Acesso em 21/03/2024.

Leandro: BTC/USD, ETH/USD e Russel 2000
