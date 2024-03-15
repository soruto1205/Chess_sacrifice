import pygame
import os

# Taille
Largeur, Hauteur = 760, 760
Lignes, Colonnes = 8, 8
Carre = Largeur // Lignes

# Couleurs
Fond = (47, 79, 79)
Noir = (0, 0, 0)
Blanc = (255, 255, 255)
Beige = (245, 245, 220)
Marron_Chocolat = (210, 105, 30)
Marron = (87, 16, 16)
Blé = (255, 248, 220)
Vert = (0, 255, 0)

# Chemin d'accès aux images
chemin_images = "chess_game/chess_images"

# Chargement des images
pieces_noires = {
    "Cavalier": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "bKN.png")), (Carre, Carre)),
    "Fou": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "bB.png")), (Carre, Carre)),
    "Roi": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "bK.png")), (Carre, Carre)),
    "Pion": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "bP.png")), (Carre, Carre)),
    "Reine": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "bQ.png")), (Carre, Carre)),
    "Tour": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "bR.png")), (Carre, Carre))
}

pieces_blanches = {
    "Cavalier": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "wKN.png")), (Carre, Carre)),
    "Fou": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "wB.png")), (Carre, Carre)),
    "Roi": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "wK.png")), (Carre, Carre)),
    "Pion": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "wp.png")), (Carre, Carre)),
    "Reine": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "wQ.png")), (Carre, Carre)),
    "Tour": pygame.transform.scale(pygame.image.load(os.path.join(chemin_images, "wR.png")), (Carre, Carre))
}
