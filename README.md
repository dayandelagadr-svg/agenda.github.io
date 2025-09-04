# agenda.github.io
agenda 2025/2026
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agenda 2026 - Unicornia</title>
    <!-- Fonts para el nuevo diseño -->
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            /* Paleta de colores inspirada en la imagen */
            --color-pink: #f5cde2;
            --color-light-purple: #d4a0f8;
            --color-mint: #b2e6d6;
            --color-blue: #a0d4f8;
            --color-white: #ffffff;
            --color-gray: #555555;
            --color-text: #3c3c3c;
        }

        body {
            font-family: 'Poppins', sans-serif;
            /* Fondo de franjas diagonales como en la imagen */
            background: linear-gradient(45deg, var(--color-light-purple) 25%, var(--color-mint) 25%, var(--color-mint) 50%, var(--color-blue) 50%, var(--color-blue) 75%, var(--color-pink) 75%, var(--color-pink) 100%);
            color: var(--color-text);
            margin: 0;
            padding: 2rem;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            min-height: 10vh;
        }

        .agenda-container {
            background-color: var(--color-white);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            padding: 3rem;
            max-width: 900px;
            width: 100%;
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }

        h1, h2, h3 {
            color: var(--color-text);
            font-weight: 700;
        }

        h1 {
            font-size: 2.5rem;
            text-align: center;
            color: var(--color-light-purple);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
            margin-bottom: 0;
        }
        
        .slogan {
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
            text-align: center;
            color: var(--color-pink);
            margin-top: 0;
            margin-bottom: 2rem;
        }

        h2 {
            font-size: 2rem;
            color: var(--color-light-purple);
            border-bottom: 2px solid var(--color-pink);
            padding-bottom: 0.5rem;
            margin-top: 2rem;
        }

        h3 {
            font-size: 1.5rem;
            color: var(--color-blue);
            margin-top: 1.5rem;
            border-left: 4px solid var(--color-blue);
            padding-left: 10px;
        }

        ul {
            list-style: none;
            padding-left: 0;
            margin-top: 0.5rem;
        }

        ul li:before {
            content: '✨';
            position: absolute;
            left: 0;
            top: 2px;
        }

        hr {
            border: 0;
            height: 2px;
            background: linear-gradient(90deg, var(--color-light-purple), var(--color-pink));
            margin: 3rem 0;
        }

        .image-container {
            text-align: center;
            margin: 2rem 0;
        }

        .image-container img {
            max-width: 100%;
            height: auto;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .print-button {
            display: block;
            margin: 2rem auto;
            padding: 1rem 2rem;
            font-size: 1.2rem;
            font-weight: 600;
            background: linear-gradient(45deg, var(--color-pink), var(--color-light-purple));
            color: var(--color-white);
            border: none;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .print-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
        }
        
        /* Estilos específicos para impresión */
        @media print {
            body {
                background: none;
                padding: 0;
            }

            .agenda-container {
                box-shadow: none;
                border-radius: 0;
                padding: 0;
            }

            .print-button {
                display: none; /* Oculta el botón al imprimir */
            }

            h1, h2, h3, .slogan, .finance-title, .finance-box h4 {
                color: #000; /* Color de tinta estándar para impresión */
            }

            ul li:before {
                content: ''; /* Oculta los emojis */
            }

            .finance-box {
                border-color: #000;
            }
            .clean-plan-table th,
            .clean-plan-table td {
                border: 1px solid black;
            }

            .time-management-grid .card {
                border-color: #000;
            }
        }

        .finance-title {
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
            text-align: center;
            margin-top: 2rem;
            margin-bottom: 1rem;
            color: var(--color-light-purple);
        }

        .finance-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 1.5rem;
        }

        .finance-box {
            border: 2px solid var(--color-light-purple);
            border-radius: 10px;
            padding: 1.5rem;
        }

        .finance-box h4 {
            font-family: 'Poppins', sans-serif;
            font-size: 1.2rem;
            text-align: center;
            margin: 0 0 1.5rem 0;
            color: var(--color-pink);
        }

        .finance-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }

        .finance-item input[type="checkbox"] {
            -webkit-appearance: none;
            -moz-appearance: none;
            appearance: none;
            width: 1.2rem;
            height: 1.2rem;
            border: 2px solid var(--color-light-purple);
            border-radius: 3px;
            cursor: pointer;
            outline: none;
            position: relative;
        }

        .finance-item input[type="checkbox"]:checked {
            background-color: var(--color-light-purple);
        }

        .finance-item input[type="checkbox"]:checked:after {
            content: '✔';
            color: var(--color-white);
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 0.8rem;
        }

        .finance-item .line {
            flex-grow: 1;
            height: 1px;
            background-color: var(--color-gray);
            margin: 0 0.5rem;
        }

        .finance-table {
            margin-top: 2rem;
        }

        .finance-table h4 {
            font-size: 1.2rem;
            text-align: left;
            margin-bottom: 1.5rem;
            color: var(--color-pink);
        }

        .finance-table .header {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            font-weight: 600;
            border-bottom: 2px solid var(--color-mint);
            padding-bottom: 0.75rem;
        }

        .finance-table .row {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            padding: 1rem 0;
            border-bottom: 1px dotted var(--color-gray);
        }

        .summary-boxes {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 1.5rem;
            margin-top: 3rem;
            text-align: center;
        }

        .summary-box {
            border: 2px solid var(--color-blue);
            border-radius: 10px;
            padding: 0.75rem;
        }

        .summary-box p {
            margin: 0;
            font-weight: 600;
        }

        /* Estilos para la tabla de plan de limpieza */
        .clean-plan-section {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .clean-plan-section h2 {
            text-align: center;
            color: var(--color-light-purple);
            border-bottom: none;
        }

        .clean-plan-table {
            border-collapse: collapse;
            width: 100%;
            margin-bottom: 1rem;
            font-size: 0.9rem;
        }

        .clean-plan-table th,
        .clean-plan-table td {
            border: 1px solid var(--color-gray);
            padding: 0.75rem;
            text-align: center;
        }

        .clean-plan-table th {
            background-color: var(--color-mint);
            color: var(--color-white);
            font-weight: 600;
        }

        .clean-plan-table td:first-child {
            text-align: left;
            font-weight: 500;
        }
        
        .clean-plan-table .daily-tasks td:first-child { background-color: var(--color-pink); }
        .clean-plan-table .weekly-tasks td:first-child { background-color: var(--color-blue); }
        .clean-plan-table .biweekly-tasks td:first-child { background-color: var(--color-mint); }
        .clean-plan-table .monthly-tasks td:first-child { background-color: var(--color-light-purple); }
        .clean-plan-table .eventual-tasks td:first-child { background-color: var(--color-pink); }

        .clean-plan-table .daily-tasks td { background-color: #fce7f4; }
        .clean-plan-table .weekly-tasks td { background-color: #e0f2fe; }
        .clean-plan-table .biweekly-tasks td { background-color: #e6f9f0; }
        .clean-plan-table .monthly-tasks td { background-color: #f1e0fc; }
        .clean-plan-table .eventual-tasks td { background-color: #fde7f4; }

        .clean-plan-table .clean-header {
            font-weight: 600;
            text-align: center;
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
            color: var(--color-text);
        }
        
        .clean-plan-section .note-box {
            border: 2px solid var(--color-blue);
            border-radius: 10px;
            padding: 1rem;
            margin-top: 1rem;
            height: 150px;
        }

        /* Estilos para la sección de Gestión de Tiempo */
        .time-management-section {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 2rem 0;
        }

        .time-management-section h2 {
            text-align: center;
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            color: var(--color-light-purple);
            border-bottom: none;
            margin-bottom: 1rem;
        }

        .time-management-section p.subtitle {
            text-align: center;
            font-size: 1rem;
            color: var(--color-gray);
            margin-bottom: 2rem;
        }

        .time-management-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 1.5rem;
        }
        
        .time-management-grid .card {
            border: 2px solid var(--color-light-purple);
            border-radius: 15px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .time-management-grid .card h4 {
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 1.2rem;
            margin: 0 0 0.5rem 0;
            color: var(--color-pink);
        }

        .time-management-grid .card p {
            font-size: 0.9rem;
            line-height: 1.4;
            color: var(--color-gray);
            margin: 0;
        }

        .card.regla { border-color: var(--color-pink); }
        .card.sapo { border-color: var(--color-mint); }
        .card.pomodoro { border-color: var(--color-blue); }
        .card.lista { border-color: var(--color-light-purple); }
        .card.delegar { border-color: var(--color-mint); }
        .card.apps { border-color: var(--color-blue); }
        .card.limites { border-color: var(--color-pink); }
        .card.calendario { border-color: var(--color-light-purple); }
        .card.cuidado { border-color: var(--color-mint); }
        .card.redes { border-color: var(--color-blue); }
        .card.multitarea { border-color: var(--color-pink); }
        .card.revision { border-color: var(--color-light-purple); }
        
        /* Estilos para el calendario anual */
        .calendar-section {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 2rem 0;
        }

        .calendar-section h2 {
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            color: var(--color-light-purple);
            border-bottom: none;
            margin-bottom: 1rem;
        }

        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 1.5rem;
            width: 100%;
        }

        .month-box {
            border: 2px solid var(--color-mint);
            border-radius: 10px;
            padding: 1rem;
            text-align: center;
        }

        .month-box h4 {
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 1.2rem;
            margin: 0 0 0.5rem 0;
            color: var(--color-pink);
        }

        .month-image {
            width: 100%;
            height: 100px;
            background-color: var(--color-pink);
            border-radius: 8px;
            margin-bottom: 0.5rem;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--color-white);
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
        }
        
        .month-days {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 5px;
            font-size: 0.8rem;
        }

        .month-days .day {
            text-align: center;
        }

        .day-label {
            font-weight: 600;
            color: var(--color-text);
        }
        
        .holiday {
            background-color: var(--color-pink);
            color: var(--color-white);
            border-radius: 50%;
            display: inline-flex;
            width: 1.5em;
            height: 1.5em;
            align-items: center;
            justify-content: center;
            font-weight: 600;
        }

        /* Estilos para el Tablero de Metas */
        .goals-section {
            padding: 2rem 0;
        }
        .goals-section h2 {
            text-align: center;
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            color: var(--color-light-purple);
            border-bottom: none;
            margin-bottom: 1rem;
        }
        .goals-section .subtitle {
            text-align: center;
            font-size: 1rem;
            color: var(--color-gray);
            margin-bottom: 2rem;
        }
        .goals-grid {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 1.5rem;
            border: 2px solid var(--color-light-purple);
            border-radius: 15px;
            padding: 1.5rem;
        }
        .goal-category {
            font-weight: 600;
            font-size: 1.1rem;
            color: var(--color-pink);
        }
        .goal-item {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
        }
        .goal-item input {
            flex-grow: 1;
            border: none;
            border-bottom: 1px solid var(--color-gray);
            outline: none;
        }
        .strategy-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 10px;
        }
        .strategy-item .line {
            flex-grow: 1;
            border-bottom: 1px solid var(--color-gray);
        }
        .meta-check {
            width: 20px;
            height: 20px;
            border: 1px solid var(--color-gray);
            display: inline-block;
        }

        /* Estilos para Notas Rápidas */
        .notes-section {
            padding: 2rem 0;
        }
        .notes-section h2 {
            text-align: center;
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            color: var(--color-light-purple);
            border-bottom: none;
            margin-bottom: 1rem;
        }
        .notes-box {
            border: 2px solid var(--color-mint);
            border-radius: 15px;
            padding: 1.5rem;
            min-height: 200px;
        }

        /* Estilos para el Registro de Hábitos */
        .habit-tracker-section {
            padding: 2rem 0;
        }
        .habit-tracker-section h2 {
            text-align: center;
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            color: var(--color-light-purple);
            border-bottom: none;
            margin-bottom: 1rem;
        }
        .habit-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 1rem;
            width: 100%;
        }
        .habit-box {
            border: 2px solid var(--color-blue);
            border-radius: 10px;
            padding: 1rem;
            text-align: center;
        }
        .habit-box h4 {
            font-family: 'Poppins', sans-serif;
            font-weight: 600;
            font-size: 1.1rem;
            margin-top: 0;
            margin-bottom: 0.5rem;
            color: var(--color-pink);
        }
        .habit-days {
            display: flex;
            flex-wrap: wrap;
            gap: 5px;
        }
        .habit-day {
            width: 15px;
            height: 15px;
            border: 1px solid var(--color-gray);
            border-radius: 3px;
        }

        /* Estilos para Contactos Importantes */
        .contacts-section {
            padding: 2rem 0;
        }
        .contacts-section h2 {
            text-align: center;
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            color: var(--color-light-purple);
            border-bottom: none;
            margin-bottom: 1rem;
        }
        .contact-item {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 1rem;
            align-items: center;
            margin-bottom: 1rem;
        }
        .contact-item label {
            font-weight: 600;
            color: var(--color-blue);
        }
        .contact-item input {
            border: none;
            border-bottom: 1px solid var(--color-gray);
            outline: none;
        }

        /* Estilos para Plan de Alimentación Semanal */
        .meal-plan-section {
            padding: 2rem 0;
        }
        .meal-plan-section h2 {
            text-align: center;
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            color: var(--color-light-purple);
            border-bottom: none;
            margin-bottom: 1rem;
        }
        .meal-plan-table {
            border-collapse: collapse;
            width: 100%;
            margin-bottom: 1rem;
        }
        .meal-plan-table th, .meal-plan-table td {
            border: 1px solid var(--color-gray);
            padding: 1rem;
            text-align: center;
            font-size: 0.9rem;
        }
        .meal-plan-table th {
            background-color: var(--color-mint);
            color: var(--color-white);
            font-weight: 600;
        }
        .meal-plan-table td {
            background-color: #f1e0fc;
            vertical-align: top;
            height: 80px;
        }
        .meal-plan-table tr:first-child th {
            background-color: var(--color-pink);
        }

        .shopping-list-container {
            display: flex;
            gap: 2rem;
            margin-top: 2rem;
        }
        .shopping-list-box {
            border: 2px solid var(--color-blue);
            border-radius: 10px;
            padding: 1.5rem;
            flex: 1;
        }
        .shopping-list-box h4 {
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--color-pink);
            margin-top: 0;
            margin-bottom: 1rem;
            text-align: center;
        }
        .shopping-list-box ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        .shopping-list-box ul li {
            position: relative;
            padding-left: 20px;
            margin-bottom: 5px;
            border-bottom: 1px dotted var(--color-gray);
        }
        .shopping-list-box ul li:before {
            content: '🛒';
            position: absolute;
            left: 0;
            top: 2px;
        }
        /* Estilos de los días para la agenda principal */
        .day-box {
            border: 2px dashed var(--color-light-purple);
            border-radius: 10px;
            padding: 1rem;
            margin-bottom: 1.2rem;
        }
        .day-box h3 {
            margin: 0 0 0.5rem 0;
            color: var(--color-purple);
        }
        .note-line {
            border-bottom: 1px solid #aaa;
            margin: 0.4rem 0;
            height: 1.2rem;
        }
    </style>
</head>
<body>

<div class="agenda-container">
    <h1>Agenda 2026</h1>
    <p class="slogan">Sueño, Planifico y Actúo</p>

    <div class="image-container">
        <img src="https://placehold.co/800x400/d4a0f8/ffffff?text=Tu+Unicornio+Mágico" alt="Un majestuoso unicornio saltando sobre un arcoíris en las nubes con purpurina y estrellas">
    </div>

    <!-- Nueva sección de Calendario Anual -->
    <hr>
    <div class="calendar-section">
        <h2>CALENDARIO 2026</h2>
        <div class="calendar-grid">
            <!-- Enero -->
            <div class="month-box">
                <h4>Enero</h4>
                <div class="month-image">Unicornio de Invierno</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span></span><span></span><span></span><span class="holiday">1</span><span>2</span><span>3</span>
                    <span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span>
                    <span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span>
                    <span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span>
                    <span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span>
                </div>
            </div>
            <!-- Febrero -->
            <div class="month-box">
                <h4>Febrero</h4>
                <div class="month-image">Unicornio de Amor</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span>1</span><span class="holiday">2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span>
                    <span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span>
                    <span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span>
                    <span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span>
                </div>
            </div>
            <!-- Marzo -->
            <div class="month-box">
                <h4>Marzo</h4>
                <div class="month-image">Unicornio de Primavera</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span>
                    <span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span>
                    <span>15</span><span class="holiday">16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span>
                    <span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span>
                    <span>29</span><span>30</span><span>31</span>
                </div>
            </div>
            <!-- Abril -->
            <div class="month-box">
                <h4>Abril</h4>
                <div class="month-image">Unicornio de Flores</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span></span><span></span><span>1</span><span>2</span><span>3</span><span>4</span>
                    <span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span>
                    <span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span>
                    <span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span>
                    <span>26</span><span>27</span><span>28</span><span>29</span><span>30</span>
                </div>
            </div>
            <!-- Mayo -->
            <div class="month-box">
                <h4>Mayo</h4>
                <div class="month-image">Unicornio del Sol</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span></span><span></span><span></span><span></span><span class="holiday">1</span><span>2</span>
                    <span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span>
                    <span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span>
                    <span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span>
                    <span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span>
                    <span>31</span>
                </div>
            </div>
            <!-- Junio -->
            <div class="month-box">
                <h4>Junio</h4>
                <div class="month-image">Unicornio de las Vacaciones</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span>
                    <span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span>
                    <span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span>
                    <span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span>
                    <span>28</span><span>29</span><span>30</span>
                </div>
            </div>
            <!-- Julio -->
            <div class="month-box">
                <h4>Julio</h4>
                <div class="month-image">Unicornio de Verano</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span></span><span></span><span>1</span><span>2</span><span>3</span><span>4</span>
                    <span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span>
                    <span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span>
                    <span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span>
                    <span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span>
                </div>
            </div>
            <!-- Agosto -->
            <div class="month-box">
                <h4>Agosto</h4>
                <div class="month-image">Unicornio de la Playa</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span></span><span></span><span></span><span></span><span></span><span>1</span>
                    <span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span>
                    <span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span>
                    <span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span>
                    <span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span>
                    <span>30</span><span>31</span>
                </div>
            </div>
            <!-- Septiembre -->
            <div class="month-box">
                <h4>Septiembre</h4>
                <div class="month-image">Unicornio de Otoño</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span></span><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span>
                    <span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span>
                    <span>13</span><span>14</span><span>15</span><span class="holiday">16</span><span>17</span><span>18</span><span>19</span>
                    <span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span>
                    <span>27</span><span>28</span><span>29</span><span>30</span>
                </div>
            </div>
            <!-- Octubre -->
            <div class="month-box">
                <h4>Octubre</h4>
                <div class="month-image">Unicornio de Calabazas</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span></span><span></span><span></span><span>1</span><span>2</span><span>3</span>
                    <span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span>
                    <span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span>
                    <span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span>
                    <span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span>
                </div>
            </div>
            <!-- Noviembre -->
            <div class="month-box">
                <h4>Noviembre</h4>
                <div class="month-image">Unicornio de Estrellas</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span class="holiday">1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span>
                    <span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span>
                    <span>15</span><span class="holiday">16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span>
                    <span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span>
                    <span>29</span><span>30</span>
                </div>
            </div>
            <!-- Diciembre -->
            <div class="month-box">
                <h4>Diciembre</h4>
                <div class="month-image">Unicornio Navideño</div>
                <div class="month-days">
                    <span class="day-label">D</span><span class="day-label">L</span><span class="day-label">M</span><span class="day-label">M</span><span class="day-label">J</span><span class="day-label">V</span><span class="day-label">S</span>
                    <span></span><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span>
                    <span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span>
                    <span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span>
                    <span>21</span><span>22</span><span>23</span><span>24</span><span class="holiday">25</span><span>26</span><span>27</span>
                    <span>28</span><span>29</span><span>30</span><span>31</span>
                </div>
            </div>
        </div>
    </div>
    <hr>
    
    <section id="agenda-content">
        <h2>Enero</h2>
        <div class="day-box">
            <h3>1 de enero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>2 de enero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>3 de enero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>4 de enero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>5 de enero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>6 de enero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>7 de enero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>8 de enero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>9 de enero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>10 de enero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>11 de enero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>12 de enero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>13 de enero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>14 de enero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>15 de enero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>16 de enero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>17 de enero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>18 de enero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>19 de enero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>20 de enero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>21 de enero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>22 de enero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>23 de enero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>24 de enero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>25 de enero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>26 de enero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>27 de enero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>28 de enero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>29 de enero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>30 de enero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>31 de enero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>

        <hr>
        <h2>Febrero</h2>
        <div class="day-box">
            <h3>1 de febrero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>2 de febrero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>3 de febrero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>4 de febrero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>5 de febrero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>6 de febrero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>7 de febrero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>8 de febrero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>9 de febrero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>10 de febrero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>11 de febrero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>12 de febrero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>13 de febrero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>14 de febrero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>15 de febrero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>16 de febrero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>17 de febrero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>18 de febrero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>19 de febrero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>20 de febrero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>21 de febrero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>22 de febrero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>23 de febrero de 2026, Lunes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>24 de febrero de 2026, Martes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>25 de febrero de 2026, Miércoles</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>26 de febrero de 2026, Jueves</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>27 de febrero de 2026, Viernes</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>28 de febrero de 2026, Sábado</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <div class="day-box">
            <h3>29 de febrero de 2026, Domingo</h3>
            <p><strong>Tareas Pendientes:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
            <p><strong>Notas:</strong></p>
            <div class="note-line"></div>
            <div class="note-line"></div>
        </div>
        <!-- Continuar hasta diciembre -->
        <hr>

        <!-- Nueva sección de Finanzas -->
        <h2 class="finance-title">Diario de finanzas</h2>

        <div class="finance-grid" style="grid-template-columns: repeat(3, 1fr);">
            <div class="finance-box">
                <h4>INGRESOS SEMANALES</h4>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
            </div>
            <div class="finance-box">
                <h4>INGRESOS QUINCENALES</h4>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
            </div>
            <div class="finance-box">
                <h4>INGRESOS MENSUALES</h4>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
                <div class="finance-item"><div class="line"></div></div>
            </div>
        </div>
        
        <div class="finance-table">
            <h4>MIS GASTOS FIJOS</h4>
            <div class="header">
                <div></div>
                <div>FECHA</div>
                <div>CANTIDAD</div>
            </div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
        </div>

        <div class="finance-table">
            <h4>MIS GASTOS VARIABLES</h4>
            <div class="header">
                <div></div>
                <div>FECHA</div>
                <div>CANTIDAD</div>
            </div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
            <div class="row"><div><input type="checkbox" /></div><div class="dotted-line"></div><div class="dotted-line"></div></div>
        </div>

        <div class="summary-boxes">
            <div class="summary-box"><p>GANANCIAS:</p></div>
            <div class="summary-box"><p>GASTOS:</p></div>
            <div class="summary-box"><p>AHORROS:</p></div>
        </div>
        
        <!-- Nueva Sección de Plan de Alimentación -->
        <hr>
        <div class="meal-plan-section">
            <h2>Plan de Alimentación Semanal</h2>
            <table class="meal-plan-table">
                <thead>
                    <tr>
                        <th>Día</th>
                        <th>Lunes</th>
                        <th>Martes</th>
                        <th>Miércoles</th>
                        <th>Jueves</th>
                        <th>Viernes</th>
                        <th>Sábado</th>
                        <th>Domingo</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Desayuno</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>Almuerzo</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>Cena</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>Snacks</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                </tbody>
            </table>
            
            <div class="shopping-list-container">
                <div class="shopping-list-box">
                    <h4>Verduras y Legumbres</h4>
                    <ul>
                        <li>Tomate</li>
                        <li>Pepinos</li>
                        <li>Lechuga</li>
                        <li>Col de Bruselas</li>
                        <li>Espárragos</li>
                        <li>Champiñones</li>
                        <li>Brócoli</li>
                        <li>Pimiento</li>
                        <li>Coliflor</li>
                        <li>Cebolla</li>
                        <li>Apio</li>
                        <li>Remolacha</li>
                        <li>Calabacín</li>
                        <li>Berenjena</li>
                        <li>Espinacas</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Cereales</h4>
                    <ul>
                        <li>Avena</li>
                        <li>Bulgur</li>
                        <li>Cebada</li>
                        <li>Pasta Integral</li>
                        <li>Maíz</li>
                        <li>Arroz Integral</li>
                        <li>Muesli sin azúcar</li>
                        <li>Tortitas de arroz</li>
                        <li>Trigo Sarraceno</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Grasas y Especias</h4>
                    <ul>
                        <li>Aceitunas</li>
                        <li>Anacardos</li>
                        <li>Nueces</li>
                        <li>Ajo</li>
                        <li>Linaza</li>
                        <li>Aguacate</li>
                        <li>Canela</li>
                        <li>Sal de mar</li>
                        <li>Hierbas y especias</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Proteínas</h4>
                    <ul>
                        <li>Pollo</li>
                        <li>Pavo</li>
                        <li>Carne magra</li>
                        <li>Conejo</li>
                        <li>Trucha</li>
                        <li>Salmón</li>
                        <li>Atún</li>
                        <li>Marisco</li>
                        <li>Dorada</li>
                        <li>Requesón</li>
                        <li>Yogur griego</li>
                        <li>Leche semidesnatada</li>
                        <li>Huevo/clara</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Proteínas Vegetales</h4>
                    <ul>
                        <li>Lentejas</li>
                        <li>Garbanzos</li>
                        <li>Soja</li>
                        <li>Tempeh</li>
                        <li>Seitán</li>
                        <li>Tofu</li>
                        <li>Guistsantes</li>
                        <li>Judías</li>
                        <li>Quinoa</li>
                        <li>Verduras verdes</li>
                        <li>Bebidas vegetales (sin azúcar)</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Frutas</h4>
                    <ul>
                        <li>Manzanas</li>
                        <li>Toronja</li>
                        <li>Naranjas</li>
                        <li>Plátanos</li>
                        <li>Pasas</li>
                        <li>Sandía/Melón</li>
                        <li>Cerezas</li>
                        <li>Uvas</li>
                        <li>Kiwi</li>
                        <li>Piña</li>
                        <li>Mango</li>
                        <li>Melocotón</li>
                        <li>Papaya</li>
                        <li>Frutas congeladas</li>
                        <li>Frutas del bosque</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <!-- Nueva sección de Plan de limpieza -->
        <hr>
        <div class="clean-plan-section">
            <h2>PLAN DE LIMPIEZA</h2>

            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>DIARIA</th>
                        <th>L</th><th>M</th><th>M</th><th>J</th><th>V</th><th>S</th><th>D</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="daily-tasks">
                        <td>Arreglar habitaciones</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Lavar platos</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Limpiar estufa</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Limpiar mesas</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Limpiar WC</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Aspirar</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Trapear</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>

            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>SEMANAL</th>
                        <th>S1</th><th>S2</th><th>S3</th><th>S4</th><th>S5</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="weekly-tasks">
                        <td>Quitar el polvo</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Tallar el piso</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar regaderas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Limpiar chapas y enchufes</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar ropa</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar sábanas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Regar plantas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar patio</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>
            
            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>QUINCENAL</th>
                        <th>Q1</th><th>Q2</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="biweekly-tasks">
                        <td>Ir al Supermercado</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Limpiar refrigerador</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Lavar el carro</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Lavar toallas</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Lavar cortinas del baño</td>
                        <td></td><td></td>
                    </tr>
                </tbody>
            </table>

            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>MENSUAL</th>
                        <th>E</th><th>F</th><th>M</th><th>A</th><th>M</th><th>J</th><th>J</th><th>A</th><th>S</th><th>O</th><th>N</th><th>D</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="monthly-tasks">
                        <td>Limpiar cocina</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="monthly-tasks">
                        <td>Limpiar clósets</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="monthly-tasks">
                        <td>Limpiar vidrios PA</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="monthly-tasks">
                        <td>Limpiar vidrios PB</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>
            
            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>EVENTUAL</th>
                        <th>E1</th><th>E2</th><th>E3</th><th>E4</th><th>E5</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="eventual-tasks">
                        <td>Lavar sillones</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Lavar sillas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Lavar cojines</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Lavar almohadas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Limpiar techo de madera</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>

            <div class="note-box">
                <h4>Notas adicionales:</h4>
                <p>...</p>
            </div>
        </div>
        
        <!-- Nueva sección de Gestión de Tiempo -->
        <hr>
        <div class="time-management-section">
            <h2>GESTIÓN DE TIEMPO</h2>
            <p class="subtitle">12 ACCIONES PARA LA GESTIÓN DEL TIEMPO</p>

            <div class="time-management-grid">
                <div class="card regla">
                    <h4>LA REGLA DE LOS 5 MINUTOS:</h4>
                    <p>Si te toma menos de 5 minutos, hazlo ahora. Sí, incluso si es levantarte para estirarte. ¡La procrastinación es para estirarse, no para las tareas!</p>
                </div>
                <div class="card sapo">
                    <h4>TRAGARSE EL SAPO PRIMERO</h4>
                    <p>Aborda la tarea más difícil primero en la mañana. Los sapos saben mejor cuando no estás pensando en ellos todo el día.</p>
                </div>
                <div class="card pomodoro">
                    <h4>TÉCNICA POMODORO</h4>
                    <p>Trabaja durante 25 minutos, luego toma un descanso de 5 minutos. Repite. Porque incluso los tomates necesitan un descanso.</p>
                </div>
                <div class="card lista">
                    <h4>HAZ UNA LISTA DE TAREAS</h4>
                    <p>Escribe tus tareas y tachalas como hechos. Se siente como una pequeña victoria cada vez.</p>
                </div>
                <div class="card delegar">
                    <h4>DELEGAR</h4>
                    <p>Comparte tareas con otros. Recuerda, el trabajo en equipo hace que el sueño funcione (y te da más tiempo para ver series).</p>
                </div>
                <div class="card apps">
                    <h4>USA APPS Y HERRAMIENTAS</h4>
                    <p>Utiliza aplicaciones de productividad. Deja que la tecnología sea el jefe que te diga que vuelvas al trabajo.</p>
                </div>
                <div class="card limites">
                    <h4>ESTABLECE LÍMITES</h4>
                    <p>Aprende a decir no. Protege tu tiempo como si fuera el último trozo de pizza.</p>
                </div>
                <div class="card calendario">
                    <h4>MANTÉN UN CALENDARIO</h4>
                    <p>Programa tus tareas y citas. Porque recordar todo es para elefantes y computadoras, no para humanos.</p>
                </div>
                <div class="card cuidado">
                    <h4>CUIDA DE TI MISMO</h4>
                    <p>Duerme lo suficiente, haz ejercicio y come bien. Un cerebro cansado es como una computadora con Windows 95. Lento y propenso a fallar.</p>
                </div>
                <div class="card redes">
                    <h4>LIMITA LAS REDES SOCIALES:</h4>
                    <p>Usa bloqueadores de redes sociales durante las horas de trabajo. Facebook y Instagram pueden esperar; tu trabajo de investigación no puede.</p>
                </div>
                <div class="card multitarea">
                    <h4>EVITA MULTITAREAS</h4>
                    <p>Concéntrate en una tarea a la vez. La multitarea es solo hacer múltiples cosas mal al mismo tiempo.</p>
                </div>
                <div class="card revision">
                    <h4>REFLEXIONA Y AJUSTA</h4>
                    <p>Revisa tu progreso regularmente y ajusta según sea necesario. Es como el GPS que te redirige después de un giro equivocado.</p>
                </div>
            </div>
        </div>

        
        <!-- Nueva sección de Notas -->
        <hr>
        <div class="notes-section">
            <h2>Notas Rápidas</h2>
            <div class="notes-box">
                <!-- Espacio para que el usuario escriba -->
            </div>
        </div>

        <!-- Nueva sección de Tablero de Metas -->
        <hr>
        <div class="goals-section">
            <h2>Tablero de Metas</h2>
            <p class="subtitle">Planea tus objetivos para lograr tus sueños.</p>
            <div class="goals-grid">
                <div>
                    <div class="goal-category">Profesional y laboral</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Económica o financiera</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Salud y bienestar</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Espiritual o personal</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Vacacional y diversión</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Académico o Educativo</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Social o familiar</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
            </div>
        </div>
        
        <!-- Sección de Registro de Hábitos -->
        <hr>
        <div class="habit-tracker-section">
            <h2>Registro de Hábitos</h2>
            <div class="habit-grid">
                <div class="habit-box">
                    <h4>Agua</h4>
                    <div class="habit-days">
                        <!-- Generar 31 casillas para los días del mes -->
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
                <div class="habit-box">
                    <h4>Ejercicio</h4>
                    <div class="habit-days">
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
                <div class="habit-box">
                    <h4>Lectura</h4>
                    <div class="habit-days">
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
                <div class="habit-box">
                    <h4>Sueño</h4>
                    <div class="habit-days">
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Sección de Contactos Importantes -->
        <hr>
        <div class="contacts-section">
            <h2>Contactos Importantes</h2>
            <div class="contact-item">
                <label for="nombre-contacto-1">Nombre:</label>
                <input type="text" id="nombre-contacto-1" />
            </div>
            <div class="contact-item">
                <label for="tel-contacto-1">Teléfono:</label>
                <input type="text" id="tel-contacto-1" />
            </div>
            <div class="contact-item">
                <label for="email-contacto-1">Email:</label>
                <input type="text" id="email-contacto-1" />
            </div>
            <div class="contact-item">
                <label for="nombre-contacto-2">Nombre:</label>
                <input type="text" id="nombre-contacto-2" />
            </div>
            <div class="contact-item">
                <label for="tel-contacto-2">Teléfono:</label>
                <input type="text" id="tel-contacto-2" />
            </div>
            <div class="contact-item">
                <label for="email-contacto-2">Email:</label>
                <input type="text" id="email-contacto-2" />
            </div>
            <div class="contact-item">
                <label for="nombre-contacto-3">Nombre:</label>
                <input type="text" id="nombre-contacto-3" />
            </div>
            <div class="contact-item">
                <label for="tel-contacto-3">Teléfono:</label>
                <input type="text" id="tel-contacto-3" />
            </div>
            <div class="contact-item">
                <label for="email-contacto-3">Email:</label>
                <input type="text" id="email-contacto-3" />
            </div>
        </div>

        <!-- Sección de Espacio Creativo -->
        <hr>
        <div class="notes-section">
            <h2>Espacio Creativo</h2>
            <div class="notes-box">
                <!-- Espacio para que el usuario dibuje o escriba -->
            </div>
        </div>
        
        <!-- Nueva Sección de Plan de Alimentación -->
        <hr>
        <div class="meal-plan-section">
            <h2>Plan de Alimentación Semanal</h2>
            <table class="meal-plan-table">
                <thead>
                    <tr>
                        <th>Día</th>
                        <th>Lunes</th>
                        <th>Martes</th>
                        <th>Miércoles</th>
                        <th>Jueves</th>
                        <th>Viernes</th>
                        <th>Sábado</th>
                        <th>Domingo</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Desayuno</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>Almuerzo</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>Cena</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>Snacks</td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                        <td></td>
                    </tr>
                </tbody>
            </table>
            
            <div class="shopping-list-container">
                <div class="shopping-list-box">
                    <h4>Verduras y Legumbres</h4>
                    <ul>
                        <li>Tomate</li>
                        <li>Pepinos</li>
                        <li>Lechuga</li>
                        <li>Col de Bruselas</li>
                        <li>Espárragos</li>
                        <li>Champiñones</li>
                        <li>Brócoli</li>
                        <li>Pimiento</li>
                        <li>Coliflor</li>
                        <li>Cebolla</li>
                        <li>Apio</li>
                        <li>Remolacha</li>
                        <li>Calabacín</li>
                        <li>Berenjena</li>
                        <li>Espinacas</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Cereales</h4>
                    <ul>
                        <li>Avena</li>
                        <li>Bulgur</li>
                        <li>Cebada</li>
                        <li>Pasta Integral</li>
                        <li>Maíz</li>
                        <li>Arroz Integral</li>
                        <li>Muesli sin azúcar</li>
                        <li>Tortitas de arroz</li>
                        <li>Trigo Sarraceno</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Grasas y Especias</h4>
                    <ul>
                        <li>Aceitunas</li>
                        <li>Anacardos</li>
                        <li>Nueces</li>
                        <li>Ajo</li>
                        <li>Linaza</li>
                        <li>Aguacate</li>
                        <li>Canela</li>
                        <li>Sal de mar</li>
                        <li>Hierbas y especias</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Proteínas</h4>
                    <ul>
                        <li>Pollo</li>
                        <li>Pavo</li>
                        <li>Carne magra</li>
                        <li>Conejo</li>
                        <li>Trucha</li>
                        <li>Salmón</li>
                        <li>Atún</li>
                        <li>Marisco</li>
                        <li>Dorada</li>
                        <li>Requesón</li>
                        <li>Yogur griego</li>
                        <li>Leche semidesnatada</li>
                        <li>Huevo/clara</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Proteínas Vegetales</h4>
                    <ul>
                        <li>Lentejas</li>
                        <li>Garbanzos</li>
                        <li>Soja</li>
                        <li>Tempeh</li>
                        <li>Seitán</li>
                        <li>Tofu</li>
                        <li>Guistsantes</li>
                        <li>Judías</li>
                        <li>Quinoa</li>
                        <li>Verduras verdes</li>
                        <li>Bebidas vegetales (sin azúcar)</li>
                    </ul>
                </div>
                <div class="shopping-list-box">
                    <h4>Frutas</h4>
                    <ul>
                        <li>Manzanas</li>
                        <li>Toronja</li>
                        <li>Naranjas</li>
                        <li>Plátanos</li>
                        <li>Pasas</li>
                        <li>Sandía/Melón</li>
                        <li>Cerezas</li>
                        <li>Uvas</li>
                        <li>Kiwi</li>
                        <li>Piña</li>
                        <li>Mango</li>
                        <li>Melocotón</li>
                        <li>Papaya</li>
                        <li>Frutas congeladas</li>
                        <li>Frutas del bosque</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <!-- Nueva sección de Plan de limpieza -->
        <hr>
        <div class="clean-plan-section">
            <h2>PLAN DE LIMPIEZA</h2>

            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>DIARIA</th>
                        <th>L</th><th>M</th><th>M</th><th>J</th><th>V</th><th>S</th><th>D</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="daily-tasks">
                        <td>Arreglar habitaciones</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Lavar platos</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Limpiar estufa</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Limpiar mesas</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Limpiar WC</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Aspirar</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="daily-tasks">
                        <td>Trapear</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>

            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>SEMANAL</th>
                        <th>S1</th><th>S2</th><th>S3</th><th>S4</th><th>S5</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="weekly-tasks">
                        <td>Quitar el polvo</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Tallar el piso</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar regaderas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Limpiar chapas y enchufes</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar ropa</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar sábanas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Regar plantas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="weekly-tasks">
                        <td>Lavar patio</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>
            
            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>QUINCENAL</th>
                        <th>Q1</th><th>Q2</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="biweekly-tasks">
                        <td>Ir al Supermercado</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Limpiar refrigerador</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Lavar el carro</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Lavar toallas</td>
                        <td></td><td></td>
                    </tr>
                    <tr class="biweekly-tasks">
                        <td>Lavar cortinas del baño</td>
                        <td></td><td></td>
                    </tr>
                </tbody>
            </table>

            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>MENSUAL</th>
                        <th>E</th><th>F</th><th>M</th><th>A</th><th>M</th><th>J</th><th>J</th><th>A</th><th>S</th><th>O</th><th>N</th><th>D</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="monthly-tasks">
                        <td>Limpiar cocina</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="monthly-tasks">
                        <td>Limpiar clósets</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="monthly-tasks">
                        <td>Limpiar vidrios PA</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="monthly-tasks">
                        <td>Limpiar vidrios PB</td>
                        <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>
            
            <table class="clean-plan-table">
                <thead>
                    <tr class="clean-header">
                        <th>EVENTUAL</th>
                        <th>E1</th><th>E2</th><th>E3</th><th>E4</th><th>E5</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="eventual-tasks">
                        <td>Lavar sillones</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Lavar sillas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Lavar cojines</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Lavar almohadas</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                    <tr class="eventual-tasks">
                        <td>Limpiar techo de madera</td>
                        <td></td><td></td><td></td><td></td><td></td>
                    </tr>
                </tbody>
            </table>

            <div class="note-box">
                <h4>Notas adicionales:</h4>
                <p>...</p>
            </div>
        </div>
        
        <!-- Nueva sección de Gestión de Tiempo -->
        <hr>
        <div class="time-management-section">
            <h2>GESTIÓN DE TIEMPO</h2>
            <p class="subtitle">12 ACCIONES PARA LA GESTIÓN DEL TIEMPO</p>

            <div class="time-management-grid">
                <div class="card regla">
                    <h4>LA REGLA DE LOS 5 MINUTOS:</h4>
                    <p>Si te toma menos de 5 minutos, hazlo ahora. Sí, incluso si es levantarte para estirarte. ¡La procrastinación es para estirarse, no para las tareas!</p>
                </div>
                <div class="card sapo">
                    <h4>TRAGARSE EL SAPO PRIMERO</h4>
                    <p>Aborda la tarea más difícil primero en la mañana. Los sapos saben mejor cuando no estás pensando en ellos todo el día.</p>
                </div>
                <div class="card pomodoro">
                    <h4>TÉCNICA POMODORO</h4>
                    <p>Trabaja durante 25 minutos, luego toma un descanso de 5 minutos. Repite. Porque incluso los tomates necesitan un descanso.</p>
                </div>
                <div class="card lista">
                    <h4>HAZ UNA LISTA DE TAREAS</h4>
                    <p>Escribe tus tareas y tachalas como hechos. Se siente como una pequeña victoria cada vez.</p>
                </div>
                <div class="card delegar">
                    <h4>DELEGAR</h4>
                    <p>Comparte tareas con otros. Recuerda, el trabajo en equipo hace que el sueño funcione (y te da más tiempo para ver series).</p>
                </div>
                <div class="card apps">
                    <h4>USA APPS Y HERRAMIENTAS</h4>
                    <p>Utiliza aplicaciones de productividad. Deja que la tecnología sea el jefe que te diga que vuelvas al trabajo.</p>
                </div>
                <div class="card limites">
                    <h4>ESTABLECE LÍMITES</h4>
                    <p>Aprende a decir no. Protege tu tiempo como si fuera el último trozo de pizza.</p>
                </div>
                <div class="card calendario">
                    <h4>MANTÉN UN CALENDARIO</h4>
                    <p>Programa tus tareas y citas. Porque recordar todo es para elefantes y computadoras, no para humanos.</p>
                </div>
                <div class="card cuidado">
                    <h4>CUIDA DE TI MISMO</h4>
                    <p>Duerme lo suficiente, haz ejercicio y come bien. Un cerebro cansado es como una computadora con Windows 95. Lento y propenso a fallar.</p>
                </div>
                <div class="card redes">
                    <h4>LIMITA LAS REDES SOCIALES:</h4>
                    <p>Usa bloqueadores de redes sociales durante las horas de trabajo. Facebook y Instagram pueden esperar; tu trabajo de investigación no puede.</p>
                </div>
                <div class="card multitarea">
                    <h4>EVITA MULTITAREAS</h4>
                    <p>Concéntrate en una tarea a la vez. La multitarea es solo hacer múltiples cosas mal al mismo tiempo.</p>
                </div>
                <div class="card revision">
                    <h4>REFLEXIONA Y AJUSTA</h4>
                    <p>Revisa tu progreso regularmente y ajusta según sea necesario. Es como el GPS que te redirige después de un giro equivocado.</p>
                </div>
            </div>
        </div>

        
        <!-- Nueva sección de Notas -->
        <hr>
        <div class="notes-section">
            <h2>Notas Rápidas</h2>
            <div class="notes-box">
                <!-- Espacio para que el usuario escriba -->
            </div>
        </div>

        <!-- Nueva sección de Tablero de Metas -->
        <hr>
        <div class="goals-section">
            <h2>Tablero de Metas</h2>
            <p class="subtitle">Planea tus objetivos para lograr tus sueños.</p>
            <div class="goals-grid">
                <div>
                    <div class="goal-category">Profesional y laboral</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Económica o financiera</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Salud y bienestar</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Espiritual o personal</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Vacacional y diversión</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Académico o Educativo</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
                <div>
                    <div class="goal-category">Social o familiar</div>
                    <div class="goal-item">1) <input type="text" /></div>
                    <div class="goal-item">2) <input type="text" /></div>
                    <div class="goal-item">3) <input type="text" /></div>
                </div>
                <div>
                    <div class="goal-category">Estrategia para lograrlo</div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                    <div class="strategy-item"><div class="line"></div><div class="meta-check"></div></div>
                </div>
            </div>
        </div>
        
        <!-- Sección de Registro de Hábitos -->
        <hr>
        <div class="habit-tracker-section">
            <h2>Registro de Hábitos</h2>
            <div class="habit-grid">
                <div class="habit-box">
                    <h4>Agua</h4>
                    <div class="habit-days">
                        <!-- Generar 31 casillas para los días del mes -->
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
                <div class="habit-box">
                    <h4>Ejercicio</h4>
                    <div class="habit-days">
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
                <div class="habit-box">
                    <h4>Lectura</h4>
                    <div class="habit-days">
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
                <div class="habit-box">
                    <h4>Sueño</h4>
                    <div class="habit-days">
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                        <div class="habit-day"></div><div class="habit-day"></div><div class="habit-day"></div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Sección de Contactos Importantes -->
        <hr>
        <div class="contacts-section">
            <h2>Contactos Importantes</h2>
            <div class="contact-item">
                <label for="nombre-contacto-1">Nombre:</label>
                <input type="text" id="nombre-contacto-1" />
            </div>
            <div class="contact-item">
                <label for="tel-contacto-1">Teléfono:</label>
                <input type="text" id="tel-contacto-1" />
            </div>
            <div class="contact-item">
                <label for="email-contacto-1">Email:</label>
                <input type="text" id="email-contacto-1" />
            </div>
            <div class="contact-item">
                <label for="nombre-contacto-2">Nombre:</label>
                <input type="text" id="nombre-contacto-2" />
            </div>
            <div class="contact-item">
                <label for="tel-contacto-2">Teléfono:</label>
                <input type="text" id="tel-contacto-2" />
            </div>
            <div class="contact-item">
                <label for="email-contacto-2">Email:</label>
                <input type="text" id="email-contacto-2" />
            </div>
            <div class="contact-item">
                <label for="nombre-contacto-3">Nombre:</label>
                <input type="text" id="nombre-contacto-3" />
            </div>
            <div class="contact-item">
                <label for="tel-contacto-3">Teléfono:</label>
                <input type="text" id="tel-contacto-3" />
            </div>
            <div class="contact-item">
                <label for="email-contacto-3">Email:</label>
                <input type="text" id="email-contacto-3" />
            </div>
        </div>

        <!-- Sección de Espacio Creativo -->
        <hr>
        <div class="notes-section">
            <h2>Espacio Creativo</h2>
            <div class="notes-box">
                <!-- Espacio para que el usuario dibuje o escriba -->
            </div>
        </div>

    </section>

    <button onclick="window.print()" class="print-button">Imprimir Agenda</button>
</div>

</body>
</html>
