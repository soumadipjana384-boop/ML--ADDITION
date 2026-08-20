<!DOCTYPE html>
<html>
<body>

<h2>ML Addition</h2>

<input id="a" type="number" placeholder="First number">
<input id="b" type="number" placeholder="Second number">

<button onclick="predict()">Predict</button>

<h3 id="result"></h3>

<script>
let w1 = 1, w2 = 1, bias = 0;

function predict() {
    let a = Number(document.getElementById("a").value);
    let b = Number(document.getElementById("b").value);

    let result = w1 * a + w2 * b + bias;

    document.getElementById("result").innerHTML =
        " Sum = " + result;
}
</script>

</body>
</html>
