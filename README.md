# Site-aux-ench-res-
Enchérir.com
#!/bin/bash

# Script pour déployer le site d'enchères sur GitHub + instructions Vercel

# 1️⃣ Initialiser git et commit
git init
git add .
git commit -m "Premier commit du site d'enchères"

# 2️⃣ Ajouter remote GitHub (remplace par ton URL)
GITHUB_URL="https://github.com/tonpseudo/site-encheres.git"
git remote add origin $GITHUB_URL

# 3️⃣ Push sur GitHub
git branch -M main
git push -u origin main

# 4️⃣ Instructions Vercel
echo "\n---"
echo "Projet envoyé sur GitHub !"
echo "\nPour déployer sur Vercel :"
echo "1. Crée un compte sur https://vercel.com/ et connecte ton GitHub."
echo "2. Clique sur 'New Project' → 'Import Git Repository' → sélectionne 'site-encheres'."
echo "3. Ajoute les variables d'environnement :"
echo "   NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY = <ta_clé_publique>"
echo "   STRIPE_SECRET_KEY = <ta_clé_secrète>"
echo "4. Clique sur 'Deploy'."
echo "5. Vercel va te donner l'URL du site en ligne."
