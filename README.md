# systeme_de_reservation
Comprendre le fonctionnement d'un systeme de reservetion
NB:  ne pas ce fier au faute d'orthograph j'ecrit avec un clavier *qwerty*

Dans un systeme de reservation il est question de reserver un service.

## Ex:
Reservation de:
- billet d'avion,
- Ticket de metro
- place ( ecole, restaurant, hotel, maquis ...)

## Comment ça fonctionne ?

Comme je viens de le dire, il s'agit de reserver un service:
 
 dans notre exemple un service est : **Un billet d'avion, Un Ticket de metro, Une place dans un restaurant...**
 
Ok on comprend, mais explique comment ca marche:

## Le fonctionnement

Derriere un systeme de reservation se cache un cache un algorithme un peu solide selon le service.

### Contraintes:

- Avoir le service dosponible pour la periode de reservation:
  
  Pour qu'un client arrive a reserver un service il faut que le service soit disponible dans la periode de reservation.
  
  Ex:
    M. Soro veut reserver un billet d'avion pour **Paris le 5 octobre avec la compagnie Corsair**.
    
    Containtes:
      - il faut que la compagnir corsaire ai un vol sur paris le 5 octoble
      - il faut qu'il ai au moin un billet disponible pour le 5 octobre au moment ou M. Soro arrive sur la plateforme de reservation.
      - il faut que M. Soro remplisse les condition de reservation
      - ...
      
      les contraintes dependent du service
      
      
### Gestion des reservations

  Il faut une plateforme de gestion du service de reservation.
  
  cette plateforme servira Au proprietaire du service de gerer les clients et les services.
  
  Ex:
    Combien de reservation sont en cours...
    Combien de reservation on ete confirme ou annule
    mise a jours de la disponibilite des service.

    Ex:
       Pour le systeme de reservation d'Imac a NaN
       - Savoir combien de mac son disponible pour la reservation
       - savoir combien de reservation ont ete effectue
       - Faire la mise a jours de Mac disponible si un mac est hors service
       
       ....
 
 ### Application
 
 Pour notre application nous allons suivre le model d'un systeme de reservation d'un restaurant.
 
D'abord il faut comprendre comment fonctionne le restaurent en question.

On prend un cas simple:

  Note restaurent offres 3 Services par jours.
    - Le **pti Dej**: Entre 6h et 10h Avec Un menu pour le peti dej
    - Le **Dej**: Entre 11h et 14h Avec Un menu
    - le **Diner**: Entre 18h et 22h Avec un menu
    
  Si un client veut effectuer une reservation dans notre restaurent il doit choisir entre (**pti Dej**, **Dej**, **Diner**)
  en suite il doit choisir le menu.
  

  - Contrainte
    - Il faut qu'il est une place dans le restaurant, au moment de la reservation,
    - Avoir un memnu disponible
  
  - gestion 
    - Le restaurent doit faire la mise a jour du nombre de pace disponible,
    - Connaitre le budget...
    

  
