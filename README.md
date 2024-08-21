
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PENDO & FAMILLE SURL</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #4CAF50;
        }
        .container {
            padding: 20px;
            max-width: 1000px;
            margin: auto;
        }
        .section {
            margin-bottom: 20px;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        form label {
            margin-top: 10px;
        }
        form input, form textarea {
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        form textarea {
            resize: vertical;
            height: 100px;
        }
        form button {
            margin-top: 15px;
            padding: 10px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        form button:hover {
            background-color: #45a049;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

    <header>
        <h1>PENDO & FAMILLE SURL</h1>
        <p>Votre partenaire de confiance pour les huiles végétales, briquettes combustibles, matériaux de construction innovants et équipements d'énergies alternatives.</p>
    </header>

    <nav>
        <a href="#accueil">Accueil</a>
        <a href="#produits">Nos produits</a>
        <a href="#contact">Contacts</a>
    </nav>

    <div class="container">
        <section id="accueil" class="section">
            <h2>Bienvenue chez PENDO & FAMILLE SURL</h2>
            <p>Nous sommes dédiés à fournir des solutions de qualité supérieure pour répondre à vos besoins quotidiens, qu'il s'agisse de produits alimentaires, de combustibles, de matériaux de construction innovants, ou d'équipements pour les énergies alternatives.</p>
        </section>

        <section id="produits" class="section">
            <h2>Nos produits</h2>
            <ul>
                <li><strong>Huiles végétales vierges :</strong> Huiles de sésame, arachide, moringa, coco et ricin, pour usage culinaire, cosmétique et médicinal.</li>
                <li><strong>Briquettes combustibles :</strong> Briquettes écologiques, fabriquées pour une combustion efficace et durable.</li>
                <li><strong>Matériaux de construction innovants :</strong> Briques de Typha, panneaux isolants en Typha, béton de Typha, composites en Typha, plâtre à base de Typha, appréciés pour leur capacité à capter du CO2 et leurs performances en termes d'isolation.</li>
                <li><strong>Equipements d'énergies alternatives :</strong> Presses à briquettes, presses à briques de Typha, séchoirs solaires et plus encore.</li>
            </ul>
        </section>

        <section id="faq" class="section">
            <h2>Nos services</h2>
            <ul>
                <li><strong>Conseils et assistance :</strong> Nous offrons des conseils et une assistance technique pour les systèmes solaires photovoltaïques, les chauffes-eau solaires et les biodigesteurs.</li>
            </ul>
        </section>

        <section id="contact" class="section">
            <h2>Contacts</h2>
            <p><strong>Téléphone :</strong> +257 79 08 40 08</p>
            <p><strong>Email :</strong> <a href="mailto:mudherwmb@gmail.com">mudherwmb@gmail.com</a></p>
            <p><strong>Adresse :</strong> 6ème Avenue, Quartier Carama, Zone Kinama, Commune Ntahangwa, Bujumbura, Burundi</p>

            <h3>Laissez-nous un message</h3>
            <form action="mailto:mudherwmb@gmail.com" method="post" enctype="text/plain">
                <label for="name">Nom :</label>
                <input type="text" id="name" name="nom" required>

                <label for="email">Email :</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message :</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit">Envoyer</button>
            </form>
        </section>
    </div>

    <footer>
        <?php
            $file = 'compteur.txt';

            // Lire le nombre actuel de visites
            $visits = (int)file_get_contents($file);

            // Incrémenter le compteur
            $visits++;

            // Enregistrer le nouveau nombre de visites
            file_put_contents($file, $visits);

            // Afficher le nombre de visites
            echo "Nombre de visites : " . $visits;
        ?>
    </footer>

</body>
</html>
