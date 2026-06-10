<hr>

<h1 align="center">🏗️ Arquitetura da Solução</h1>

<p align="center">
  O diagrama abaixo representa a comunicação entre a infraestrutura local da empresa e os serviços hospedados na AWS.
</p>

<div align="center">

<img
    src="Diagrama de EC2.png"
    alt="Diagrama de Arquitetura AWS EC2"
    width="900"
/>

</div>

<br>

<h2>📋 Componentes da Arquitetura</h2>

<h3>👤 Usuário (Ator)</h3>

<p>
Responsável por interagir com o sistema corporativo e realizar o envio de arquivos para processamento.
</p>

<h3>💻 Sistema Corporativo</h3>

<p>
Aplicação hospedada na infraestrutura da empresa responsável pela comunicação com os serviços AWS.
</p>

<h3>☁️ AWS Cloud</h3>

<p>
Ambiente responsável pelo processamento, armazenamento e gerenciamento dos recursos utilizados pela aplicação.
</p>

<h3>🖥️ Amazon EC2</h3>

<p>
Instância utilizada para processamento das informações e execução da aplicação.
</p>

<h3>💾 Amazon EBS</h3>

<ul>
<li>EBS D - Volume de armazenamento auxiliar</li>
<li>EBS E - Volume de armazenamento persistente</li>
</ul>

<h3>🗄️ Amazon RDS</h3>

<p>
Serviço de banco de dados gerenciado responsável pelo armazenamento das informações da aplicação.
</p>

<hr>

<h2>🔄 Fluxo de Funcionamento</h2>

<ol>
<li>O usuário interage com o sistema corporativo.</li>
<li>O sistema envia arquivos para processamento.</li>
<li>A instância EC2 recebe e processa os dados.</li>
<li>Os arquivos são armazenados nos volumes EBS.</li>
<li>As informações são persistidas no Amazon RDS.</li>
<li>Os resultados retornam ao sistema corporativo.</li>
</ol>

<hr>

<h2>✅ Benefícios da Arquitetura</h2>

<ul>
<li>Escalabilidade</li>
<li>Alta disponibilidade</li>
<li>Armazenamento persistente</li>
<li>Segurança dos dados</li>
<li>Facilidade de manutenção</li>
<li>Integração com serviços AWS</li>
</ul>

<hr>
