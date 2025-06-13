# Tabela.PHP
Criação de tabela no php

-- ht é o atalho para HTML5 --
-- td*4 é o atalho para criar varias tabelas --

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8"> <!-- Define a codificação de caracteres -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Configura o tamanho da tela para dispositivos móveis -->
    <title>Tabela</title> <!-- Define o título da página -->
</head>
<body>
    <!-- Corpo da página, vazio por enquanto -->
</body>

<!-- Criação da tabela com borda -->
<table border="1">
<tr>
    <td>Codigo</td> <!-- Coluna para o código identificador -->
    <td>CPF</td> <!-- Coluna para o CPF -->
    <td>Telefone</td> <!-- Coluna para o telefone -->
    <td>RG</td> <!-- Coluna para o RG -->
</tr>

<?php
// Loop que gera 5 linhas de dados fictícios //
for($x = 0; $x < 5; $x ++){
    ?>
<tr>
        <td><?= $x + 1 ?></td> <!-- Código sequencial começando em 1 -->
        <td><?= rand(10000000000,99999999999) ?></td> <!-- Geração de um CPF aleatório -->
        <td><?= rand(10000000000,99999999999) ?></td> <!-- Geração de um telefone aleatório -->
        <td><?= rand(100000000,999999999) ?></td> <!-- Geração de um RG aleatório -->
    </tr>
    <?php
}
?>
</tr>
</table>
</html>
