# Tabela.PHP
Criação de tabela no php

-- ht é o atalho para HTML5 --
-- td*4 é o atalho para criar varias tabelas --

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tabela</title>
</head>
<body>
    
</body>
<table border="1">
<tr>
    <td>Codigo</td>
    <td>CPF</td>
    <td>Telefone</td>
    <td>RG</td>
</tr>
<?php
for($x = 0; $x < 5; $x ++){
    ?>
    <tr>
        <td><?=$x + 1?></td>
        <td><?= rand(10000000000,99999999999) ?></td>
        <td><?= rand(10000000000,99999999999) ?></td>
        <td><?= rand(100000000,999999999) ?></td>
    </tr>
    <?php
}
?>
</tr>
</table>
</html>
