# Desafio Técnico: Desenvolvimento Web Full-Stack

Olá, candidato(a)! Seja bem-vindo(a) ao nosso desafio técnico na **seer.**

Este teste foi desenhado para avaliar sua capacidade técnica em programação e resolução de problemas.

## Contexto do Projeto Fictício: "seer.dash"

O seer.dash é uma ferramenta web para análise simplificada de vendas. A ideia é que pequenos empreendedores possam fazer o upload de uma planilha de vendas (arquivo `.csv`) e obter insights e métricas importantes de forma rápida e visual, sem a necessidade de softwares de BI complexos.

A estrutura atual permite que um usuário faça o upload de um arquivo CSV e veja (ou deveria ver) um dashboard com algumas métricas.

## Sua Missão

Seu objetivo é duplo: primeiro, consertar os erros que estão impedindo o projeto de funcionar; segundo, enriquecer o projeto com uma nova funcionalidade.

### Parte 1: Correção de Erros e Ajustes

O projeto, como está, possui bugs que corrompem a análise. Esperamos que você:

1.  **Identifique e corrija os problemas distribuídos no repositório.**

Encare esse processo como um processo de testagem e revisão do projeto, analisando os fluxos e detalhes das páginas.

Ao identificar e resolver um problema, documente num relatório simplificado ([modelo disponível aqui](https://drive.google.com/drive/home)) como encontrou e resolveu cada erro. 

### Parte 2: Implementação de Nova Feature de Análise

Com a base do projeto funcionando, queremos que você implemente pelo menos uma das três features de análise abaixo. Escolha a que você achar mais interessante.

* **Opção A: Filtros por Período de Tempo**
    * Adicione ao dashboard a opção de filtrar toda a análise por um período: "Últimos 7 dias", "Este Mês" ou um intervalo de datas personalizado.

* **Opção B: Gráfico de Vendas por Categoria**
    * Adicione um novo gráfico (barras ou pizza) ao dashboard que mostra o faturamento total para cada categoria de produto.

* **Opção C: Tabela de "Top 5 Produtos"**
    * Crie uma tabela no dashboard que mostre os 5 produtos mais vendidos (em unidades) e, para cada um, a quantidade de vendas e o faturamento total.

## Como Entregar

1.  Faça um fork deste repositório.
2.  Faça commits com mensagens claras à medida que avança.
3.  Ao finalizar, preencha completamente o modelo de relatório disponibilizado.
4.  A entrega deve ser um .zip com o relatório, pasta com um código finalizado e um vídeo breve de até 2 minutos sobre o trabalho realizado (o vídeo é opcional). 

## O Relatório

No seu relatório, você irá descrever de forma concisa (seguindo o modelo):

* **Diagnóstico:** Quais foram os erros que você encontrou e qual era a causa raiz de cada um.
* **Solução:** Como você resolveu cada um dos problemas.
* **Feature Escolhida:** Qual feature você implementou e uma breve explicação dos passos técnicos que você tomou.
* **(Opcional) Considerações Adicionais:** Se tiver qualquer outra sugestão de melhoria, sinta-se à vontade para compartilhar.

## Configuração do Ambiente

Para rodar o projeto, você precisará de Python e Pip. O projeto usa a biblioteca Pandas para manipulação de dados.

**Formato do CSV esperado:** O arquivo `vendas.csv` possui as colunas: `produto,categoria,preco,data` (data no formato `YYYY-MM-DD`).

```bash
# 1. Clone o repositório e entre na pasta
git clone [URL_DO_SEU_REPOSITORIO]
cd [NOME_DA_PASTA]

# 2. Crie e ative um ambiente virtual
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate

# 3. Instale as dependências
pip install -r requirements.txt

# 4. Rode as migrações e crie um superusuário
python manage.py migrate
python manage.py createsuperuser

# 5. Inicie o servidor
python manage.py runserver
```

Boa sorte! Estamos muito interessados em ver como você aborda o desafio. 
