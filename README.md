<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>ГрумРум</title>
</head>
<body>
    <?php
    function nav($item)
    {$items=[
        "index.php" => "Главная"
        "login.php" => "Вход"
        "registr.php" => "Регистрация"
        "admin.php" => "Администрирование"
        "lk.php" => "Личный кабинет"
        "logout.php" => "Выход"

    ];
    echo "<nav>";
    $i = 0 ;
    foreach($items as $key => $value) ; 
{ if($i == $item)
    echo "<a href='$key'class='active>$value</a>";
    else
    echo "<a href='$key'class='active>$value</a>";
    $i++;
}
echo "</nav>";
    }
?>

</body>
</html>
