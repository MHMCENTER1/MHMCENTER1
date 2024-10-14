<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MHM Center</title>
    <style>
        body { display: none; font-family: Arial, sans-serif; margin: 0; padding: 20px; background-color: #e3f2fd; color: #333; user-select: none; }
        .loader { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: #2196F3; display: flex; justify-content: center; align-items: center; font-size: 5em; color: white; opacity: 0; animation: fadeIn 1s forwards; }
        @keyframes fadeIn { 0% { opacity: 0; } 100% { opacity: 1; } }
    </style>
</head>
<body oncontextmenu="return false;">
    <div class="loader" id="loader">M</div>
    <script>
        const loader = document.getElementById('loader'), letters = ['M', 'H', 'M']; let index = 0;
        function changeLetter() { loader.textContent = letters[index]; index++; if (index >= letters.length) { clearInterval(interval); setTimeout(() => { loader.style.display = 'none'; document.body.style.display = 'block'; }, 500); } }
        const interval = setInterval(changeLetter, 1000); loader.style.opacity = '1';
    </script>
    
    <header>
        <h1>MHM Center</h1>
        <img src="https://drive.google.com/uc?id=1pHxyDhO8_Vw9s4EOWQbtg_vt0SHSkogj" alt="Photo de l'auteur" style="width: 150px; border-radius: 75px;">
        <p>Coordonnées : <strong>gbagoulemelchior@gmail.com</strong>, <strong>+229 55282826</strong></p>
    </header>
    
    <section class="products">
        <h2>Produits</h2>
        <div class="product">
            <h3>Produit 1</h3>
            <p>Musique création. <a href="https://whatsapp.com/channel/0029VajpP41GehEQcHhMCd2a">Voir le lien</a></p>
        </div>
        <div class="product">
            <h3>Produit 2</h3>
            <p>PREMIUM APK 💙🙃. <a href="https://t.me/PREMIUMApkFREE001">Voir le lien</a></p>
        </div>
    </section>

    <section>
        <h2>Mise à jour</h2>
        <p>Cette section permettra d'ajouter des options plus tard.</p>
        <button onclick="alert('Fonction de mise à jour à venir !')" class="contact-button">Mettre à jour</button>
    </section>

    <section>
        <h2>Contactez-nous</h2>
        <form action="mailto:gbagoulemelchior@gmail.com" method="post" enctype="text/plain">
            <label for="name">Nom :</label>
            <input type="text" id="name" name="name" required>
            <label for="email">E-mail :</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message :</label>
            <textarea id="message" name="message" rows="4" required></textarea>
            <input type="submit" value="Envoyer">
        </form>
    </section>

    <footer>
        <h2>Contact</h2>
        <a class="contact-button" href="https://wa.me/22955282826">Contacter via WhatsApp</a>
    </footer>
</body>
</html>
