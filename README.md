# Parcial – Paradigmas de Programación

# Gabriel Santamaria Hernandez - parcial-4

## Errores encontrados en estructural.py

- El error es de sintaxis (no se ejecuta)
- El la linea 11 hace falta cerrar un parentesis para llamar corerctamente la función
´print(invertir_lista([1,2,3,4,5])´

- Linea corregida
´print(invertir_lista([1,2,3,4,5]))´

## Errores encontrados en opp.py

- EL error es de logica 
- El ´if´ de la funcion ´def retirar(self, cantidad):´ unicamente evalua el caso cuando la cantidad a retirar es menor a la que hay
´if cantidad < self.saldo:
            self.saldo = self.saldo - cantidad´

- Se debe poder retirar la cantidad igual a la que hay en el momento, adicional que muestre el saldo despues de hacer el retiro 
- Linea corregida
´def retirar(self, cantidad):
        if cantidad <= self.saldo:
            self.saldo = self.saldo - cantidad
            print(f"tu saldo actual es {self.saldo}")´

