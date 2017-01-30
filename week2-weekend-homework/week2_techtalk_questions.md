'''What is self? Why do all classes and methods need self?''' 

#Self is how you access variables inside a particular class; self also refers to a newly created object in other class methods. 
#It refers to the instance whose method that is called; also, self has to be the first parameter within a class. 
#So, whatever self is before the period is what your object is before the period. 
#The reason why classes and methods need self is because it is a temporay placeholder for the object



class Securitization: 
	def __init__(self, select, package, name):
		self.select = select
		self.package = package 
		self.name = name 

	def MBS_name(self):
		name = input('What kind of MBS is this?')
		if type(self.name) is str:
			print('CDO, but you can also buy a CDS as insurance against default')
			return True 
		elif type(self.name) is str:
			print ('')
			return True 
		else: 
			print('High default risk')
			return False


MBS1 = Securitization('Mortgages', 'DB', 'CDO')
MBS2 = Securitization('CC debt', 'GS', 'CLO')

Securitization.MBS_name(MBS1)