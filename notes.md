1-COMMENTAIRES DOCKER

\## TP 1 - Lancer mon premier conteneur

J'ai exécuté docker run hello-world. Docker a téléchargé l'image depuis internet

puis a lancé le conteneur. Le conteneur a affiché un message de bienvenue puis

s'est arrêté tout seul. Avec docker ps -a j'ai vu le conteneur avec le statut

"Exited", ce qui montre qu'un conteneur peut s'arrêter automatiquement après

avoir fait sa tâche.



\## TP 2 - Lancer un serveur web et l'afficher

J'ai lancé nginx avec le port 8080 de ma machine relié au port 80 du conteneur.

En ouvrant http://localhost:8080 dans mon navigateur j'ai vu la page d'accueil

de nginx. Les logs montraient les requêtes reçues par le serveur. Au début j'avais

mis -name au lieu de --name ce qui a causé une erreur.



\## TP 3 - Entrer dans un conteneur

J'ai utilisé docker exec -it pour entrer dans le conteneur nginx. A l'intérieur

j'ai pu naviguer comme dans un vrai système Linux avec ls et cd. J'ai trouvé

les fichiers html de nginx dans /usr/share/nginx/html.



\## TP 4 - Créer ma propre image avec un Dockerfile

J'ai créé un fichier index.html et un Dockerfile avec deux lignes. La commande

docker build a construit mon image en téléchargeant nginx:alpine et en copiant

mon fichier dedans. En lançant le conteneur j'ai vu ma page personnalisée sur

http://localhost:8080.



\## TP 5 - Utiliser docker compose

J'ai créé un fichier docker-compose.yml décrivant un service nginx. La commande

docker compose up -d a lancé le conteneur automatiquement. docker compose down

a tout arrêté et supprimé proprement.



2-COMMENTAIRES GIT ET GITHUB

\## TP Git et GitHub

J'ai vérifié que Git était installé avec git --version, la version 2.54.0 s'est

affichée. J'ai configuré mon identité avec git config --global en donnant mon

nom et mon email.



J'ai créé un dépôt nommé onboarding-dgs sur github.com puis je l'ai cloné sur

ma machine avec git clone. J'ai essayé cd onboarding.dgs avec un point au lieu

d'un tiret ce qui n'a pas marché, la bonne commande était cd onboarding-dgs.



J'ai créé le fichier notes.md avec mes commentaires des TP Docker, ajouté mes

captures d'écran dans le dossier, puis j'ai tout envoyé sur GitHub avec

git add . , git commit et git push. 29 fichiers ont été envoyés dont les 28

captures et le notes.md. Le push a bien fonctionné et tout est visible sur

mon dépôt GitHub.



Lien du dépôt : https://github.com/ousmane-diouf/onboarding-dgs







