# Sobre os arquivos

O arquivo de dados é: Base_mapeamento_cidades_mais_de_100_mil_habitantes.csv

E o principal arquivo de processamento: relatorio1.py

Os arquivos preprocessamento.py, distribuicao_geografica.py, formatos_publicacao.py, dominios.py e acervo_historico.py são auxiliares (pacotes de funções) para relatorio1.py

# Como executar

Com o arquivo de dados nessa mesma pasta, o ambiente virtual ativado e com a dependências do repositório já baixadas, execute:

```sh
python relatorio_1.py
```

Ao final da execução, diversos arquivos .csv existirão dentro da pasta "resultados", referentes às informações utilizadas no relatório 1 do Censo de Diários Oficiais do Querido Diário.

# Observações metodológicas

No arquivo preprocessamento.py, há uma função (substitui_sem_diario()) que classifica as cidades de Viamão (RS), Rio Grande (RS), Tubarão (SC) e Tatuí (SP) como "Indefinido" para as variáveis associadas ao Diário Oficial. O motivo da ação é que essas cidades publicam seus atos pulverizadamente, não se adequando ao conceito do documento de Diário Oficial que consideramos para o censo.
