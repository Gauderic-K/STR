# STR \- fiche de cadrage

### **Contexte**

La Société de Tir de Reims est un club de tir sportif qui accueille des tireurs licenciés. Le club dispose de 16 postes de tir : 15 cibles loisir et 1 cible électronique. Il propose aussi une boutique (munitions, cibles) et la location d’armes à ses membres. Aujourd’hui, tout est géré sur papier et dans des tableaux Excel séparés, ce qui crée des erreurs et des pertes de temps. Le club a besoin d’un système unique pour gérer les réservations, le stock de la boutique et les locations d’armes.

### **Objectifs du projet**

Développer une application web permettant :

* Aux licenciés de créer un compte personnel et de se connecter.  
* De consulter les disponibilités des différents pas de tir.  
* De réserver un pas de tir pour un créneau défini (exemple : 1 heure).  
* De modifier ou d'annuler une réservation.  
* Au personnel du club de consulter et gérer les réservations.

### **Acteurs pressentis**

| Acteur | Rôle | Attente |
| ----- | ----- | ----- |
| **Comité directeur** | Commanditaire du projet, prend les décisions pour le club | Avoir une vue d’ensemble de l’activité (réservations, ventes, locations) et réduire les erreurs liées au papier |
| **Secrétaire** | Gère les membres, les réservations et le suivi administratif | Centraliser les informations au même endroit et ne plus recopier entre le cahier et Excel |
| **Animateurs / instructeurs** | Encadrent les tireurs sur le pas de tir, gèrent la sortie et le retour des armes louées | Voir le planning du jour et savoir à tout moment quelle arme est sortie et avec qui |
| **Adhérents loisir** | Réservent une cible, louent une arme, achètent en boutique | Voir les cibles libres et réserver facilement, sans passer par un appel |
| **Adhérents compétiteurs** | S’entraînent régulièrement, utilisent souvent la cible électronique | Pouvoir réserver à l’avance des créneaux réguliers pour préparer leurs compétitions |

### **Périmètre**

**Inclus dans le projet :**

* Création et gestion des comptes utilisateurs avec les informations utiles (nom, numéro de licence, date de fin de validité).  
* Distinction entre compétiteurs et tireurs loisir.  
* La réservation des 16 cibles : voir les créneaux libres, réserver, annuler, déplacer.  
* La gestion du stock de la boutique : entrées, ventes, alerte quand un produit passe sous un seuil.  
* La location d’armes sur place : à saisir en même temps que la réservation du pas de tir, suivre l’historique.

**Exclu du projet :**

* Le paiement en ligne et la comptabilité du club.  
* Réservation des armes à distance.  
* La gestion des adhésions annuelles et des licences fédérales (on lit seulement leur validité).  
* L’organisation des compétitions.  
* L’achat et l’entretien des armes du club.  
* Le site internet de présentation du club.

### **Un irritant concret**

Un adhérent loisir se met d’accord à l’oral avec un animateur pour avoir la cible électronique le lendemain à 14h pour la tester. Mais un compétiteur avait déjà réservé la cible au même créneau auprès de la secrétaire, qui l’avait notée dans son tableau Excel. L’animateur et la secrétaire n’ont aucun moyen de voir les réservations de l’autre. Le lendemain, les deux adhérents se présentent en même temps : cela crée des tensions entre eux et avec l’équipe du club, et l’un des deux doit se cantonner à tirer sur cible carton.

### **Contraintes**

* Application accessible depuis un navigateur web.  
* Compte utilisateur obligatoire pour réserver.  
* Un pas de tir ne peut pas être réservé deux fois sur le même créneau.  
* Les compétiteurs sont prioritaires pour la réservation de la cible électronique.  
* Les locations d'armes et les achats s'effectuent uniquement au club.  
* Protection des données personnelles conformément au RGPD.

### **Livrables attendus**

* Une application web de réservation.  
* Une base de données contenant les comptes et les réservations.  
* Une interface d'administration pour le personnel du club.  
* Une documentation utilisateur simplifiée.