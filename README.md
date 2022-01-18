

[![N|Solid](https://primeschool.pt/logo.png)](http://primeschool.pt/)

# Pygame CheatSheet

## import Pygame
```
import pygame
```

## Initilize Screen
```
screen = pygame.display.set_mode((1200, 1000))
```
## Draw a rect on screen
```
pygame.draw.rect(screen, color, (pos_x,pos_y, width, height))
pos_x = x co-ordinate
pos_y = y co-ordinate
color: color of rect lines
```

## Fill Screen with a Color
```
screen.fill((255,45,234))
```

## Load Image to pygame
```
background_image = pygame.image.load('background.jpg')
```
## Show Image to screen
```
screen.blit(background_image, (0,0)) ## starting at (0,0) can be given any co-ordinates on screen
```

## Scale Image to 2X
```
background_image = pygame.transform.scale2x(background_image)
```
## Scale Image to custom dimensions
```
background_image = pygame.transform.scale(background_image, (1000,900))
```

## Stop Program on pressing X button on screen
```
for event in pygame.event.get():
    if event.type == pygame.QUIT:
        print ("Pressed Quit Button")
        run = False
```


## Detect if a left key was pressed
```
    for event in pygame.event.get():
        if event.type == pygame.KEYDOWN:
            if event.key == pygame.K_LEFT:
                print ("Left key was pressed")
            if event.key == pygame.K_RIGHT:
                print ("Right key was pressed")
```

