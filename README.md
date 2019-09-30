# counts-instances-through-oops




class Persons:
    count = 0
    def __init__(self,id,name,age):
        Persons.count += 1
        self.id = id
        self.name = name
        self.age = age

    def above_18(self):
        if self.age > 18:
            print('adult')
        else:
            print('Teenage')

    def display_all(self):
        return (f'{self.id} , {self.name} , and {self.age}')

p1 = Persons(10,'kamran',24)
p2 = Persons(20,'aisha',23)
p3 = Persons(30,'kishwar',21)

# print(p1.age)
# print(p1.display_all())
# print(p1.above_18())

print(Persons.count)
