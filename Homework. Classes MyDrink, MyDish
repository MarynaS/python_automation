
import random

dishes_string = ('eggs, Cake, cake, Spam, Spam   ,,, Butter, New, new, cookie, water , juice')
drink_string = ["Water","Juice","Sprite","Coffee"]

new_list =[]
dish_set = []

class MyServing():
    '''ALL that you ordered in the restaurant'''

    def __init__(self, dish_name):
            self.name = dish_name
 
    def call_time(self,random_a,random_b):
        '''Randomizer of a time'''
        dish_time = random.randint(random_a,random_b)
        return (dish_time)

    def print_dish(self, random_a,random_b):
        '''Print what you ordered and time'''
        print ("{:.<15}{:.>20} min"
        .format(self.name,self.call_time(random_a,random_b)))

class MyDrink (MyServing):
    '''Dish (Main cource) you ordered in the restaurant'''
    def __init__(self, drink_name):
        MyServing.__init__(self, drink_name)
        
    def print_drink(self):
        '''Print what you ordered and time'''
        print ("{:.<15}{:.>20} min"
        .format(self.name,5))

class MyDish(MyServing):
    '''Dish (Main cource) you ordered in the restaurant'''
    def __init__(self, dish_name):
        MyServing.__init__(self, dish_name)
 
    
for el in dishes_string.title().split(','):
    if el.strip() != "":
        new_list.append(el.strip())
        dish_ordered = list(set(new_list))

for dish in dish_ordered:
    if (dish in drink_string):
        time_for_drink = MyDrink(dish)
        time_for_drink.print_drink()
    else:
        time_for_dish = MyDish(dish)
        time_for_dish.print_dish(0,100)
        
# OUTPUT
# Butter...........................74 min
# Cake.............................37 min
# Water.............................5 min
# Spam..............................1 min
# Eggs.............................38 min
# Juice.............................5 min
# Cookie...........................37 min
# New..............................86 min


        
        
