<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <h1>FizzBUzz</h1>

</head>
<body>
<script>

function fizzbuzz() {
        var display = document.getElementById('display');
        var divisible = "";
        var displayHTML = "";

for (i = 1; i < 101; i++) {
        if (i % 3 === 0 && i % 5 === 0) {
            divisible = "FizzBuzz";
        } else if (i % 5 === 0) {
                divisible = "Buzz";
        } else if (i % 3 === 0) {
                divisible = "Fizz";
        } else {
            divisible = "";
        }

displayHTML += "<p>" + i + ":" + divisible + "</p>";
    }
    display.insertAdjacentHTML('afterend', displayHTML);
}


</script>
</body>
</html>