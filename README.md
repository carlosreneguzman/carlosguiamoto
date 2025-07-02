<style>
        /* Estilos Generales */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }

        /* Encabezado */
        header {
            background-color: #2c3e50;
            color: #ecf0f1;
            padding: 30px 0;
            text-align: center;
            border-radius: 8px 8px 0 0;
            margin-bottom: 20px;
        }

        header h1 {
            font-family: 'Oswald', sans-serif;
            font-size: 3em;
            margin: 0;
            letter-spacing: 2px;
        }

        header p {
            font-size: 1.2em;
            margin-top: 10px;
        }

        /* Secciones de Motos */
        .moto-card {
            display: flex;
            flex-wrap: wrap; /* Permite que los elementos se envuelvan en pantallas pequeñas */
            align-items: center;
            background-color: #ffffff;
            border: 1px solid #ddd;
            border-radius: 8px;
            margin-bottom: 30px;
            padding: 20px;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease-in-out;
        }

        .moto-card:hover {
            transform: translateY(-5px);
        }

        .moto-card:nth-child(even) { /* Invertir orden en tarjetas pares */
            flex-direction: row-reverse;
        }

        .moto-image {
            flex: 1; /* Ocupa el espacio disponible */
            min-width: 300px; /* Ancho mínimo para la imagen */
            text-align: center;
            padding: 10px;
        }

        .moto-image img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .moto-info {
            flex: 2; /* Ocupa el doble de espacio */
            min-width: 320px; /* Ancho mínimo para la información */
            padding: 10px 20px;
        }

        .moto-info h2 {
            font-family: 'Oswald', sans-serif;
            color: #e74c3c;
            font-size: 2.2em;
            margin-top: 0;
            border-bottom: 2px solid #e74c3c;
            padding-bottom: 5px;
            margin-bottom: 15px;
        }

        .moto-info h3 {
            color: #2c3e50;
            font-size: 1.4em;
            margin-top: 20px;
            margin-bottom: 10px;
        }

        .moto-info ul {
            list-style-type: none;
            padding: 0;
        }

        .moto-info ul li {
            margin-bottom: 8px;
            padding-left: 20px;
            position: relative;
        }

        .moto-info ul li::before {
            content: '✓'; /* Un checkmark */
            color: #27ae60;
            font-weight: bold;
            position: absolute;
            left: 0;
        }

        /* Pie de página */
        footer {
            text-align: center;
            padding: 20px;
            margin-top: 30px;
            background-color: #34495e;
            color: #ecf0f1;
            border-radius: 0 0 8px 8px;
            font-size: 0.9em;
        }

        /* Media Queries para Responsive */
        @media (max-width: 768px) {
            .moto-card {
                flex-direction: column; /* Apilar en pantallas pequeñas */
            }
            .moto-card:nth-child(even) {
                flex-direction: column; /* También apilar para pares */
            }
            .moto-image, .moto-info {
                min-width: unset; /* Quitar ancho mínimo en pantallas pequeñas */
                width: 100%;
                padding: 10px 0;
            }
            header h1 {
                font-size: 2.5em;
            }
            .moto-info h2 {
                font-size: 1.8em;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>MotorCycle Zone</h1>
        <p>Tu destino para explorar las máquinas de dos ruedas más impresionantes del mundo.</p>
    </header>

    <div class="container">

        <div class="moto-card">
            <div class="moto-image">
                <img src="bmw_s1000rr.jpg" alt="BMW S1000RR">
            </div>
            <div class="moto-info">
                <h2>BMW S1000RR</h2>
                <p>La BMW S1000RR es la cúspide de la ingeniería alemana en el segmento de las superbikes. Nacida en la competición, esta máquina de cuatro cilindros en línea no solo impresiona por su diseño afilado y agresivo, sino por su rendimiento explosivo y su avanzada suite electrónica que la hace domable incluso para los pilotos más exigentes.</p>
                <h3>Características Clave:</h3>
                <ul>
                    <li>Motor de 999cc, 4 cilindros en línea, refrigeración líquida.</li>
                    <li>Potencia máxima: Más de 200 CV.</li>
                    <li>Electrónica de última generación: ABS Pro, Control Dinámico de Tracción (DTC), modos de conducción Pro.</li>
                    <li>Chasis Flex Frame para un manejo preciso.</li>
                    <li>Aerodinámica optimizada con alerones integrados (en modelos recientes).</li>
                </ul>
            </div>
        </div>

        <div class="moto-card">
            <div class="moto-image">
                <img src="kawasaki_zh2.jpg" alt="Kawasaki Z H2">
            </div>
            <div class="moto-info">
                <h2>Kawasaki Z H2</h2>
                <p>La Kawasaki Z H2 rompe moldes al combinar la potencia desbordante de un motor sobrealimentado con la agilidad y el estilo de una naked. Es una "hypernaked" que ofrece una experiencia de conducción visceral, con una aceleración asombrosa desde bajas revoluciones, envuelta en un diseño Sugomi que no deja a nadie indiferente.</p>
                <h3>Características Clave:</h3>
                <ul>
                    <li>Motor de 998cc, 4 cilindros en línea sobrealimentado.</li>
                    <li>Potencia impresionante y un par motor descomunal.</li>
                    <li>Suspensiones de alta calidad y frenos Brembo.</li>
                    <li>Control electrónico de crucero y modos de potencia.</li>
                    <li>Iluminación Full LED y pantalla TFT a color.</li>
                </ul>
            </div>
        </div>

        <div class="moto-card">
            <div class="moto-image">
                <img src="honda_cbr1000rr.jpg" alt="Honda CBR1000RR-R Fireblade">
            </div>
            <div class="moto-info">
                <h2>Honda CBR1000RR-R Fireblade</h2>
                <p>La Honda CBR1000RR-R Fireblade es la encarnación de la velocidad y la precisión de Honda, directamente derivada de la experiencia de la marca en MotoGP. Diseñada para la pista, ofrece un motor de altas revoluciones, una parte ciclo extremadamente ligera y rígida, y un paquete electrónico avanzado que permite extraer cada gota de rendimiento.</p>
                <h3>Características Clave:</h3>
                <ul>
                    <li>Motor de 999cc, 4 cilindros en línea, desarrollado para competición.</li>
                    <li>Potencia máxima líder en su clase.</li>
                    <li>Sistema de frenado Nissin/Brembo de alto rendimiento.</li>
                    <li>Control de par seleccionable (HSTC), control de wheelie, y ABS en curva.</li>
                    <li>Diseño aerodinámico con alerones inspirados en MotoGP.</li>
                </ul>
            </div>
        </div>

        <div class="moto-card">
            <div class="moto-image">
                <img src="yamaha_r1.jpg" alt="Yamaha YZF-R1">
            </div>
            <div class="moto-info">
                <h2>Yamaha YZF-R1</h2>
                <p>La Yamaha YZF-R1 es un icono en el mundo de las superbikes, reconocida por su distintivo motor "Crossplane" que ofrece una entrega de potencia única y un sonido inconfundible. Su enfoque en la ligereza, la agilidad y la tecnología la convierten en una opción formidable tanto para el circuito como para la carretera, ofreciendo una conexión excepcional entre el piloto y la máquina.</p>
                <h3>Características Clave:</h3>
                <ul>
                    <li>Motor Crossplane de 998cc, 4 cilindros en línea.</li>
                    <li>Sensación de tracción directa gracias al cigüeñal crossplane.</li>
                    <li>Sistema de medición inercial (IMU) de 6 ejes para una electrónica avanzada.</li>
                    <li>Control de lanzamiento, control de deslizamiento, y control de elevación.</li>
                    <li>Chasis Deltabox de aluminio para una rigidez y ligereza óptimas.</li>
                </ul>
            </div>
        </div>

        <div class="moto-card">
            <div class="moto-image">
                <img src="yamaha_mt07.jpg" alt="Yamaha MT-07">
            </div>
            <div class="moto-info">
                <h2>Yamaha MT-07</h2>
                <p>La Yamaha MT-07 es la naked de media cilindrada que ha conquistado corazones por su perfecta combinación de diversión, facilidad de uso y un motor bicilíndrico con un carácter inigualable. Ideal para la ciudad, las rutas y para aquellos que buscan una moto ágil y con un gran empuje desde bajas revoluciones, sin ser abrumadora.</p>
                <h3>Características Clave:</h3>
                <ul>
                    <li>Motor CP2 de 689cc, bicilíndrico en línea, con cigüeñal crossplane.</li>
                    <li>Gran par motor a bajas y medias revoluciones.</li>
                    <li>Chasis ligero y compacto que facilita la manejabilidad.</li>
                    <li>Posición de conducción cómoda y erguida.</li>
                    <li>Perfecta para la ciudad y para aprender.</li>
                </ul>
            </div>
        </div>

    </div>

    <footer>
        <p>&#169; 2023 MotorCycle Zone. Todos los derechos reservados. | Diseñado con pasión por las dos ruedas.</p>
    </footer>
</body>
</html>
