# Saludos en GO

Este paquete proporciona una forma rapida de obtener saludos

## Instalación
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/CARLOSDOZA/greetings
```
## Uso
Aqui tiene un ejemplo de uso:

```go
package main

import (
	"fmt"
	"log"
	"github.com/CARLOSDOZA/greetings"
)

func main() {
	log.SetPrefix("greetings: ")
	log.SetFlags(0)
	names := []string {
		"Carlos", "Carla", "Omar",
	}

	messages, err := greetings.Hellos(names)
	if err != nil {
		log.Fatal(err)
	}
	
	fmt.Println(messages)
}
```

