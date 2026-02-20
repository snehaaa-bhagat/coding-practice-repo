

class Tyres:
    def __init__(self, name, t_type, width):
        self.name = name
        self.t_type = t_type
        self.width = width
    
    def __str__(self):
        return "Tyres:\t Branch: "+self.name+"\n \t type: "+self.t_type+"\n \t width: "+self.width
class Engine:
    def __init__(self, fuel_type, noise_level):
        self.fuel_type = fuel_type
        self.noise_level = noise_level
        
    def __str__(self):
        return "Engine: \n \t Fuel Type:"+str(self.fuel_type)+"\n \tnoise level: "+str(self.noise_level)
class Body:
    def __init__(self, size):
        self.size = size
    def __str__(self):
        return "Body \n \tsize: "+self.size
class Car:
    def __init__(self, tyres, engine, body):
        self.tyres = tyres
        self.engine = engine
        self.body = body
        
    def __str__(self):
        return str(self.tyres)+"\n"+str(self.engine)+"\n"+str(self.body)
tyres = Tyres("MRF", "Offroad", "16 inches")
engine = Engine("Petrol", 3)
body = Body("Large")
car = Car(tyres, engine, body)
car = Car("MRF", "Petrol", "SUV")
print(car)
