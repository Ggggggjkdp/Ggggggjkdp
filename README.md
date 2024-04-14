import pygame
import sys

# تهيئة Pygame
pygame.init()

# تحديد عرض وارتفاع النافذة
width, height = 800, 600
window = pygame.display.set_mode((width, height))
pygame.display.set_caption("مثال بسيط")

# لون الخلفية
bg_color = (255, 255, 255)

# الحلقة الرئيسية
running = True
while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # رسم الخلفية
    window.fill(bg_color)

    # تحديث الشاشة
    pygame.display.flip()

# إغلاق Pygame
pygame.quit()
sys.exit()
