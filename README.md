# test1


import pygame


#پنچره
pygame.init()
x = 10
y = 10
test = pygame.display.set_mode((950,100))




#رنگ
red  =  (255, 0, 0)
sabez = (0,255,0)
sfiid = (255,255,255)
khakestre = (70,70,80)
f = (0,255,255)
darck = (0,0,0)




#سرعت
speed = 500

#نام پنجره
pygame.display.set_caption("my game")



#متن
text = "Route: "
font = pygame.font.Font(None, 200)
t_s = font.render(text, True, (0,0,0))
t_r = t_s.get_rect()
t_r.center = (240, 100)




y_box = 950
x_boy = 100


while True :
 test.fill(sfiid)
 
 
 #حرکت
 for event in pygame.event.get():
  #1
  if event.type == pygame.QUIT:
   exit()
  if event.type == pygame.KEYDOWN:
   if event.key == pygame.K_q:
    y_box -= speed
    #2
  if event.type == pygame.KEYDOWN:
   if event.key == pygame.K_p:
    y_box += speed
    #مرز
    
    if 950 < y_box:
     y_box = 950
     #
     if 950 > y_box:
      y_box = 120
    
    
    	
    	
   
    #امتیاز
   
    
    
    
 test.blit(t_s, t_r)
  
 
 
 
 #شکل
 pygame.draw.rect(test,f, ((0, 1050),(9999,49)))
 pygame.draw.rect(test,darck, ((0, 1080),(9999
,9999)))

 pygame.draw.rect(test,f, ((450,10),(1000,200,)))
 
 e =  pygame.draw.rect(test,red,((25, y_box),(100,100)))
  
 pygame.draw.rect(test,darck, ((0, 210),(1500,10)))
 pygame.draw.rect(test,darck, ((0, 1080),(9999
,9999)))
  
  #_#_#_#_#_#_#_#_#_#_#_#_#_#
  
  
 pygame.display.update()
 
 
 
 
 
 
 
if __name__ == '__main__':
    main()
    
