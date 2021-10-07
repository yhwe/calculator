# calculator
# a calculator that take 2 inputs and calculate in html
<!DOCTYPE html>
<html>

<head>
    <title>javascript: calculate two numbers</title>
    <meta charset="windows-1252">
    <meta name="viewport" content="width=device-width, intial-scale=1.0">

    <script>
        function calc() {
            var n1 = parseInt(document.getElementById("n1").value);
            var n2 = parseInt(document.getElementById('n2').value);
            var oper = document.getElementById('operators').value;

            if (oper == "+") {
                document.getElementById('result').value = n1 + n2;
            }
            if (oper == '-') {
                document.getElementById('result').value = n1 - n2;
            }
            if (oper == '/') {
                document.getElementById('result').value = n1 / n2;
            }
            if (oper == 'X') {
                document.getElementById('result').value = n1 * n2;
            }
        }
    </script>

    <style>
        body {
            background-color: red;
        }
        
        .i1 {
            margin-left: 10%;
            margin-top: 10%;
            background-color: #724caf;
            color: white;
            padding: 15px 32px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            cursor: pointer;
        }
    </style>

</head>

<body>
    <form>
        <input type="text" id="n1" class="i1"><br/><br/>
        <input type="text" id="n2" class="i1"><br/><br/>
    </form>
    <select id="operators" class="i1">
            <option value="+">topla</option>
            <option value="-">cikart</option>
            <option value="/">bol</option>
            <option value="X">carp</option>
        </select>
    <button onclick="calc();" class="i1">=</button>
    <input type="text" class="i1" id="result" />

</body>
  
</html>
