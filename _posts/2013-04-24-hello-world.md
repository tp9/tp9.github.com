---
layout: post
title: "Hello world"
description: ""
category: 
tags: [pygame]
---
{% include JB/setup %}

    import pygame, sys
    from pygame.locals import *
    
    def main():
        pygame.init()
        DISPLAYSURF = pygame.display.set_mode((400,300))
        pygame.display.set_caption('Hello world')
        while True:
            for event in pygame.event.get():
                if event.type == QUIT:
                    pygame.quit()
                    sys.exit()
            titleFont = pygame.font.Font('freesansbold.ttf', 50)
            titleSurf = titleFont.render('Hello world!', True, (255,0,0))
            titleRect = titleSurf.get_rect()
            DISPLAYSURF.blit(titleSurf, titleRect)
            pygame.display.update()
            
    if __name__=='__main__':
        main()