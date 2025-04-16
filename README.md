<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ficha de Admissão de Funcionários</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      padding: 20px;
    }
    h1 {
      text-align: center;
      font-size: 24px;
    }
    fieldset {
      border: 1px solid #ccc;
      padding: 15px;
      margin-bottom: 20px;
    }
    legend {
      font-weight: bold;
      font-size: 18px;
    }
    label {
      display: block;
      margin-top: 8px;
    }
    input[type="text"], input[type="date"], input[type="number"], input[type="time"], select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      margin-bottom: 10px;
    }
    input[type="checkbox"], input[type="radio"] {
      margin-right: 10px;
    }
    .row {
      display: flex;
      flex-wrap: wrap;
    }
    .col {
      flex: 1;
      margin-right: 10px;
    }
    .col:last-child {
      margin-right: 0;
    }
    button {
      background-color: #4CAF50;
      color: white;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
      font-size: 16px;
      margin-top: 20px;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <h1>Ficha de Admissão de Funcionário</h1>

  <form id="fichaAdmissao" onsubmit="return validarFormulario();">
    <fieldset>
      <legend>01) INFORMAÇÕES PESSOAIS</legend>
      <label for="nome">NOME DO FUNCIONÁRIO (A):</label>
      <input type="text" id="nome" name="nome" required>

      <label for="endereco">Endereço Residencial:</label>
      <input type="text" id="endereco" name="endereco" required>

      <label for="bairro">Bairro:</label>
      <input type="text" id="bairro" name="bairro" required>

      <label for="cep">CEP:</label>
      <input type="text" id="cep" name="cep" required>

      <label for="telefone">Fones:</label>
      <input type="text" id="telefone" name="telefone" required>

      <label for="cidade">Cidade:</label>
      <input type="text" id="cidade" name="cidade" required>

      <label for="uf">UF:</label>
      <input type="text" id="uf" name="uf" required>

      <p>OBS: Sempre que houver mudança de endereço, deve ser comunicado imediatamente ao escritório.</p>

      <label><input type="checkbox" id="casa_propria" name="casa_propria"> Casa Própria</label>
      <label><input type="checkbox" id="recursos_cef" name="recursos_cef"> Adquirida com recursos da CEF</label>

      <label for="grau_escolaridade">Grau de Escolaridade:</label>
      <select id="grau_escolaridade" name="grau_escolaridade" required>
        <option value="">Selecione</option>
        <option value="analfabeto">Analfabeto</option>
        <option value="ate_4a_serie">Até a 4ª Série</option>
        <option value="de_5a_8a_serie">De 5ª a 8ª Série</option>
        <option value="1o_grau_completo">1º grau completo</option>
        <option value="2o_grau_incompleto">2º grau incompleto</option>
        <option value="2o_grau_completo">2º grau completo</option>
        <option value="superior_incompleto">Superior incompleto</option>
        <option value="superior_completo">Superior Completo</option>
        <option value="pos_graduacao">Pós Graduação</option>
      </select>

      <label for="data_nascimento">Data de Nascimento:</label>
      <input type="date" id="data_nascimento" name="data_nascimento" required>

      <label for="naturalidade">Naturalidade:</label>
      <input type="text" id="naturalidade" name="naturalidade" required>

      <label for="estado_civil">Estado Civil:</label>
      <input type="text" id="estado_civil" name="estado_civil" required>

      <label for="nome_conjugue">Nome do Cônjuge:</label>
      <input type="text" id="nome_conjugue" name="nome_conjugue">

      <label for="cpf_conjugue">CPF do Cônjuge:</label>
      <input type="text" id="cpf_conjugue" name="cpf_conjugue">

      <label>Conta Bancária:</label>
      <label><input type="radio" name="conta_bancaria" value="corrente" required> Conta Corrente</label>
      <label><input type="radio" name="conta_bancaria" value="poupanca" required> Conta Poupança</label>

      <label for="banco">Banco:</label>
      <input type="text" id="banco" name="banco" required>

      <label for="agencia">Agência:</label>
      <input type="text" id="agencia" name="agencia" required>

      <label for="numero_conta">Número da Conta:</label>
      <input type="text" id="numero_conta" name="numero_conta" required>

      <label for="pix">PIX:</label>
      <input type="text" id="pix" name="pix" required>
    </fieldset>

    <fieldset>
      <legend>02) INFORMAÇÕES PARA REGISTRO</legend>

      <label for="data_admissao">Data da Admissão:</label>
      <input type="date" id="data_admissao" name="data_admissao" required>

      <label for="data_exame_admissional">Data do Exame Admissional:</label>
      <input type="date" id="data_exame_admissional" name="data_exame_admissional" required>

      <label for="funcao">Função:</label>
      <input type="text" id="funcao" name="funcao" required>

      <label for="salario">Salário (R$):</label>
      <input type="number" id="salario" name="salario" required>

      <label><input type="checkbox" id="contrato_experiencia" name="contrato_experiencia"> Contrato de Experiência</label>

      <label>Prazo do Contrato:</label>
      <label><input type="radio" name="prazo_contrato" value="30" required> 30 dias</label>
      <label><input type="radio" name="prazo_contrato" value="45" required> 45 dias</label>
      <label><input type="radio" name="prazo_contrato" value="60" required> 60 dias</label>
      <label><input type="radio" name="prazo_contrato" value="90" required> 90 dias</label>

      <label for="pis">PIS:</label>
      <input type="text" id="pis" name="pis" required>

      <label><input type="checkbox" id="primeiro_emprego" name="primeiro_emprego"> 1º Emprego</label>

      <label><input type="checkbox" id="vale_transporte" name="vale_transporte"> Vale Transporte</label>

      <label for="quantos_por_dia">Quantos por dia:</label>
      <input type="number" id="quantos_por_dia" name="quantos_por_dia" required>

      <label for="horario_trabalho">Horário de Trabalho:</label>
      <div class="row">
        <div class="col">
          <label for="entrada">Entrada:</label>
          <input type="time" id="entrada" name="entrada" required>
        </div>
        <div class="col">
          <label for="saida">Saída:</label>
          <input type="time" id="saida" name="saida" required>
        </div>
      </div>

      <label for="intervalo">Intervalo:</label>
      <div class="row">
        <div class="col">
          <label for="inicio_intervalo">Início:</label>
          <input type="time" id="inicio_intervalo" name="inicio_intervalo" required>
        </div>
        <div class="col">
          <label for="fim_intervalo">Fim:</label>
          <input type="time" id="fim_intervalo" name="fim_intervalo" required>
        </div>
      </div>
    </fieldset>

    <fieldset>
      <legend>03) DEPENDENTES</legend>
      <label><input type="checkbox" id="filhos_menores_14" name="filhos_menores_14"> Filhos menores de 14 anos</label>

      <label for="quantidade_filhos">Quantos:</label>
      <input type="number" id="quantidade_filhos" name="quantidade_filhos" required>
    </fieldset>

    <fieldset>
      <legend>04) DOCUMENTOS NECESSÁRIOS PARA ADMISSÃO</legend>
      <label><input type="checkbox" name="documentos" value="ficha_admissao" required> Ficha de Admissão</label>
      <label><input type="checkbox" name="documentos" value="carteira_trabalho" required> Carteira de Trabalho</label>
      <label><input type="checkbox" name="documentos" value="pis_documento" required> Número do PIS</label>
      <label><input type="checkbox" name="documentos" value="rg" required> RG</label>
      <label><input type="checkbox" name="documentos" value="cpf" required> CPF</label>
      <label><input type="checkbox" name="documentos" value="exame_medico" required> Exame Médico Admissional</label>
      <label><input type="checkbox" name="documentos" value="foto" required> Foto 3x4</label>
    </fieldset>

    <fieldset>
      <legend>05) DOCUMENTOS DE INTERESSE FUNCIONÁRIO</legend>
      <label><input type="checkbox" name="documentos_funcionario" value="certidao_nascimento" required> Certidão de Nascimento</label>
      <label><input type="checkbox" name="documentos_funcionario" value="cartao_vacina" required> Cartão de Vacina</label>
      <label><input type="checkbox" name="documentos_funcionario" value="atestado_escolaridade" required> Atestado de Escolaridade</label>
      <label><input type="checkbox" name="documentos_funcionario" value="termo_judicial" required> Termo Judicial (Adotivo)</label>
      <label><input type="checkbox" name="documentos_funcionario" value="certidao_casamento" required> Certidão de Casamento</label>
      <label><input type="checkbox" name="documentos_funcionario" value="cpf_filhos" required> CPF dos Filhos</label>
    </fieldset>

    <div>
      <label for="assinatura_funcionario">Assinatura do Funcionário:</label>
      <input type="text" id="assinatura_funcionario" name="assinatura_funcionario" required>
    </div>

    <div>
      <label for="assinatura_empresa">Assinatura da Empresa:</label>
      <input type="text" id="assinatura_empresa" name="assinatura_empresa" required>
    </div>

    <button type="submit">Enviar Ficha de Admissão</button>
    <button type="button" onclick="window.print()">Imprimir Ficha</button>
  </form>

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
  </script>
</body>
</html>
