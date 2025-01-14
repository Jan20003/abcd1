# abcd1
my_website-index.html
<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moja Rozbudowana Strona</title>
    <style>
        /* Resetowanie domyślnych stylów */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f4f9;
            color: #333;
        }

        /* Nagłówek */
        header {
            background-color: #333;
            color: white;
            padding: 1rem;
            text-align: center;
        }

        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            margin-top: 1rem;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        /* Sekcja powitalna */
        .welcome-section {
            background-color: #007bff;
            color: white;
            padding: 4rem 2rem;
            text-align: center;
        }

        .welcome-section h1 {
            font-size: 2.5rem;
        }

        /* Sekcja O mnie */
        .about-section {
            padding: 3rem 2rem;
            background-color: #fff;
            margin-top: 2rem;
        }

        .about-section h2 {
            text-align: center;
            margin-bottom: 1rem;
        }

        .about-section p {
            text-align: center;
            font-size: 1.1rem;
        }

        /* Galeria */
        .gallery-section {
            padding: 3rem 2rem;
            background-color: #e9ecef;
        }

        .gallery-section h2 {
            text-align: center;
            margin-bottom: 1rem;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 8px;
            transition: transform 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.05);
        }

        /* Formularz kontaktowy */
        .contact-section {
            padding: 3rem 2rem;
            background-color: #fff;
            margin-top: 2rem;
        }

        .contact-section h2 {
            text-align: center;
            margin-bottom: 1rem;
        }

        .contact-section form {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .contact-section input,
        .contact-section textarea {
            width: 100%;
            max-width: 500px;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .contact-section button {
            background-color: #007bff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .contact-section button:hover {
            background-color: #0056b3;
        }

        /* Stopka */
        footer {
            background-color: #333;
            color: white;
            padding: 1rem;
            text-align: center;
            margin-top: 2rem;
        }
    </style>
</head>
<body>

    <!-- Nagłówek z nawigacją -->
    <header>
        <h1>Moja Rozbudowana Strona</h1>
        <nav>
            <ul>
                <li><a href="#welcome">Powitanie</a></li>
                <li><a href="#about">O mnie</a></li>
                <li><a href="#gallery">Galeria</a></li>
                <li><a href="#contact">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <!-- Sekcja powitalna -->
    <section class="welcome-section" id="welcome">
        <h1>Witaj na mojej stronie!</h1>
        <p>To jest przykładowa, rozbudowana strona, którą stworzyłem za pomocą HTML, CSS i JavaScript.</p>
    </section>

    <!-- Sekcja O mnie -->
    <section class="about-section" id="about">
        <h2>O mnie</h2>
        <p>Cześć! Jestem pasjonatem web designu i programowania. Uwielbiam tworzyć strony internetowe i aplikacje webowe, które są zarówno funkcjonalne, jak i estetyczne. Moim celem jest ciągłe doskonalenie moich umiejętności i nauka nowych technologii!</p>
    </section>

    <!-- Galeria -->
    <section class="gallery-section" id="gallery">
        <h2>Galeria</h2>
        <div class="gallery">
            <img src="https://via.placeholder.com/400" alt="Zdjęcie 1">
            <img src="https://via.placeholder.com/400" alt="Zdjęcie 2">
            <img src="https://via.placeholder.com/400" alt="Zdjęcie 3">
            <img src="https://via.placeholder.com/400" alt="Zdjęcie 4">
            <img src="https://via.placeholder.com/400" alt="Zdjęcie 5">
            <img src="https://via.placeholder.com/400" alt="Zdjęcie 6">
        </div>
    </section>

    <!-- Formularz kontaktowy -->
    <section class="contact-section" id="contact">
        <h2>Skontaktuj się ze mną</h2>
        <form onsubmit="return handleFormSubmit(event)">
            <input type="text" id="name" placeholder="Imię i nazwisko" required>
            <input type="email" id="email" placeholder="Twój email" required>
            <textarea id="message" placeholder="Twoja wiadomość" rows="4" required></textarea>
            <button type="submit">Wyślij</button>
        </form>
    </section>

    <!-- Stopka -->
    <footer>
        <p>© 2025 Moja Rozbudowana Strona | Wszystkie prawa zastrzeżone.</p>
    </footer>

    <script>
        // Obsługa formularza kontaktowego
        function handleFormSubmit(event) {
            event.preventDefault();
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const message = document.getElementById('message').value;
            
            alert(`Dziękujemy za kontakt, ${name}! Twoja wiadomość została wysłana.`);
            
            // Można dodać wysyłanie danych do serwera lub zapis do bazy danych
        }
    </script>

</body>
</html>
