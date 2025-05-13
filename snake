import pygame

# Инициализация Pygame
pygame.init()

BLACK = (0, 0, 0)
WHITE = (255, 255, 255)
# Размеры окна
WIDTH = 800
HEIGHT = 400


#Карта
map_width = 2000
map_height = 400

# Создание окна
screen = pygame.display.set_mode((WIDTH, HEIGHT))
pygame.display.set_caption("Камера в Pygame")

class Hero():
    def __init__(self, x, y):
       self.x = x
       self.y = y
    def draw(self, screen, camera_x, camera_y):
        pygame.draw.rect(screen, WHITE, (camera_x, camera_y, 32, 32))
        
hero = Hero(10, 10)
clock = pygame.time.Clock()
# Основной цикл игры
running = True
while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # Очистка экрана
    hero.draw(screen, 10, 10)

    # Обновление экрана
    pygame.display.flip()
    clock.tick(60)
# Завершение работы Pygame
pygame.quit()
