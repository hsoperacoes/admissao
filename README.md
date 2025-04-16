<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ficha de Admissão</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
    }
    h1 {
      text-align: center;
    }
    fieldset {
      border: 1px solid #ccc;
      padding: 15px;
      margin-bottom: 20px;
    }
    label {
      display: block;
      margin-top: 8px;
    }
    input, select {
      width: 100%;
      padding: 6px;
      margin-top: 4px;
      margin-bottom: 10px;
    }
    button {
      margin-top: 15px;
      padding: 10px 15px;
      font-size: 16px;
    }
    #resumoImpressao {
      display: none;
    }
    .linha-resumo {
      margin-bottom: 10px;
    }

    @media print {
      body * {
        visibility: hidden;
      }
      #resumoImpressao, #resumoImpressao * {
        visibility: visible;
      }
      #resumoImpressao {
        position: absolute;
        left: 0;
        top: 0;
      }
    }
  </style>
</head>
<body>

<h1>Ficha de Admissão</h1>

<form id="fichaAdmissao" onsubmit="return validarFormulario();">
  <fieldset>
    <legend>Informações Pessoais</legend>

    <label>Nome:</label>
    <input type="text" name="nome" required>

    <label>Endereço:</label>
    <input type="text" name="endereco" required>

    <label>Telefone:</label>
    <input type="text" name="telefone" required>

    <label>Data de Nascimento:</label>
    <input type="date" name="nascimento" required>

    <label>CPF:</label>
    <input type="text" name="cpf" required>

    <label>Função:</label>
    <input type="text" name="funcao" required>

    <label>Salário:</label>
    <input type="number" name="salario" required>
  </fieldset>

  <button type="submit">Enviar</button>
  <button type="button" onclick="gerarResumo()">Imprimir</button>
</form>

<div id="resumoImpressao">
  <h2>Resumo da Ficha de Admissão</h2>
  <div class="linha-resumo"><strong>Nome:</strong> <span id="resumoNome"></span></div>
  <div class="linha-resumo"><strong>Endereço:</strong> <span id="resumoEndereco"></span></div>
  <div class="linha-resumo"><strong>Telefone:</strong> <span id="resumoTelefone"></span></div>
  <div class="linha-resumo"><strong>Data de Nascimento:</strong> <span id="resumoNascimento"></span></div>
  <div class="linha-resumo"><strong>CPF:</strong> <span id="resumoCPF"></span></div>
  <div class="linha-resumo"><strong>Função:</strong> <span id="resumoFuncao"></span></div>
  <div class="linha-resumo"><strong>Salário:</strong> R$ <span id="resumoSalario"></span></div>

  <button type="button" onclick="voltarFormulario()">Voltar</button>
</div>

<script>
  function validarFormulario() {
    const form = document.getElementById("fichaAdmissao");
    if (!form.checkValidity()) {
      alert("Por favor, preencha todos os campos obrigatórios.");
      return false;
    }
    alert("Ficha enviada com sucesso!");
    return true;
  }

  function gerarResumo() {
    const form = document.forms["fichaAdmissao"];

    document.getElementById("resumoNome").textContent = form.nome.value;
    document.getElementById("resumoEndereco").textContent = form.endereco.value;
    document.getElementById("resumoTelefone").textContent = form.telefone.value;
    document.getElementById("resumoNascimento").textContent = form.nascimento.value;
    document.getElementById("resumoCPF").textContent = form.cpf.value;
    document.getElementById("resumoFuncao").textContent = form.funcao.value;
    document.getElementById("resumoSalario").textContent = parseFloat(form.salario.value).toFixed(2);

    document.getElementById("fichaAdmissao").style.display = "none";
    document.getElementById("resumoImpressao").style.display = "block";

    window.print();
  }

  function voltarFormulario() {
    document.getElementById("resumoImpressao").style.display = "none";
    document.getElementById("fichaAdmissao").style.display = "block";
  }
</script>

</body>
</html>
