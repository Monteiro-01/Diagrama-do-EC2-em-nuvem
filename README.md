```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AWS EC2 Lab - Gerenciamento de Instâncias</title>

    <link rel="stylesheet" href="css/style.css">
</head>

<body>

<header>
    <h1>🚀 AWS EC2 Lab</h1>
    <p>Gerenciamento de Instâncias na AWS</p>

    <div class="badges">
        <span class="badge">AWS EC2</span>
        <span class="badge">Cloud Computing</span>
        <span class="badge">GitHub Documentation</span>
        <span class="badge">Concluído</span>
    </div>
</header>

<div class="container">

<section>
    <h2>📌 Sobre o Projeto</h2>

    <div class="card">
        <p>
            Este laboratório teve como objetivo explorar os principais recursos do
            Amazon EC2 (Elastic Compute Cloud), permitindo a criação,
            configuração, monitoramento e gerenciamento de servidores virtuais
            na nuvem.
        </p>
    </div>
</section>

<section>
    <h2>🎯 Objetivos</h2>

    <div class="grid">

        <div class="card">
            Criar e configurar instâncias EC2
        </div>

        <div class="card">
            Configurar Security Groups
        </div>

        <div class="card">
            Acesso remoto via SSH
        </div>

        <div class="card">
            Monitoramento com CloudWatch
        </div>

        <div class="card">
            Aplicar boas práticas de segurança
        </div>

        <div class="card">
            Documentação utilizando GitHub
        </div>

    </div>
</section>

<section>
    <h2>🏗️ Arquitetura</h2>

    <div class="architecture">
<pre>
┌──────────────┐
│   Usuário    │
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ Internet     │
└──────┬───────┘
       │
       ▼
┌─────────────────────┐
│ Security Group      │
│ SSH | HTTP | HTTPS  │
└──────┬──────────────┘
       │
       ▼
┌─────────────────────┐
│ Amazon EC2          │
│ Ubuntu Server       │
└──────┬──────────────┘
       │
       ▼
┌─────────────────────┐
│ Amazon CloudWatch   │
└─────────────────────┘
</pre>
    </div>
</section>

<section>
    <h2>🔧 Configurações da Instância</h2>

    <table>

        <tr>
            <th>Configuração</th>
            <th>Valor</th>
        </tr>

        <tr>
            <td>Sistema Operacional</td>
            <td>Ubuntu Server</td>
        </tr>

        <tr>
            <td>Tipo da Instância</td>
            <td>t2.micro</td>
        </tr>

        <tr>
            <td>Região</td>
            <td>us-east-1</td>
        </tr>

        <tr>
            <td>Armazenamento</td>
            <td>8 GB SSD</td>
        </tr>

        <tr>
            <td>Chave SSH</td>
            <td>RSA</td>
        </tr>

    </table>

</section>

<section>
    <h2>🔒 Segurança</h2>

    <table>

        <tr>
            <th>Porta</th>
            <th>Protocolo</th>
            <th>Função</th>
        </tr>

        <tr>
            <td>22</td>
            <td>TCP</td>
            <td>SSH</td>
        </tr>

        <tr>
            <td>80</td>
            <td>TCP</td>
            <td>HTTP</td>
        </tr>

        <tr>
            <td>443</td>
            <td>TCP</td>
            <td>HTTPS</td>
        </tr>

    </table>

</section>

<section>
    <h2>💻 Conexão SSH</h2>

    <div class="code">
<pre>
ssh -i chave.pem ubuntu@IP_PUBLICO
</pre>
    </div>

</section>

<section>
    <h2>📊 Monitoramento CloudWatch</h2>

    <div class="card">
        <ul>
            <li>Uso de CPU</li>
            <li>Tráfego de Rede</li>
            <li>Disco</li>
            <li>Status da Instância</li>
            <li>Alarmes e Eventos</li>
        </ul>
    </div>
</section>

<section>
    <h2>📈 Insights Obtidos</h2>

    <div class="card">
        <p>
            O laboratório demonstrou como a computação em nuvem permite
            provisionar infraestrutura rapidamente, garantindo escalabilidade,
            disponibilidade e segurança.
        </p>
    </div>

</section>

</div>

<footer>

    <h3>👨‍💻 Gabriel Monteiro</h3>

    <p>
        Estudante de Engenharia | Dados | IA | Cloud Computing
    </p>

    <p>
        Projeto desenvolvido para fins educacionais.
    </p>

</footer>

</body>
</html>
```
