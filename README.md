<!DOCTYPE html>
<html lang="pt-br">    
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gerenciador de Atividades</title>
    <link rel="stylesheet" href="gerenciador.css">
</head>
<body>
    <header>
        <h1>Gerenciador de Atividades dos Colaboradores</h1>
        <img src="C:\U" alt="Downloads\Vtl_logo.jpg">
    </header>
    <main>
        <section class="form-section">
            <h2>Adicionar Informações</h2>
            <form id="activityForm">
                <input type="Date" id="activityDate" placeholder="Data" required>
                <input type="time" id="activityHorario" placeholder="Hora de Entrada" required>
                <input type="time" id="activityHorario" placeholder="Hora de Saída" required>
                <input type="text" id="collaboratorName" placeholder="Nome do Colaborador" required>
                <label for="cpf">CPF:</label>
                <input type="text" id="cpf" name="cpf" 
               placeholder="000.000.000-00" 
               maxlength="14" 
               pattern="\d{3}\.\d{3}\.\d{3}-\d{2}" 
               title="Digite um CPF no formato: 000.000.000-00" 
               required>
               <input type="text" id="activityName" placeholder="Nome da Atividade" required>
               </p>
        </form>
               <label for="celular">Número de Celular:</label>
               <input type="tel" id="celular" name="celular" 
               placeholder="(XX) XXXXX-XXXX" 
               pattern="\(\d{2}\) \d{5}-\d{4}" 
               title="Digite um número de celular no formato: (XX) XXXXX-XXXX" 
               required>
                <input type="text" id="room" placeholder="Sala de Transmissão" required>
                <input type="text" id="activityName" placeholder="Empresa" required>
                <input type="text" id="collaboratorName" placeholder="responsável pela atividade" required>
                <input type="text" id="activityName" placeholder="Materiais utilizados"required><br>
                <label for="metragem">Metragem de Cordões:</label>
        <input type="number" id="metragem" name="metragem" 
               placeholder="Insira a metragem" 
               min="0.1" step="0.1" 
               title="Insira a metragem de cordões em metros"
               required>
        <input type="text" id="activityName" placeholder="De Fila número e letra"required><br>
        <label for="bastidor">Bastidor:</label>
        <input type="number" id="bastidor" name="bastidor" 
               pattern="[A-Za-z]" maxlength="1" required>
        <br>
        <input type="text" id="activityName" placeholder="Para Fila número e letra" required>
        <label for="bastidor">Bastidor:</label>
        <input type="number" id="bastidor" name="bastidor" 
               pattern="[A-Za-z]" maxlength="1" required><br>
       <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Botão Azul</title>
    <link rel="stylesheet" href="gerenciador.html">
</head>
<body><br>
<!-- Botão de envio -->
    <form action="/sua-action" method="post">
        <button type="submit" id="botao-enviar">Enviar</button>
    </form>

        </form>
        </section>
        <section class="activities-section">
            <h2>Atividades Registradas</h2>
            <table id="activitiesTable">
                <thead>
                    <tr>
                        <th>Atividade</th>
                        <th>Colaborador</th>
                        <th>Sala de Transmissão</th>
                    </tr>
                </thead>
                <tbody>
                    <!-- As atividades serão inseridas aqui -->
                </tbody>
            </table>
        </section>
    </main>
</body>
</html>

#Código em css#

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #007bff;
    color: white;
    padding: 20px;
    text-align: center;
}

main {
    margin: 20px;
}

h2 {
    color: #333;
}

.form-section, .activities-section {
    background-color: white;
    padding: 20px;
    margin-bottom: 20px;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

form {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
}

/* Estilo básico para inputs */
input[type="text"] {
    width: 100%; /* Largura completa para ocupar o contêiner */
    padding: 8px 12px; /* Espaçamento interno para o texto não ficar muito colado nas bordas */
    margin: 8px 0; /* Margem para separar os inputs um do outro */
    box-sizing: border-box; /* Garante que o padding e a borda sejam incluídos na largura total */
    border: 1px solid #ccc; /* Cor da borda */
    border-radius: 4px; /* Bordas arredondadas */
    background-color: #f8f8f8; /* Cor de fundo do input */
    font-size: 16px; /* Tamanho da fonte */
}

/* Estilo do input quando estiver em foco */
input[type="text"]:focus {
    border-color: #4A90E2; /* Muda a cor da borda para azul */
    outline: none; /* Remove o contorno padrão do navegador */
}

form button {
    background-color: #007bff; /* Azul */
    color: white; /* Texto branco */
    padding: 10px 20px; /* Espaçamento interno */
    border: none; /* Sem borda */
    border-radius: 5px; /* Bordas arredondadas */
    cursor: pointer; /* Cursor do mouse como ponteiro */
    font-size: 16px; /* Tamanho do texto */
    transition: background-color 0.2s; /* Transição suave para mudança de cor */
}

#botao-enviar:hover {
    background-color: #0056b3; /* Azul mais escuro ao passar o mouse */
}


table {
    width: 100%;
    border-collapse: collapse;
}

table, th, td {
    border: 1px solid #ddd;
}

th, td {
    padding: 10px;
    text-align: left;
}

th {
    background-color: #007bff;
    color: white;
}
