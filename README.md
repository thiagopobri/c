<!DOCTYPE html>
<html lang="pt-br">
<head>
  <title>Bootstrap 5 Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <div id="header" class="container-fluid header p-5 text-white text-center" style="background-color: blue;">
    <h3>Cálculo de Massa Corporal (IMC)</h3>
</div>
  <div class="container mx-auto mt-5">
    <div class="row">
      <div class="col-sm-4">
        <div class="form-imc">
          <form novalidate class="form">
            <label for="peso" class="form-label">Informe o peso:</label>
            <input type="number" class="form-control" placeholder="Peso (Kg)" id="peso" />
            <label for="altura" class="form-label">Informe a altura:</label>
            <input type="number" class="form-control" placeholder="Altura" id="altura" />
          </form>
          <button class="btn btn-primary calcular" onclick="imc()">Calcular</button>
        </div>
      </div>
      <div class="col-sm-4">
        <div class="imc-resultado homem">
          <div><img src="img/homem.png" style="width: 200px;" id="mulher" alt=""></div>
          <button class="btn btn-primary btn-imc" type="button" id="btmulher">Mulher</button>
          <button class="btn btn-primary btn-imc" type="button" id="bthomem">Homem</button>
        </div>
      </div>
      <div class="col-sm-4">
        <div class="resultado" id="resultado">
          <p id="imcresultado">Seu IMC:</p>
          <p id="imc">Classificação:</p>
        </div>
      </div>
    </div>
  </div>
  <div class="container mx-auto mt-5">
    <div class="row">
      <div class="col-sm-4">
        <div class="medida">
          <p>
            O IMC (Índice de Massa Corpórea) é uma medida internacional usada para avaliar o peso ideal. Seu cálculo é
            feito dividindo o peso pela altura elevada ao quadrado. O resultado diz se estamos dentro de uma faixa
            saudável ou não. Caso você esteja abaixo ou acima do recomendado, procure ajuda especializada para receber
            acompanhamento.
          </p>
        </div>
      </div>
      <div class="col-sm-4">
        <div>
          <table class="table table-bordered">
            <thead>
              <tr>
                <th>IMC</th>
                <th>CLASSIFICAÇÃO</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Menor que 18,5</td>
                <td>Abaixo do peso</td>
              </tr>
              <tr>
                <td>18,5 a 24,9</td>
                <td>Peso saudável</td>
              </tr>
              <tr>
                <td>25,0 a 29,9</td>
                <td>Sobrepeso</td>
              </tr>
              <tr>
                <td>30,0 a 34,9</td>
                <td>Obesidade Grau 1</td>
              </tr>
              <tr>
                <td>35,0 a 39,9</td>
                <td>Obesidade Grau 2</td>
              </tr>
              <tr>
                <td>Maior que 40,0</td>
                <td>Obesidade Grau 3</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
  <footer class="container-fluid p-4 text-white text-center">
    <p>&copy; 2023 Desenvolvido por thiago</p>
  </footer>
</body>
<script src="js/index.js"></script>
</html>
