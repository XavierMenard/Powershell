# Powershell
Home Made Powershell Scripts


Documentation Powershell-XM Fundamentals

# Documentation PowerShell : Commandes de Base

## 1. Navigation dans le système de fichiers
Lister le contenu d'un dossier :
```powershell
Get-ChildItem
```
Changer de répertoire :
```powershell
Set-Location Chemin/Du/Dossier
```
Revenir au dossier parent :
```powershell
Set-Location ..
```

## 2. Gestion des fichiers et dossiers
Créer un nouveau dossier :
```powershell
New-Item -ItemType Directory -Path "NomDuDossier"
```
Créer un fichier vide :
```powershell
New-Item -ItemType File -Path "NomDuFichier.txt"
```
Supprimer un fichier ou un dossier :
```powershell
Remove-Item -Path "NomDuFichierOuDossier"
```

## 3. Gestion des processus
Lister les processus en cours :
```powershell
Get-Process
```
Arrêter un processus :
```powershell
Stop-Process -Name "NomDuProcessus"
```

## 4. Gestion des services
Lister les services en cours d'exécution :
```powershell
Get-Service
```
Démarrer un service :
```powershell
Start-Service -Name "NomDuService"
```
Arrêter un service :
```powershell
Stop-Service -Name "NomDuService"
```

## 5. Gestion des utilisateurs
Créer un nouvel utilisateur local :
```powershell
New-LocalUser -Name "NomUtilisateur" -Password (ConvertTo-SecureString "MotDePasse" -AsPlainText -Force) -FullName "Nom Complet" -Description "Description de l'utilisateur"
```
Supprimer un utilisateur :
```powershell
Remove-LocalUser -Name "NomUtilisateur"
```

## 6. Exécution de scripts
Exécuter un script PowerShell :
```powershell
./NomDuScript.ps1
```
Changer la politique d'exécution pour autoriser les scripts :
```powershell
Set-ExecutionPolicy RemoteSigned
```

## 7. Réseau
Obtenir l'adresse IP de la machine :
```powershell
Get-NetIPAddress
```
Tester la connexion à une adresse IP :
```powershell
Test-Connection -ComputerName "AdresseIP" -Count 4
```

---

