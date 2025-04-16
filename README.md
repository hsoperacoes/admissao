<style>
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background-color: #f4f6f8;
        margin: 0;
        padding: 30px;
    }

    h1 {
        text-align: center;
        color: #333;
        font-size: 28px;
        margin-bottom: 30px;
    }

    form {
        max-width: 900px;
        margin: 0 auto;
        background-color: white;
        padding: 30px;
        border-radius: 12px;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    fieldset {
        border: none;
        margin-bottom: 25px;
        padding: 0;
    }

    legend {
        font-size: 20px;
        font-weight: bold;
        color: #2c3e50;
        margin-bottom: 10px;
    }

    label {
        display: block;
        margin-top: 15px;
        font-weight: 500;
        color: #333;
    }

    input[type="text"],
    input[type="date"],
    input[type="number"],
    input[type="time"],
    select {
        width: 100%;
        padding: 10px;
        margin-top: 5px;
        border: 1px solid #ccc;
        border-radius: 6px;
        background-color: #fff;
    }

    input[type="checkbox"],
    input[type="radio"] {
        margin-right: 6px;
        transform: scale(1.2);
    }

    .row {
        display: flex;
        gap: 20px;
        margin-top: 10px;
    }

    .col {
        flex: 1;
    }

    button {
        display: block;
        margin: 30px auto 0;
        background-color: #2ecc71;
        color: white;
        font-size: 18px;
        padding: 12px 30px;
        border: none;
        border-radius: 8px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }

    button:hover {
        background-color: #27ae60;
    }

    p {
        font-size: 14px;
        color: #666;
        margin-top: 5px;
    }

    .checkbox-group,
    .radio-group {
        display: flex;
        flex-wrap: wrap;
        gap: 15px;
        margin-top: 10px;
    }

    .checkbox-group label,
    .radio-group label {
        display: flex;
        align-items: center;
        font-weight: normal;
        margin-top: 0;
    }

    @media (max-width: 600px) {
        .row {
            flex-direction: column;
        }
    }
</style>
