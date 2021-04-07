<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <script>
        function quadrat(abc) {
            var ergebnis = abc * abc;
            return ergebnis;
        }
        function dritteRechnung(Dreifach) {
            var ergebnis = (Dreifach*Dreifach*Dreifach)-3;
            return ergebnis;
}
        function teilrechnung(a) {
            var ergebnis = (a * a * a) /2; 
            return ergebnis
        }
    </script>
    <style>
        td{
            width:25%;
        }
    </style>
</head>

<body>
    
    <table class="table">
        <thead>
          <tr>
            <th scope="col">i</th>
            <th scope="col">i*i</th>
            <th scope="col">(i*i*i)-3</th>
            <th scope="col">(i*i*i)/2</th>
          </tr>
        </thead>
        <script>
            for (var i=0; i < 10; i++){
              document.write("<tr><td>" + i + "</td><td>" + quadrat(i) + "</td><td>" + dritteRechnung(i) + "</td><td>" + teilrechnung(i) + "</td></tr>")

            }

        </script>


        <tbody>
      </table>
      

</body>




</html>

<!--
function dritteRechnung(Dreifach) {
    var ergebnis = Dreifach*Dreifach*Dreifach;
    return ergebnis;
}


function NamederFunktion(Variable) {
    var Ergebnis = (Variable*Variable*Variable)-3;
    return Ergebnis;



-->
