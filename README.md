from random import*
from time import*
round = 3
ball_bot = 0
ball_user = 0
while True :
 if round == 0:
  break
 user = input('введите свой выбор , камень ножницы или бумага')
 a = randint (1 , 3)
 if a == 1:
   print('бот выбрал камень')
   a = 'камень'
 elif a == 2:
   print('бот выбрал ножницы')
   a = 'ножницы'
 elif a == 3:
    print('бот выбрал бумагу')
    a = 'бумага'
 if user == a:
   print('ничья')
 elif user == 'бумага' and a == 'камень':
   print('игрок выиграл')
   ball_user += 1
 elif user == 'камень' and a == 'ножницы':
   print('игрок победил')
   ball_user += 1
 elif user == 'ножницы' and a == 'бумага':
   print('игрок победил')
   ball_user += 1 
  else:
    print('выиграл бот')
 round -= 1
print('конец игры', 'баллы игрока:', ball_user  , 'баллы бота:' , ball_bot)
