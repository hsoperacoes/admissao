<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
        input[type="text"], input[type="date"], input[type="number"], select {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            margin-bottom: 10px;
        }
        input[type="checkbox"] {
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
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <h1>Ficha de Admissão de Funcionário</h1>
    
    <form action="#" method="POST">
        <!-- Dados da empresa -->
        <fieldset>
            <legend>01) INFORMAÇÕES PESSOAIS</legend>
            <label for="nome">Nome do Funcionário:</label>
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

            <label for="casa_propria">Casa Própria:</label>
            <input type="checkbox" id="casa_propria" name="casa_propria">

            <label for="grau_escolaridade">Grau de Escolaridade:</label>
            <select id="grau_escolaridade" name="grau_escolaridade">
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

            <label for="conta_bancaria">Conta Bancária:</label>
            <input type="radio" id="conta_corrente" name="conta_bancaria" value="corrente">
            <label for="conta_corrente">Conta Corrente</label>
            <input type="radio" id="conta_poupanca" name="conta_bancaria" value="poupanca">
            <label for="conta_poupanca">Conta Poupança</label>

            <label for="banco">Banco:</label>
            <input type="text" id="banco" name="banco">

            <label for="agencia">Agência:</label>
            <input type="text" id="agencia" name="agencia">

            <label for="numero_conta">Número da Conta:</label>
            <input type="text" id="numero_conta" name="numero_conta">
        </fieldset>

        <!-- Dados para Registro -->
        <fieldset>
            <legend>02) INFORMAÇÕES PARA REGISTRO</legend>
            <label for="data_admissao">Data da Admissão:</label>
            <input type="date" id="data_admissao" name="data_admissao" required>

            <label for="data_exame_admissional">Data do Exame Admissional:</label>
            <input type="date" id="data_exame_admissional" name="data_exame_admissional" required>

            <label for="funcao">Função:</label>
            <input type="text" id="funcao" name="funcao" required>

            <label for="salario">Salário:</label>
            <input type="number" id="salario" name="salario" required>

            <label for="contrato_experiencia">Contrato de Experiência:</label>
            <input type="checkbox" id="contrato_experiencia" name="contrato_experiencia">
            
            <label for="pis">PIS:</label>
            <input type="text" id="pis" name="pis" required>

            <label for="primeiro_emprego">Primeiro Emprego:</label>
            <input type="checkbox" id="primeiro_emprego" name="primeiro_emprego">
        </fieldset>

        <!-- Dependentes -->
        <fieldset>
            <legend>03) DEPENDENTES</legend>
            <label for="filhos_menores_14">Filhos menores de 14 anos:</label>
            <input type="checkbox" id="filhos_menores_14" name="filhos_menores_14">

            <label for="quantidade_filhos">Quantos:</label>
            <input type="number" id="quantidade_filhos" name="quantidade_filhos">
        </fieldset>

        <!-- Documentos Necessários -->
        <fieldset>
            <legend>04) DOCUMENTOS NECESSÁRIOS PARA ADMISSÃO</legend>
            <label for="documentos">Marque os documentos entregues:</label>
            <input type="checkbox" id="ficha_admissao" name="documentos" value="ficha_admissao">
            <label for="ficha_admissao">Ficha de Admissão</label>
            <input type="checkbox" id="carteira_trabalho" name="documentos" value="carteira_trabalho">
            <label for="carteira_trabalho">Carteira de Trabalho</label>
            <input type="checkbox" id="pis_documento" name="documentos" value="pis_documento">
            <label for="pis_documento">Número do PIS</label>
            <input type="checkbox" id="rg" name="documentos" value="rg">
            <label for="rg">RG</label>
            <input type="checkbox" id="cpf" name="documentos" value="cpf">
            <label for="cpf">CPF</label>
            <input type="checkbox" id="exame_medico" name="documentos" value="exame_medico">
            <label for="exame_medico">Exame Médico Admissional</label>
        </fieldset>

        <button type="submit">Enviar Ficha de Admiss
