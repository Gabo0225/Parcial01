# Parcial – Paradigmas de Programación

# Gabriel Santamaria Hernandez - parcial-4

## Errores encontrados en estructural.py

- El error es de sintaxis (no se ejecuta)
- El la linea 11 hace falta cerrar un parentesis para llamar corerctamente la función
  ```python
  print(invertir_lista([1,2,3,4,5])

- Linea corregida
  ```python
  print(invertir_lista([1,2,3,4,5]))

## Errores encontrados en opp.py

- El error es de lógica.
- El `if` de la función `def retirar(self, cantidad):` únicamente evalúa el caso cuando la cantidad a retirar es menor que el saldo.
- Código original:
  ```python
  if cantidad < self.saldo:
      self.saldo = self.saldo - cantidad

- Se debe poder retirar la cantidad igual a la que hay en el momento; adicionalmente, que muestre el saldo después de hacer el retiro.
- Línea corregida:

```python
def retirar(self, cantidad):
    if cantidad <= self.saldo:
        self.saldo = self.saldo - cantidad
        print(f"Tu saldo actual es {self.saldo}")

