import UIKit

/*mettre propriété imad krifa*/

class MainRpg {
    
    var player1 : String?
    var player2 : String?
    var personnage1 : String?
    var personnage2 : String?
    var personnage3 : String?
    var personnage4 : String?
    var personnage5 : String?
    var personnage6 : String?
    
 
    
    
    
    
    init (player1 : String, player2 : String,personnage1 : String, personnage2 : String, personnage3 : String, personnage4 : String, personnage5 : String, personnage6 : String) {
    
    self.player1=player1
    self.player2=player2
    self.personnage1=personnage1
    self.personnage2=personnage2
    self.personnage3=personnage3
    self.personnage4=personnage4
    self.personnage5=personnage5
    self.personnage6=personnage6
    }
    
    func launchGame() {
        /*Appel fonctions pour lancer le jeu dans la class MainRpg*/
        consignes()
        createTeams()
        choiceNamePersonnage()
        noSimilaryNamePersonnage()
        startBattle()
        displayWinner()
        
    }
    
        
    func consignes() {
        Swift.print("Menu du jeu RPG : SUIKODEN 99\n")
        Swift.print(" ce jeu se présente sous la forme d'un jeu de rôle de deux équipes de 3 personnages.\n")
        Swift.print("4 type de personnages sont à votre disposition, voici les choix possible :"
              + "\n1. L'Orc à une attaque forte (120 att), une défense moyenne (100 DEF) et un hp faible (75 HP)"
              + "\n2. L'Elf à une attaque moyenne (90 att), une défense moyenne (80 DEF) et des points de vie forte (120 HP)"
              + "\n3. Le Sorcier à une attaque faible (75 att), une défense faible (75 DEF) et un hp moyen (90 HP)"
              + "\n4. Le Chevalier à une attaque forte (120 att), une défense moyenne (100 DEF) et un hp moyen (100 HP)")
    }
              
    func createTeams(){
        /* optionnel si rien de rempli remplacer par vide */
        player1 = String(readLine() ?? " ")
        player2 = String(readLine() ?? " ")
            
    }
        /*faire attention qu'il y ai aucun personnage qui porte le nom d'un autre personnage : enumerer ou fonction utiliser if et || */
        
      
    // pas de doublon dans le nommage des joueurs
    // a peaufiner car rien ne bloque
    func noSimilaryNamePersonnage()() {
          if player1== player2{
            print("Nom de joueur déja utilisé, merci de choisir un autre nom de joueur")
        } else
            print("Nommage est OK")
    
    }
    
    
    
            
            
            
        
       
        
        
        
        
        
    func choiceNamePersonnage(){
        //choisir 3 personnages de son equipe
        .print("Merci de nommer le premier personnage de votre equipe")
        personnage1 = String(readLine() ?? " " )
        Swift.print("Merci de nommer le deuxième personnage de votre equipe")
        personnage2 = String(readLine() ?? " " )
        Swift.print("Merci de nommer le troisième personnage de votre equipe")
        personnage3 = String(readLine() ?? " " )
        
        //Nommez 3 personnage de l'équipe adverse
        
        Swift.print("Merci de nommer le premier personnage de l'équipe adverse")
        personnage4 = String(readLine() ?? " " )
        Swift.print("Merci de nommer le deuxième personnage de l'équipe adverse")
        personnage5 = String(readLine() ?? " " )
        Swift.print("Merci de nommer le troisième personnage de l'équipe adverse")
        personnage6 = String(readLine() ?? " " )
    }
        
        //afficher synthese des personnage choisi par chaque joueur
                  
    
        
            
            
            
       /* BONUS : si un personnage a moins de 20% de points de vie, son attaque augmente de 30% */
            
            
        }
        
        
    }
    
    
    func startBattle() {
        
        
        
        
        
          
        
        /* choisir action attaque - defense - items */
        
        
        
        
        
        
        
        /* choisir personnage adverse qui prend le coup*/
        
        
        
        
        
        
        
        /* utiliser func displayWinner si hp<1 donc true donc la partie est perdue ou non SINON c'est le tour du joueur adverse */
        
        
        if diplayWinner==true
        
        
    }
   
    
    func displayWinner() -> Bool{
        if player1
        
        /* afficher le gagnant des qu'un joueur n'a plus de vie pour tous ses personnages*/
        
        
        /* afficher les staitisques du jeu : le nombre de tours, liste des personnages des 2 equipes avec leurs propriétés (point de vie, force, arme utilisé) des 2 EQUIPES*/
        
    }




    


}

class player : MainRpg{
    
    
    //tableau des valeurs des type de personnage
    var character = [Character]()

}







class Character : player {
    
    /* il faut penser le nom du personnage, aux points de vie et son arme */
    /* choisir 4 types de personnage knight Orc Elf Sorcerer  donc var en tableau*/
    var attack : Int
    var def : Int
    var hp : Int
    var weapon = [Weapon]()
    
    init(hp : Int){
        self.def=def
        self.hp=hp
        self.attack=attack
        super.init(String : player.personnage1)
    }
    
    
    func typePersonnage(){
        
        
        
        
        
    }
    
    
    
   
}



class Weapon : Character {
    
    /* mettre en valeur des armes : leur puissance de preference pour tel type de personnage */
    /* il y a 4 types de personnages donc 4 type d'armes et 4 niveau de puissance selon le personnage en face*/
    /* utiliser enum et case pour y parvenir*/
    /* faudra penser que l'attaque sera réduit de 50%  en cas de défense de l'eauipe adverse*/
    
    
}

let rpg = MainRpg()
rpg.launchgame()
