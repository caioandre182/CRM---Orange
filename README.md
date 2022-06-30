<h1>Projeto - CRM (Orange)</h1>
<br>
<img src='https://github.com/caioandre182/CRM---Orange/blob/main/CRM/207884-como-usar-o-crm-na-gestao-de-relacionamento-com-o-cliente.jpg' widht=300 height=300>
<br>
<h2>Objetivo</h2>

<p>
  CRM (<i>Customer Relationship Management</i>) ou gestão de relacionamento com o cliente, é uma estratégia essencial para qualquer empresa que deseja melhorar suas receitas e lucratividade, reduzir custos e aumentar a fidelidade do cliente.
</p>
<p>
  Com uma base de dados real, da <i>Orange</i>, uma empresa francesa de telecomunicações, utilizada em uma competição da <a href='https://kdd.org/kdd-cup/view/kdd-cup-2009'>KDD Cup 2009</a>, iremos prever:
  <ul>
    <li>A propensão dos clientes a mudar de provedor - <code>Churn</code></li>
    <li>A compra de novos produtos ou serviços - <code>Appentency</code></li>
    <li>E comprar upgrades ou add-ons propostos para tornar a venda mais lucrativa - <code>Upselling</code></li>
  </ul>
</p>

<p>
  A maneira mais prática de construir um conhecimento sobre o cliente é produzir pontuações, nosso modelo através de variáveis de entrada, classificará dicotomicamente se um cliente irá ou não realizar aquela ação (churn, appentency, upselling). Quanto maior a pontuação, melhor o desempenho do nosso modelo.
</p>
<br>
<h2>Informações Importantes</h2>

<p>
  Devido a GDPR (<i>Gerenal Data Protection Regulation</i>), os dados, afim de manter a descrição dos clientes são mascarados, por tanto não sabemos o que cada variável significa, apenas nos basearemos na natureza das mesmas.
</p>
<br>
<h2>Tratamento e Seleção de Variáveis</h2>

<p>
  No notebook <a href='https://github.com/caioandre182/CRM---Orange/blob/main/CRM/CRM%20%20-%20Tratamento%20das%20Vari%C3%A1veis.ipynb'>CRM - Tratamento das Variáveis</a> além do tratamento das variáveis, faremos a seleção delas, e para cada variável target (churn, appentency, upselling), teremos uma seleção diferente e a criação de um dataset com essas variáveis.
</p>

<p>
  Por conta do limite da plataforma, não podemos subir um arquivo com mais de 25mb, mas basta você entrar no site da <a href='https://kdd.org/kdd-cup/view/kdd-cup-2009'>KDD Cup 2009</a>, baixar o dataset e rodar esse Jupyter Notebook, onde será gerado os três novos datasets, utilizados para a predição das variáveis.
</p>
<br>
<h2>Churn, Appentency, Upselling</h2>

<p>
  Com os novos datasets gerados, podemos realizar as predições, através de um modelo de classificação. Os notebooks se encontram aqui:
  <ul>
    <li><a href='https://github.com/caioandre182/CRM---Orange/blob/main/CRM/Predi%C3%A7%C3%A3o%20-%20Churn.ipynb'>CHURN</a></li>
    <li><a href='https://github.com/caioandre182/CRM---Orange/blob/main/CRM/Predi%C3%A7%C3%A3o%20-%20Appentency.ipynb'>APPENTENCY</a></li>
    <li><a href='https://github.com/caioandre182/CRM---Orange/blob/main/CRM/Predi%C3%A7%C3%A3o%20-%20Upselling.ipynb'>UPSELLING</a></li>
  </ul>
</p>
<br>
<h2>Conclusões</h2>

<h3>Resultados</h3>

<table>
    <tr>
      <td>Variáveis</td>
      <td>Churn</td>
      <td>Appentency</td>
      <td>Upselling</td>
    </tr>
    <tr>
       <td>Scores</td>
       <td>0.68</td>
       <td>0.74</td>
       <td>0.75</td>
    </tr>
    <tr>
       <td>Porcentagem(%)</td>
       <td>68%</td>
       <td>74%</td>
       <td>75%</td>
    </tr>
</table>

<p>
  A tabela acima, indica o score e a porcentagem de precisão do modelo, em classificar corretamente as variáveis preditas. Pela falta de informação das variáveis, considero um bom resultado, óbvio que conforme vou aumentando meu conhecimento, pretendo trazer melhorias afim de elevar essas pontuações. Um grupo de pesquisa venceu a competição, a variável Churn teve um score de 0.75, evidenciando de certa forma, uma boa predição. Aplicar esses modelos em novas bases de dados que virão, podem garantir enormes retornos financeiros para empresa, antecipar a troca de serviço, identificar clientes com maior possibilidade de adquirir novos serviços ou produtos, é fundamental para uma empresa se manter competitiva e seguir crescendo.
</p>
