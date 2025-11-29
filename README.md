# Mini-Calculater

<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mini Calculater</title>
</head>

<style>
    h1 {
        text-align: center;
        border: 5px solid black;
        width: 50%;
        border-radius: 10px;
        margin: auto;
    }
</style>

<body>
    <script>
        alert('Do you want to calculate any number with the help of + , - , * and /');
        let num1 = + prompt('Enter your first number');
        let operater = prompt('Enter operaters : + , - , * and /');
        let num2 = + prompt('Enter your second number');


        if (isNaN(num1) || isNaN(num2)) {
            document.write('<h1><b> Error: Enter only numbers</b></h1>')
        }

        else if (operater === '+') {
            document.write(' <h1><b> Result Of ' + num1 + ' + ' + num2 + ' Is : ' + (num1 + num2) + '</h1></b>')
        }

        else if (operater === '-') {
            document.write(' <h1><b> Result Of ' + num1 + ' - ' + num2 + ' Is : ' + (num1 - num2) + '</h1></b>')
        }

        else if (operater === '*') {
            document.write(' <h1><b> Result Of ' + num1 + ' * ' + num2 + ' Is : ' + (num1 * num2) + '</h1></b>')
        }

        else if (operater === '/') {
            if (num2 === 0) {
                document.write(' <h1><b> Division by 0 is not allowed </h1></b>')
            }
            else {
                document.write(' <h1><b> Result Of ' + num1 + ' / ' + num2 + ' Is : ' + (num1 / num2) + '</h1></b>')
            }

        }

        else if (!(operater === '+' || operater === '-' || operater === '*' || operater === '/')) {
            document.write('<h1><b> Error: Use Only These Operaters Like : + , - , * and /</b></h1>')
        }


    </script>
</body>

</html>
