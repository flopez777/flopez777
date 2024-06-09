<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VitalPets - Agendamiento de Citas</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Bienvenido a VitalPets</h1>
        <p>Agendamiento de Citas</p>
    </header>
    <main>
        <section id="appointment-form">
            <h2>Agendar una Cita</h2>
            <form id="appointmentForm">
                <label for="name">Nombre de la Mascota:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="owner">Nombre del Dueño:</label>
                <input type="text" id="owner" name="owner" required>
                
                <label for="date">Fecha:</label>
                <input type="date" id="date" name="date" required>
                
                <label for="time">Hora:</label>
                <input type="time" id="time" name="time" required>
                
                <button type="submit">Agendar Cita</button>
            </form>
        </section>
    </main>

    <script>
        // Espera a que el DOM esté completamente cargado
        document.addEventListener('DOMContentLoaded', function() {
            // Selecciona el formulario
            const form = document.getElementById('appointmentForm');

            // Agrega un evento de escucha al envío del formulario
            form.addEventListener('submit', function(event) {
                // Previene el comportamiento por defecto del formulario (recargar la página)
                event.preventDefault();

                // Redirige a la página de confirmación
                window.location.href = 'confirmation.html';
            });
        });
    </script>
</body>
</html>
