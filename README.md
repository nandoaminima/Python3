# Python3

x= ["x","x","x"]
y = [ 0,0,0]
abrir = open("vitoria.txt","r")
for linha in abrir:
	linha.strip()
	X, Y = linha.split(",")
	Y = int(Y)
	if Y > min(y):
		x.pop(y.index(min(y)))
		y.remove(min(y))
		y.append(int(Y))
		x.append(X)
print(x)
print(y)
