<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ficha de Admissão de Funcionários</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background-color: #f4f6f8;
      margin: 0;
      padding: 30px;
      color: #333;
    }

    h1 {
      text-align: center;
      font-size: 28px;
      color: #2c3e50;
      margin-bottom: 30px;
    }

    form {
      background: #ffffff;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      max-width: 900px;
      margin: 0 auto;
    }

    fieldset {
      border: none;
      margin-bottom: 25px;
      padding: 0;
    }

    legend {
      font-weight: 600;
      font-size: 20px;
      color: #2980b9;
      margin-bottom: 10px;
      border-bottom: 1px solid #ddd;
      padding-bottom: 5px;
    }

    label {
      display: block;
      margin-top: 15px;
      font-size: 14px;
    }

    input[type="text"],
    input[type="date"],
    input[type="number"],
    input[type="time"],
    select {
      width: 100%;
      padding: 10px;
      margin-top: 6px;
      border: 1px solid #ccc;
      border-radius: 8px;
      box-sizing: border-box;
      font-size: 14px;
    }

    input[type="checkbox"],
    input[type="radio"] {
      margin-right: 8px;
    }

    .row {
      display: flex;
      gap: 20px;
    }

    .col {
      flex: 1;
    }

    button {
      background-color: #3498db;
      color: white;
      padding: 12px 24px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
      transition: background 0.3s;
      display: block;
      margin: 30px auto 0;
    }

    button:hover {
      background-color: #2980b9;
    }

    p {
      margin-top: 15px;
      font-size: 13px;
      color: #7f8c8d;
    }

    .checkbox-group,
    .radio-group {
      margin-top: 10px;
    }

    .checkbox-group label,
    .radio-group label {
      display: inline-block;
      margin-right: 20px;
      font-size: 14px;
    }

    input[type="text"][disabled] {
      background-color: #eee;
    }
  </style>
</head>
<body>
  <h1>Ficha de Admissão de Funcionário</h1>

  <form>
    <fieldset>
      <legend>Informações Pessoais</legend>

      <label for="nome">Nome completo:</label>
      <input type="text" id="nome" name="nome">

      <label for="nascimento">Data de nascimento:</label>
      <input type="date" id="nascimento" name="nascimento">

      <label for="cpf">CPF:</label>
      <input type="text" id="cpf" name="cpf">

      <label for="rg">RG:</label>
      <input type="text" id="rg" name="rg">

      <label for="sexo">Sexo:</label>
      <select id="sexo" name="sexo">
        <option value="">Selecione</option>
        <option value="masculino">Masculino</option>
        <option value="feminino">Feminino</option>
        <option value="outro">Outro</option>
      </select>

      <label for="civil">Estado civil:</label>
      <select id="civil" name="civil">
        <option value="">Selecione</option>
        <option value="solteiro">Solteiro(a)</option>
        <option value="casado">Casado(a)</option>
        <option value="divorciado">Divorciado(a)</option>
        <option value="viuvo">Viúvo(a)</option>
      </select>

      <label for="nacionalidade">Nacionalidade:</label>
      <input type="text" id="nacionalidade" name="nacionalidade">
    </fieldset>

    <fieldset>
      <legend>Endereço</legend>

      <label for="endereco">Endereço:</label>
      <input type="text" id="endereco" name="endereco">

      <label for="cidade">Cidade:</label>
      <input type="text" id="cidade" name="cidade">

      <label for="estado">Estado:</label>
      <input type="text" id="estado" name="estado">

      <label for="cep">CEP:</label>
      <input type="text" id="cep" name="cep">
    </fieldset>

    <fieldset>
      <legend>Informações Profissionais</legend>

      <label for="cargo">Cargo:</label>
      <input type="text" id="cargo" name="cargo">

      <label for="salario">Salário:</label>
      <input type="number" id="salario" name="salario" step="0.01">

      <label for="admissao">Data de admissão:</label>
      <input type="date" id="admissao" name="admissao">

      <label for="horario">Horário de trabalho:</label>
      <input type="text" id="horario" name="horario" placeholder="Ex: 08:00 às 17:00">
    </fieldset>

    <fieldset>
      <legend>Informações de Contato</legend>

      <label for="telefone">Telefone:</label>
      <input type="text" id="telefone" name="telefone">

      <label for="email">E-mail:</label>
      <input type="text" id="email" name="email">
    </fieldset>

    <fieldset>
      <legend>Documentos Entregues</legend>

      <div class="checkbox-group">
        <label><input type="checkbox" name="documentos" value="cpf">CPF</label>
        <label><input type="checkbox" name="documentos" value="rg">RG</label>
        <label><input type="checkbox" name="documentos" value="ctps">CTPS</label>
        <label><input type="checkbox" name="documentos" value="comprovante">Comprovante de Residência</label>
      </div>
    </fieldset>

    <fieldset>
      <legend>Observações</legend>
      <textarea name="observacoes" rows="4" style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid #ccc; font-size: 14px;"></textarea>
    </fieldset>

    <button type="submit">Enviar</button>
  </form>
</body>
</html>
