```python
import random
import time

class DevBienvenida:
    def __init__(self):
        self.nombre = "Joel Cruz"
        self.usuario = "Joel252"
        self.stack = [".NET", "Python", "React", "SQL", "AWS", "Terraform"]
        self.location = "Chetumal, México 🇲🇽";
        self.mensaje = [
            "Codificando el futuro...",
            "Compilando sueños en realidades...",
            "Refactorizando la vida..."
        ]

    def __str__(self):
        return f"👋 ¡Hola! Soy {self.nombre} (@{self.usuario})\n" \
               f"💻 Stack: {', '.join(self.stack)}\n" \
               f"🎯 {random.choice(self.mensaje)}"

    def boot(self):
        for _ in range(3):
            print("🔄 Inicializando perfil...", end="\r")
            time.sleep(1)
        print(self)

if __name__ == "__main__":
    yo = DevBienvenida()
    yo.boot()
```
