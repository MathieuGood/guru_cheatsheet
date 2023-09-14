# PHP Cheatsheet

```php
// Variables
$myVariable = 0;
$name = "Mathieu";
var_dump($name);

// Print PHP config
phpinfo();

// Checking equality
// "1" == 1 >> TRUE
// "1" === 1 >> FALSE

// Arrays
$namesArray = [$name, "John", "Paul", "James"];
// OR via array() function
$recipes = array('Guacamole', 'Taco', 'Hamburger');
$recipes[3] = 'Pizza';
$recipes[] = 'Mac and cheese';
$recipes = array(2 =>'Guacamole', 3 => 'Taco', 4 => 'Hamburger');
$recipes = array("Guacamole" => "Mexican", "Taco" => "Mexican");

$recipe = [
    'title' => 'Pizza',
    'recipe' => 'Spread dough, add toppings, cook',
    'author' => 'chef@best-pizza.com',
    'enabled' => true,
];

$recipe['title'] = 'Pizza';
$recipe['recipe'] = 'Spread dough, add toppings, cook';
$recipe['author'] = 'chef@best-pizza.com';
$recipe['enable'] = true;

// Print
echo $myVariable;
echo 'hello ' . $name . ' and welcome!';

// Conditionals
// AND >> &&
// OR >> || 
if ($totalPrice > $totalBudget) {
    echo "Price higher than budget";
}
elseif ($totalPrice < $totalBudget) {
    echo "Price lower than budget";
}
else {
    echo "Price equal to budget";
}

if (! $isAllowedToEnter) {
    echo "Not allowed";
}

// Conditional integrated in HTML code
<?php $chickenRecipesEnabled = true; ?>
<?php if ($chickenRecipesEnabled): ?> <!-- Not to forget ":" -->
<h1>Liste of recipes with chicken</h1>
<?php endif; ?> 

// Swich case
$country = "France";

switch ($grade)
{ 
    case "France":
        echo "Europe";
    break;
    
    case > 12:
        echo "Average";
    break;
    
    case > 10:
        echo "Need more work";
    break;

    default:
        echo "Fail";
}


// While loop
$count = 1;
while ($count <= 100) {
    echo "Compteur : $count<br>";
    $count++
}


// For loop
$michael = ['Michael Palin', 'michael.palin@montypython.com', 'S3cr3t', 34];
$john = ['John Cleese', 'john.cleese@montypython.com', 'devine', 33];
$eric = ['Eric Idle', 'eric.idle@montypython.com', 'P4ssw0rD', 28];
$users = [$michael, $john, $eric];

for ($lines = 0; $lines <= 2; $lines++)
{
    echo $users[$lines][0] . ' ' . $users[$lines][1] . '<br>';
}


// For loop integrated in HTML
<ul>
    <?php for ($lines = 0; $lines <= 1; $lines++): ?>
        <li><?php echo $users[$lines][0] . ' (' . $users[$lines][1] . ')'; ?></li>
    <?php endfor; ?>
</ul>

```
