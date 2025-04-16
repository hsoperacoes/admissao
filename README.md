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

            <label for="casa_propria">Casa Própria:</label>
            <input type="checkbox" id="casa_propria" name="casa_propria"> Sim

            <label for="recursos_cef">Adquirida com recursos da CEF:</label>
            <input type="checkbox" id="recursos_cef" name="recursos_cef"> Sim

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

            <label for="pix">PIX:</label>
            <input type="text" id="pix" name="pix">
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

            <label for="contrato_experiencia">Contrato de Experiência:</label>
            <input type="checkbox" id="contrato_experiencia" name="contrato_experiencia"> Sim

            <label for="prazo_contrato">Prazo:</label>
            <input type="radio" id="30_dias" name="prazo_contrato" value="30">
            <label for="30_dias">30 dias</label>
            <input type="radio" id="45_dias" name="prazo_contrato" value="45">
            <label for="45_dias">45 dias</label>
            <input type="radio" id="60_dias" name="prazo_contrato" value="60">
            <label for="60_dias">60 dias</label>
            <input type="radio" id="90_dias" name="prazo_contrato" value="90">
            <label for="90_dias">90 dias</label>

            <label for="pis">PIS:</label>
            <input type="text" id="pis" name="pis">

            <label for="primeiro_emprego">1º Emprego:</label>
            <input type="checkbox" id="primeiro_emprego" name="primeiro_emprego"> Sim

            <label for="vale_transporte">Vale Transporte:</label>
            <input type="checkbox" id="vale_transporte" name="vale_transporte"> Sim

            <label for="quantos_por_dia">Quantos por dia:</label>
            <input type="number" id="quantos_por_dia" name="quantos_por_dia">

            <label for="horario_trabalho">Horário de Trabalho:</label>
            <div class="row">
                <div class="col">
                    <label for="entrada">Entrada:</label>
                    <input type="time" id="entrada" name="entrada">
                </div>
                <div class="col">
                    <label for="saida">Saída:</label>
                    <input type="time" id="saida" name="saida">
                </div>
            </div>

            <label for="intervalo">Intervalo:</label>
            <div class="row">
                <div class="col">
                    <label for="inicio_intervalo">Início:</label>
                    <input type="time" id="inicio_intervalo" name="inicio_intervalo">
                </div>
                <div class="col">
                    <label for="fim_intervalo">Fim:</label>
                    <input type="time" id="fim_intervalo" name="fim_intervalo">
                </div>
            </div>
        </fieldset>

        <fieldset>
            <legend>03) DEPENDENTES</legend>
            <label for="filhos_menores_14">Filhos menores de 14 anos:</label>
            <input type="checkbox" id="filhos_menores_14" name="filhos_menores_14"> Sim

            <label for="quantidade_filhos">Quantos:</label>
            <input type="number" id="quantidade_filhos" name="quantidade_filhos">
        </fieldset>

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

            <input type="checkbox" id="foto" name="documentos" value="foto">
            <label for="foto">Foto 3x4</label>
        </fieldset>

        <fieldset>
            <legend>05) DOCUMENTOS DE INTERESSE FUNCIONÁRIO</legend>
            <label for="documentos_funcionario">Marque os documentos entregues:</label>
            <input type="checkbox" id="certidao_nascimento" name="documentos_funcionario" value="certidao_nascimento">
            <label for="certidao_nascimento">Certidão de Nascimento (Filhos até 07 anos)</label>

            <input type="checkbox" id="cartao_vacina" name="documentos_funcionario" value="cartao_vacina">
            <label for="cartao_vacina">Cartão de Vacina (Filhos até 07 anos)</label>

            <input type="checkbox" id="atestado_escolaridade" name="documentos_funcionario" value="atestado_escolaridade">
            <label for="atestado_escolaridade">Atestado de Escolaridade (Filhos entre 07 e 14 anos)</label>

            <input type="checkbox" id="termo_judicial" name="documentos_funcionario" value="termo_judicial">
            <label for="termo_judicial">Filho Adotivo - Comprovação de Termo Judicial</label>

            <input type="checkbox" id="certidao_casamento" name="documentos_funcionario" value="certidao_casamento">
            <label for="certidao_casamento">Certidão de Casamento ou Averbação Judicial</label>

            <input type="checkbox" id="cpf_filhos" name="documentos_funcionario" value="cpf_filhos">
            <label for="cpf_filhos">CPF dos Filhos</label>
        </fieldset>

        <div>
            <label for="assinatura_funcionario">Assinatura do Funcionário:</label>
            <input type="text" id="assinatura_funcionario" name="assinatura_funcionario">
        </div>

        <div>
            <label for="assinatura_empresa">Assinatura da Empresa:</label>
            <input type="text" id="assinatura_empresa" name="assinatura_empresa">
        </div>

        <button type="submit">Enviar Ficha de Admissão</button>
    </form>
</body>
</html>
