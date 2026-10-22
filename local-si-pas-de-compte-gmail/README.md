# 🚀 Installer et lancer ton projet Python sur Windows

**Si tu n'as pas de compte Google, tu dois installer ton projet directement sur ton ordinateur.**

Nous allons utiliser **uv** pour installer Python et les bibliothèques nécessaires, puis **Jupyter Notebook** pour écrire et exécuter ton code.

### 1. Installer uv 📦

1. Ouvre **PowerShell** sur Windows (cherche « PowerShell » dans le menu Démarrer).
2. Copie-colle cette commande et appuie sur **Entrée** :

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

3. Attends que l'installation soit terminée.
4. Ferme PowerShell et ouvre-le à nouveau.

### 2. Ouvrir le dossier de ton projet 📂

1. Mets `project_base.ipynb` et `requirements.txt` dans le même dossier.
2. Ouvre ce dossier dans l'Explorateur de fichiers.
3. Clique dans la barre d'adresse, écris `powershell` et appuie sur **Entrée**.

PowerShell s'ouvre directement dans le bon dossier !

### 3. Lancer Jupyter Notebook ▶️

Dans PowerShell, copie-colle cette commande :

```powershell
uv run --python 3.11 --with-requirements requirements.txt --with notebook jupyter notebook
```

**Que fait cette commande ?**

- Installe Python 3.11 si nécessaire.
- Prépare les bibliothèques de ton projet.
- Lance Jupyter Notebook.

La première exécution peut prendre quelques minutes.

### 4. Ouvrir ton notebook 💻

1. Une page Jupyter devrait s'ouvrir automatiquement dans ton navigateur.
2. Clique sur `project_base.ipynb`.
3. Clique sur **▶️ Run** pour exécuter une cellule.
4. Modifie le code et expérimente !

### 5. Sauvegarder et arrêter 💾

- Pour sauvegarder ton travail, appuie sur **Ctrl + S** dans Jupyter.
- Pour arrêter Jupyter, retourne dans PowerShell et appuie sur **Ctrl + C**.
- Pour reprendre ton projet plus tard, relance simplement la commande de l'étape 3.

**🎉 Bravo ! Ton environnement Python est prêt. Amuse-toi avec ton projet d'IA !**