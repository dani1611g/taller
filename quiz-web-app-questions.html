<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz Interactivo con Preguntas</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        .header {
            text-align: center;
            padding: 20px 0;
            background-color: #4a4a4a;
            color: white;
            border-radius: 10px;
            margin-bottom: 30px;
        }
        .qr-section {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 40px;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        #qrcode {
            margin: 20px 0;
        }
        .controls {
            display: flex;
            justify-content: center;
            margin-bottom: 20px;
        }
        .stats {
            display: flex;
            justify-content: space-around;
            margin-top: 20px;
        }
        .stat-box {
            text-align: center;
            background-color: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            width: 30%;
        }
        .stat-box h3 {
            margin-top: 0;
            color: #4a4a4a;
        }
        .stat-box p {
            font-size: 24px;
            font-weight: bold;
            color: #2c3e50;
        }
        .btn {
            padding: 10px 20px;
            margin: 0 10px;
            background-color: #3498db;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }
        .btn:hover {
            background-color: #2980b9;
        }
        .btn-reset {
            background-color: #e74c3c;
        }
        .btn-reset:hover {
            background-color: #c0392b;
        }
        
        /* Estilos para la página móvil */
        .mobile-container {
            max-width: 500px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
        }
        .category-btn {
            display: block;
            width: 100%;
            padding: 20px;
            margin: 15px 0;
            background-color: #3498db;
            color: white;
            border: none;
            border-radius: 10px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.2s, background-color 0.3s;
        }
        .category-btn:hover {
            transform: scale(1.02);
        }
        .vehicles {
            background-color: #e74c3c;
        }
        .pilot {
            background-color: #2ecc71;
        }
        .cross {
            background-color: #f39c12;
        }
        .thank-you {
            display: none;
            padding: 50px 20px;
            background-color: #2ecc71;
            color: white;
            border-radius: 10px;
            margin-top: 20px;
        }
        .results-container {
            margin-top: 40px;
            padding: 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .results-bar {
            display: flex;
            justify-content: space-between;
            margin-bottom: 15px;
        }
        .bar-label {
            width: 100px;
            text-align: left;
        }
        .bar-container {
            flex-grow: 1;
            background-color: #ecf0f1;
            margin: 0 15px;
            border-radius: 5px;
            overflow: hidden;
        }
        .bar {
            height: 30px;
            line-height: 30px;
            color: white;
            text-align: right;
            padding-right: 10px;
            border-radius: 5px;
            transition: width 1s ease-in-out;
        }
        .vehicles-bar {
            background-color: #e74c3c;
        }
        .pilot-bar {
            background-color: #2ecc71;
        }
        .cross-bar {
            background-color: #f39c12;
        }
        .bar-value {
            width: 50px;
            text-align: right;
        }
        
        /* Estilos para el formulario de preguntas */
        .question-form {
            display: none;
            margin-top: 30px;
            text-align: left;
        }
        .form-group {
            margin-bottom: 20px;
        }
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
        }
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            resize: vertical;
            min-height: 100px;
            font-family: inherit;
            font-size: 16px;
        }
        .submit-btn {
            padding: 12px 25px;
            background-color: #3498db;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
            display: block;
            width: 100%;
            margin-top: 20px;
        }
        .submit-btn:hover {
            background-color: #2980b9;
        }
        
        /* Estilos para mostrar las preguntas en la vista del presentador */
        .questions-list {
            margin-top: 30px;
            max-height: 400px;
            overflow-y: auto;
        }
        .question-card {
            background-color: white;
            border-left: 5px solid #3498db;
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .question-card.vehicles {
            border-left-color: #e74c3c;
        }
        .question-card.pilot {
            border-left-color: #2ecc71;
        }
        .question-card.cross {
            border-left-color: #f39c12;
        }
        .question-category {
            font-size: 12px;
            text-transform: uppercase;
            color: #7f8c8d;
            margin-bottom: 5px;
        }
        .question-text {
            font-size: 16px;
            color: #2c3e50;
        }
        .no-questions {
            text-align: center;
            color: #7f8c8d;
            padding: 20px;
        }
        .question-filter {
            display: flex;
            justify-content: center;
            margin-bottom: 15px;
        }
        .filter-btn {
            padding: 8px 15px;
            margin: 0 5px;
            background-color: #ecf0f1;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 14px;
            transition: background-color 0.3s;
        }
        .filter-btn.active {
            background-color: #3498db;
            color: white;
        }
        .filter-btn.vehicles.active {
            background-color: #e74c3c;
        }
        .filter-btn.pilot.active {
            background-color: #2ecc71;
        }
        .filter-btn.cross.active {
            background-color: #f39c12;
        }
    </style>
</head>
<body>
    <div id="presenter-view">
        <div class="container">
            <div class="header">
                <h1>Quiz Interactivo</h1>
                <p>Escanea el código QR para participar</p>
            </div>
            
            <div class="qr-section">
                <h2>Código QR para participar</h2>
                <div id="qrcode"></div>
                <p>O visita: <span id="page-url">https://tu-quiz.com/participar</span></p>
            </div>
            
            <div class="controls">
                <button class="btn" id="start-btn">Iniciar sesión</button>
                <button class="btn btn-reset" id="reset-btn">Reiniciar</button>
            </div>
            
            <div class="results-container">
                <h2>Estadísticas de Categorías</h2>
                
                <div class="results-bar">
                    <div class="bar-label">Vehículos</div>
                    <div class="bar-container">
                        <div class="bar vehicles-bar" id="vehicles-bar" style="width: 0%">0</div>
                    </div>
                    <div class="bar-value" id="vehicles-value">0</div>
                </div>
                
                <div class="results-bar">
                    <div class="bar-label">Piloto</div>
                    <div class="bar-container">
                        <div class="bar pilot-bar" id="pilot-bar" style="width: 0%">0</div>
                    </div>
                    <div class="bar-value" id="pilot-value">0</div>
                </div>
                
                <div class="results-bar">
                    <div class="bar-label">Cross</div>
                    <div class="bar-container">
                        <div class="bar cross-bar" id="cross-bar" style="width: 0%">0</div>
                    </div>
                    <div class="bar-value" id="cross-value">0</div>
                </div>
            </div>
            
            <div class="stats">
                <div class="stat-box">
                    <h3>Participantes</h3>
                    <p id="participants-count">0</p>
                </div>
                <div class="stat-box">
                    <h3>Preguntas</h3>
                    <p id="questions-count">0</p>
                </div>
                <div class="stat-box">
                    <h3>Categoría popular</h3>
                    <p id="popular-category">-</p>
                </div>
            </div>
            
            <!-- Sección para mostrar las preguntas -->
            <div class="results-container">
                <h2>Preguntas de los participantes</h2>
                
                <div class="question-filter">
                    <button class="filter-btn active" data-filter="all">Todas</button>
                    <button class="filter-btn vehicles" data-filter="vehicles">Vehículos</button>
                    <button class="filter-btn pilot" data-filter="pilot">Piloto</button>
                    <button class="filter-btn cross" data-filter="cross">Cross</button>
                </div>
                
                <div class="questions-list" id="questions-list">
                    <div class="no-questions" id="no-questions">
                        No hay preguntas todavía.
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Vista móvil para participantes -->
    <div id="participant-view" style="display: none;">
        <div class="mobile-container">
            <h1>Selecciona una categoría</h1>
            <p>¿Sobre qué tema prefieres hacer preguntas?</p>
            
            <button class="category-btn vehicles" id="vehicles-btn">Vehículos</button>
            <button class="category-btn pilot" id="pilot-btn">Piloto</button>
            <button class="category-btn cross" id="cross-btn">Cross</button>
            
            <!-- Formulario para enviar pregunta -->
            <div class="question-form" id="question-form">
                <h2>Envía tu pregunta sobre <span id="selected-category">-</span></h2>
                <div class="form-group">
                    <label for="question-text">Escribe tu pregunta:</label>
                    <textarea id="question-text" placeholder="Escribe aquí tu pregunta..."></textarea>
                </div>
                <button class="submit-btn" id="submit-question">Enviar pregunta</button>
            </div>
            
            <div class="thank-you" id="thank-you">
                <h2>¡Gracias por tu participación!</h2>
                <p>Tu pregunta ha sido enviada correctamente.</p>
            </div>
        </div>
    </div>

    <script>
        // Determinar si es presentador o participante
        const isParticipant = window.location.search.includes('mode=participant');
        
        // Variables para almacenar los datos
        let votes = {
            vehicles: 0,
            pilot: 0,
            cross: 0
        };
        
        let participants = 0;
        let questions = [];
        let currentFilter = 'all';
        let selectedCategory = '';
        
        // Función para actualizar la URL y el código QR
        function updateQRCode() {
            const currentURL = window.location.href.split('?')[0];
            const participantURL = currentURL + '?mode=participant';
            
            document.getElementById('page-url').textContent = participantURL;
            
            // Generar código QR
            const qrcode = new QRCode(document.getElementById('qrcode'), {
                text: participantURL,
                width: 200,
                height: 200,
                colorDark: '#000000',
                colorLight: '#ffffff',
                correctLevel: QRCode.CorrectLevel.H
            });
        }
        
        // Función para actualizar las estadísticas
        function updateStats() {
            const totalVotes = votes.vehicles + votes.pilot + votes.cross;
            
            // Actualizar contadores
            document.getElementById('participants-count').textContent = participants;
            document.getElementById('questions-count').textContent = questions.length;
            
            // Actualizar barras de progreso
            if (totalVotes > 0) {
                document.getElementById('vehicles-bar').style.width = (votes.vehicles / totalVotes * 100) + '%';
                document.getElementById('pilot-bar').style.width = (votes.pilot / totalVotes * 100) + '%';
                document.getElementById('cross-bar').style.width = (votes.cross / totalVotes * 100) + '%';
                
                document.getElementById('vehicles-bar').textContent = votes.vehicles;
                document.getElementById('pilot-bar').textContent = votes.pilot;
                document.getElementById('cross-bar').textContent = votes.cross;
                
                document.getElementById('vehicles-value').textContent = votes.vehicles;
                document.getElementById('pilot-value').textContent = votes.pilot;
                document.getElementById('cross-value').textContent = votes.cross;
                
                // Determinar categoría más popular
                let popularCategory = 'Ninguna';
                let maxVotes = 0;
                
                if (votes.vehicles > maxVotes) {
                    maxVotes = votes.vehicles;
                    popularCategory = 'Vehículos';
                }
                if (votes.pilot > maxVotes) {
                    maxVotes = votes.pilot;
                    popularCategory = 'Piloto';
                }
                if (votes.cross > maxVotes) {
                    maxVotes = votes.cross;
                    popularCategory = 'Cross';
                }
                
                document.getElementById('popular-category').textContent = popularCategory;
            }
        }
        
        // Función para mostrar las preguntas en la vista del presentador
        function updateQuestionsList() {
            const questionsList = document.getElementById('questions-list');
            const noQuestionsElement = document.getElementById('no-questions');
            
            // Limpiar la lista
            questionsList.innerHTML = '';
            
            // Mostrar mensaje si no hay preguntas
            if (questions.length === 0) {
                questionsList.appendChild(noQuestionsElement);
                return;
            }
            
            // Filtrar las preguntas según la categoría seleccionada
            const filteredQuestions = currentFilter === 'all' 
                ? questions 
                : questions.filter(q => q.category === currentFilter);
            
            // Mostrar mensaje si no hay preguntas en la categoría filtrada
            if (filteredQuestions.length === 0) {
                const noFilteredQuestions = document.createElement('div');
                noFilteredQuestions.className = 'no-questions';
                noFilteredQuestions.textContent = 'No hay preguntas en esta categoría.';
                questionsList.appendChild(noFilteredQuestions);
                return;
            }
            
            // Agregar cada pregunta a la lista
            filteredQuestions.forEach(question => {
                const questionCard = document.createElement('div');
                questionCard.className = `question-card ${question.category}`;
                
                const categoryName = {
                    'vehicles': 'Vehículos',
                    'pilot': 'Piloto',
                    'cross': 'Cross'
                };
                
                questionCard.innerHTML = `
                    <div class="question-category">${categoryName[question.category]}</div>
                    <div class="question-text">${question.text}</div>
                `;
                
                questionsList.appendChild(questionCard);
            });
        }
        
        // Función para simular el almacenamiento en el servidor
        function simulateServerStorage(category, questionText) {
            // Incrementar contadores
            participants++;
            votes[category]++;
            
            // Añadir la pregunta a la lista
            questions.push({
                id: Date.now(),
                category: category,
                text: questionText,
                timestamp: new Date().toISOString()
            });
            
            // Actualizar estadísticas y lista de preguntas
            updateStats();
            updateQuestionsList();
        }
        
        // Inicializar la página según el modo
        window.onload = function() {
            if (isParticipant) {
                // Mostrar vista de participante
                document.getElementById('presenter-view').style.display = 'none';
                document.getElementById('participant-view').style.display = 'block';
                
                // Configurar botones de categorías
                document.getElementById('vehicles-btn').addEventListener('click', function() {
                    selectCategory('vehicles', 'Vehículos');
                });
                
                document.getElementById('pilot-btn').addEventListener('click', function() {
                    selectCategory('pilot', 'Piloto');
                });
                
                document.getElementById('cross-btn').addEventListener('click', function() {
                    selectCategory('cross', 'Cross');
                });
                
                // Configurar envío de pregunta
                document.getElementById('submit-question').addEventListener('click', function() {
                    const questionText = document.getElementById('question-text').value.trim();
                    
                    if (questionText) {
                        submitQuestion(questionText);
                    } else {
                        alert('Por favor, escribe una pregunta antes de enviar.');
                    }
                });
            } else {
                // Mostrar vista de presentador
                updateQRCode();
                
                // Configurar botones de control
                document.getElementById('reset-btn').addEventListener('click', function() {
                    votes = { vehicles: 0, pilot: 0, cross: 0 };
                    participants = 0;
                    questions = [];
                    updateStats();
                    updateQuestionsList();
                });
                
                // Configurar filtros de preguntas
                const filterButtons = document.querySelectorAll('.filter-btn');
                filterButtons.forEach(button => {
                    button.addEventListener('click', function() {
                        // Remover clase activa de todos los botones
                        filterButtons.forEach(btn => btn.classList.remove('active'));
                        // Añadir clase activa al botón seleccionado
                        this.classList.add('active');
                        // Actualizar filtro
                        currentFilter = this.getAttribute('data-filter');
                        // Actualizar lista de preguntas
                        updateQuestionsList();
                    });
                });
                
                // Para demostración, simular algunas preguntas
                document.getElementById('start-btn').addEventListener('click', function() {
                    const demoQuestions = [
                        { category: 'vehicles', text: '¿Cuál es la marca de tu moto favorita?' },
                        { category: 'pilot', text: '¿Qué equipamiento es indispensable para un piloto principiante?' },
                        { category: 'cross', text: '¿Cuál es la diferencia entre motocross y enduro?' },
                        { category: 'vehicles', text: '¿Qué tipo de mantenimiento requiere una moto de cross?' },
                        { category: 'pilot', text: '¿Cómo se debe preparar físicamente un piloto de motocross?' }
                    ];
                    
                    let index = 0;
                    const intervalId = setInterval(function() {
                        if (index < demoQuestions.length) {
                            const demo = demoQuestions[index];
                            simulateServerStorage(demo.category, demo.text);
                            index++;
                        } else {
                            clearInterval(intervalId);
                        }
                    }, 2000);
                });
            }
        };
        
        // Función para seleccionar categoría
        function selectCategory(category, categoryName) {
            selectedCategory = category;
            
            // Ocultar botones de categoría
            document.getElementById('vehicles-btn').style.display = 'none';
            document.getElementById('pilot-btn').style.display = 'none';
            document.getElementById('cross-btn').style.display = 'none';
            
            // Actualizar el título con la categoría seleccionada
            document.getElementById('selected-category').textContent = categoryName;
            
            // Mostrar formulario de pregunta
            document.getElementById('question-form').style.display = 'block';
        }
        
        // Función para enviar la pregunta
        function submitQuestion(questionText) {
            // Ocultar formulario
            document.getElementById('question-form').style.display = 'none';
            
            // Mostrar mensaje de agradecimiento
            document.getElementById('thank-you').style.display = 'block';
            
            // En una implementación real, enviaría los datos al servidor
            console.log('Pregunta enviada:', selectedCategory, questionText);
            
            // Simular almacenamiento en servidor
            // En una implementación real, esto sería manejado por el servidor
            simulateServerStorage(selectedCategory, questionText);
        }
    </script>
</body>
</html>
