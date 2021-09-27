# 创建和使用类

## 创建类 


```python
class Dog():
    """一次模拟小狗的简单尝试"""
    def __init__(self, name, age):
        """初始化属性name和age"""
        self.name = name
        self.age = age
        
    def sit(self):
        """模拟小狗被命令时蹲下"""
        print(self.name.title()+" is now sitting")
        
    def roll_over(self):
        """模拟小狗被命令时打滚"""
        print(self.name.title()+" rolled over")
```

## 根据类创建实例


```python
my_dog = Dog('willie', 6)

print("My dog's name is "+my_dog.name.title()+".")
print("My dog is "+str(my_dog.age)+" years old.")
```

    My dog's name is Willie.
    My dog is 6 years old.
    


```python
my_dog = Dog('willie', 6)

my_dog.sit()
my_dog.roll_over()
```

    Willie is now sitting
    Willie rolled over
    

### 类的知识
    最重要的是理解属性和方法
    方法类似函数
    属性联系现实世界中一个类型事物如何分类，根据不同事物中的共同点来区分，属性即共同点
    
    如何使用类
        创建类
        类中方法的使用：句点法

# 使用类和实例

## Car类


```python
class Car():
    """一次模拟汽车的简单尝试"""
    
    def __init__(self, make, model, year):
        """初始化描述汽车的属性"""
        self.make = make
        self.model = model
        self.year = year
        
    def get_descriptive_name(self):
        """返回整洁的描述性信息"""
        long_name =str(self.year)+ ' '+ self.make+' '+self.model
        return long_name.title()
    
my_new_car = Car('audi','a4',2016)
print(my_new_car.get_descriptive_name())
```

    2016 Audi A4
    

## 给属性指定默认值


```python
class Car():
    """一次模拟汽车的简单尝试"""
    
    def __init__(self, make, model, year):
        """初始化描述汽车的属性"""
        self.make = make
        self.model = model
        self.year = year
        self.odometer_reading = 0
        
    def get_descriptive_name(self):
        """返回整洁的描述性信息"""
        long_name =str(self.year)+ ' '+ self.make+' '+self.model
        return long_name.title()
    
    def read_odometer(self):
        """打印一条指出汽车里程的消息"""
        print("This car has " + str(self.odometer_reading)+" miles on it.")
        
my_new_car = Car('audi','a4',2016)
print(my_new_car.get_descriptive_name())
my_new_car.read_odometer()
```

    2016 Audi A4
    This car has 0 miles on it.
    

## 修改属性的值


```python
### 直接修改属性的值

my_new_car.odometer_reading = 23
my_new_car.read_odometer()
```

    This car has 23 miles on it.
    


```python
### 通过方法修改属性的值

class Car():
    """一次模拟汽车的简单尝试"""
    
    def __init__(self, make, model, year):
        """初始化描述汽车的属性"""
        self.make = make
        self.model = model
        self.year = year
        self.odometer_reading = 0
        
    def get_descriptive_name(self):
        """返回整洁的描述性信息"""
        long_name =str(self.year)+ ' '+ self.make+' '+self.model
        return long_name.title()
    
    def read_odometer(self):
        """打印一条指出汽车里程的消息"""
        print("This car has " + str(self.odometer_reading)+" miles on it.")
    
    def updata_odometer(self,mileage):
        """将里程表读书设置为指定的值"""
        self.odometer_reading = mileage
        
my_new_car = Car('audi','a4',2016)
print(my_new_car.get_descriptive_name())

my_new_car.updata_odometer(23)
my_new_car.read_odometer()
```

    2016 Audi A4
    This car has 23 miles on it.
    

# 继承

## 子类的方法


```python
class ElectricCar(Car):
    """电动汽车的独特之处"""
    def __init__(self, make, model, year):
        """初始化父类的属性"""
        super().__init__(make, model, year)
        
my_tesla = ElectricCar("tesla",'model s',2016)
print(my_tesla.get_descriptive_name())
```

    2016 Tesla Model S
    

## 给子类定义属性和方法


```python
class ElectricCar(Car):
    """电动汽车的独特之处"""
    def __init__(self, make, model, year):
        """初始化父类的属性"""
        super().__init__(make, model, year)
        self.battery_size = 70
    
    def describe_battery(self):
        """打印一条描述点评容量的信息"""
        print("This car has a "+str(self.battery_size)+"-kwh battery.")
        
my_tesla = ElectricCar("tesla",'model s',2016)
print(my_tesla.get_descriptive_name())
my_tesla.describe_battery()
```

    2016 Tesla Model S
    This car has a 70-kwh battery.
    

## 重写父类的方法

## 将实例用作属性


```python
class Battery():
    """"""
    def __init__(self,battery_size = 70):
        """"""
        self.battery_size = battery_size
        
    def describe_battery(self):
        """"""
        print("This car has a "+str(self.battery_size)+ "-kwh battery.")
        
class ElectricCar(Car):
    """电动汽车的独特之处"""
    def __init__(self, make, model, year):
        """
        初始化父类的属性
        再初始化电动汽车特有的属性
        """
        super().__init__(make, model, year)
        self.battery = Battery()

my_tesla = ElectricCar("tesla",'model s',2016)
print(my_tesla.get_descriptive_name())
my_tesla.battery.describe_battery()
```

    2016 Tesla Model S
    This car has a 70-kwh battery.
    


```python

```
