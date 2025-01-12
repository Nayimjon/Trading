<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shaxsiy Profil</title>
    <style>
        /* Stil qismi */
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f8ff;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #007BFF;
            color: white;
            padding: 20px;
        }
        main {
            margin-top: 20px;
            padding: 10px;
        }
        img {
            width: 150px;
            border-radius: 50%;
        }
        section {
            margin: 20px auto;
            padding: 10px;
            max-width: 600px;
            text-align: left;
        }
        button {
            background-color: #007BFF;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .contact-form button {
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Shaxsiy Profil</h1>
    </header>
    <main>
        <!-- Profil rasmi va qisqacha ma'lumot -->
        <img src="profil.jpg" alt="Profil rasmi">
        <h2>Ism: Nayimjon</h2>
        <p>Men dasturchi bo‘lishni xohlayman va saytlar yaratishga qiziqaman!</p>
        <button onclick="aloqaQil()">Menga yozing!</button>

        <!-- Qiziqishlar -->
        <section>
            <h3>Qiziqishlar</h3>
            <ul>
                <li>Dasturlash</li>
                <li>Sport</li>
                <li>Kitob o'qish</li>
                <li>Sayohat qilish</li>
            </ul>
        </section>

        <!-- Aloqa shakli -->
        <section class="contact-form">
            <h3>Aloqa shakli</h3>
            <p>Menga xabar yuboring:</p>
            <form onsubmit="xabarYuborish(event)">
                <input type="text" placeholder="Ismingiz" required>
                <input type="email" placeholder="Email" required>
                <textarea placeholder="Xabaringizni yozing..." rows="4" required></textarea>
                <button type="submit">Yuborish</button>
            </form>
        </section>
    </main>

    <script>
        // Aloqa tugmasi uchun
        function aloqaQil() {
            alert("Rahmat! Tez orada sizga javob beraman!");
        }

        // Shakl yuborilishi uchun
        function xabarYuborish(event) {
            event.preventDefault(); // Formani qayta yuklashini to'xtatadi
            alert("Xabaringiz yuborildi! Rahmat!");
        }
    </script>
</body>
</html>
