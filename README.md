# Projet
import pygame
from pygame.locals import *

pygame.init()
### Dimension de l'écran (1300,650)
fenetre = pygame.display.set_mode((1300,650))
fond = pygame.image.load("background.jpg").convert()
fenetre.blit(fond,(0,0))
continuer = 0

while continuer==0 :
    for event in pygame.event.get():
        if event.type == QUIT:
            continuer = 1
        pygame.display.update()
pygame.quit()``
