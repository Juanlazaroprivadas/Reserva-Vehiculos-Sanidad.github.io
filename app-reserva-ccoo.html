<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reserva de Vehículos - Sanidad CCOO</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #d32f2f;
            --primary-dark: #b71c1c;
            --secondary: #37474f;
            --bg: #f5f5f5;
            --surface: #ffffff;
            --text: #212121;
            --text-light: #757575;
            --border: #e0e0e0;
            --radius: 8px;
            --shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Open Sans', sans-serif; }
        body { background-color: var(--bg); color: var(--text); padding: 16px; }
        header { max-width: 800px; margin: 0 auto 24px auto; text-align: center; border-bottom: 3px solid var(--primary); padding-bottom: 12px; }
        header h1 { color: var(--primary); font-size: 24px; font-weight: 700; }
        header p { color: var(--text-light); font-size: 14px; margin-top: 4px; }
        .container { max-width: 800px; margin: 0 auto; display: flex; flex-direction: column; gap: 20px; }
        .card { background: var(--surface); padding: 20px; border-radius: var(--radius); box-shadow: var(--shadow); border: 1px solid var(--border); }
        h2 { font-size: 18px; color: var(--secondary); margin-bottom: 16px; display: flex; align-items: center; gap: 8px; }
        .grid-vehicles { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
        @media(max-width: 600px) { .grid-vehicles { grid-template-columns: 1fr; } }
        .vehicle-option { border: 2px solid var(--border); padding: 16px; border-radius: var(--radius); cursor: pointer; transition: all 0.2s; position: relative; }
        .vehicle-option:hover { border-color: var(--text-light); }
        .vehicle-option.selected { border-color: var(--primary); background-color: #ffebee; }
        .vehicle-title { font-weight: 700; font-size: 16px; margin-bottom: 4px; }
        .vehicle-desc { font-size: 13px; color: var(--text-light); }
        .form-group { margin-bottom: 16px; }
        label { display: block; font-size: 14px; font-weight: 600; margin-bottom: 6px; color: var(--secondary); }
        input, select { width: 100%; padding: 10px; border: 1px solid var(--border); border-radius: var(--radius); font-size: 14px; outline: none; }
        input:focus, select:focus { border-color: var(--primary); }
        .grid-inputs { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
        @media(max-width: 500px) { .grid-inputs { grid-template-columns: 1fr; } }
        btn, button { display: block; width: 100%; background: var(--primary); color: white; border: none; padding: 12px; font-size: 16px; font-weight: 600; border-radius: var(--radius); cursor: pointer; text-align: center; transition: background 0.2s; }
        btn:hover, button:hover { background: var(--primary-dark); }
        .reserva-item { display: flex; justify-content: space-between; align-items: center; padding: 12px; border-bottom: 1px solid var(--border); font-size: 14px; }
        .reserva-item:last-child { border-bottom: none; }
        .reserva-info span { display: block; }
        .reserva-vehiculo { font-weight: 700; color: var(--primary); }
        .reserva-meta { font-size: 12px; color: var(--text-light); }
        .btn-delete { background: none; color: #d32f2f; border: none; padding: 4px 8px; font-size: 13px; cursor: pointer; width: auto; display: inline; }
        .btn-delete:hover { text-decoration: underline; background: none; }
        .empty-state { text-align: center; color: var(--text-light); font-size: 14px; padding: 20px; }
    </style>
</head>
<body>

    <header>
        <h1>Sanidad CCOO - Control de Vehículos</h1>
        <p>Sistema de Gestión Móvil y de Escritorio</p>
    </header>

    <div class="container">
        <!-- Formulario de Reserva -->
        <div class="card">
            <h2>Nueva Reserva</h2>
            <form id="reservationForm">
                <div class="form-group">
                    <label>1. Selecciona el Vehículo</label>
                    <div class="grid-vehicles">
                        <div class="vehicle-option" id="v1" onclick="selectVehicle('Dacia Sandero')">
                            <div class="vehicle-title">Dacia Sandero</div>
                            <div class="vehicle-desc">5 plazas • Compacto urbano • Ideal distancias cortas</div>
                        </div>
                        <div class="vehicle-option" id="v2" onclick="selectVehicle('Seat Alhambra')">
                            <div class="vehicle-title">Seat Alhambra</div>
                            <div class="vehicle-desc">7 plazas • Monovolumen grande • Ideal rutas largas / material</div>
                        </div>
                    </div>
                </div>

                <div class="form-group">
                    <label for="user">2. Nombre del Solicitante</label>
                    <input type="text" id="user" placeholder="Ej. María García (Delegada)" required>
                </div>

                <div class="grid-inputs">
                    <div class="form-group">
                        <label for="date">3. Fecha del Uso</label>
                        <input type="date" id="date" required>
                    </div>
                    <div class="form-group">
                        <label for="timeSlot">4. Horario</label>
                        <select id="timeSlot" required>
                            <option value="Mañana (08:00 - 14:00)">Mañana (08:00 - 14:00)</option>
                            <option value="Tarde (14:00 - 20:00)">Tarde (14:00 - 20:00)</option>
                            <option value="Día Completo">Día Completo</option>
                        </select>
                    </div>
                </div>

                <button type="submit" style="margin-top: 10px;">Confirmar Reserva</button>
            </form>
        </div>

        <!-- Agenda de Reservas -->
        <div class="card">
            <h2>Reservas Confirmadas</h2>
            <div id="reservationsList">
                <div class="empty-state">No hay reservas programadas.</div>
            </div>
        </div>
    </div>

    <script>
        let selectedVehicleType = '';
        let reservations = JSON.parse(localStorage.getItem('ccoo_vehiculos')) || [];

        function selectVehicle(vehicle) {
            selectedVehicleType = vehicle;
            document.getElementById('v1').classList.remove('selected');
            document.getElementById('v2').classList.remove('selected');
            if(vehicle === 'Dacia Sandero') {
                document.getElementById('v1').classList.add('selected');
            } else {
                document.getElementById('v2').classList.add('selected');
            }
        }

        function renderReservations() {
            const container = document.getElementById('reservationsList');
            if (reservations.length === 0) {
                container.innerHTML = '<div class="empty-state">No hay reservas programadas.</div>';
                return;
            }
            // Ordenar por fecha
            reservations.sort((a,b) => new Date(a.date) - new Date(b.date));
            
            container.innerHTML = reservations.map((res, index) => `
                <div class="reserva-item">
                    <div class="reserva-info">
                        <span class="reserva-vehiculo">${res.vehicle}</span>
                        <span>Por: ${res.user}</span>
                        <span class="reserva-meta">Fecha: ${formatDate(res.date)} | Horario: ${res.timeSlot}</span>
                    </div>
                    <button class="btn-delete" onclick="deleteReservation(${index})">Cancelar</button>
                </div>
            `).join('');
        }

        function formatDate(dateStr) {
            const parts = dateStr.split('-');
            return `${parts[2]}/${parts[1]}/${parts[0]}`;
        }

        function deleteReservation(index) {
            if(confirm('¿Seguro que deseas cancelar esta reserva?')) {
                reservations.splice(index, 1);
                localStorage.setItem('ccoo_vehiculos', JSON.stringify(reservations));
                renderReservations();
            }
        }

        document.getElementById('reservationForm').addEventListener('submit', function(e) {
            e.preventDefault();
            if(!selectedVehicleType) {
                alert('Por favor, selecciona un vehículo (Dacia Sandero o Seat Alhambra).');
                return;
            }

            const user = document.getElementById('user').value;
            const date = document.getElementById('date').value;
            const timeSlot = document.getElementById('timeSlot').value;

            // Validación de conflicto simple
            const conflicto = reservations.some(res => res.vehicle === selectedVehicleType && res.date === date && (res.timeSlot === timeSlot || res.timeSlot === 'Día Completo' || timeSlot === 'Día Completo'));
            
            if(conflicto) {
                alert('Error: Este vehículo ya está reservado para esa fecha y horario.');
                return;
            }

            reservations.push({ vehicle: selectedVehicleType, user, date, timeSlot });
            localStorage.setItem('ccoo_vehiculos', JSON.stringify(reservations));
            
            // Resetear
            document.getElementById('reservationForm').reset();
            selectedVehicleType = '';
            document.getElementById('v1').classList.remove('selected');
            document.getElementById('v2').classList.remove('selected');
            
            renderReservations();
            alert('¡Reserva confirmada con éxito!');
        });

        // Carga inicial
        renderReservations();
    </script>
</body>
</html>
