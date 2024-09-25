# Simulación de Cuenta Bancaria en C#

Este proyecto es una simulación básica de una cuenta bancaria utilizando dos clases en C#: `CuentaBancaria` y `Titular`. El programa permite crear titulares de cuentas, gestionar cuentas bancarias, realizar depósitos y retiros, y mostrar información sobre las cuentas y sus titulares.

## Características

- **Titular**: Representa a una persona titular de una cuenta bancaria, con atributos como nombre, apellido, dirección y teléfono.
- **CuentaBancaria**: Gestiona el saldo, número de cuenta y está asociada a un titular. Permite realizar operaciones de depósito y retiro.
  
## Clases

### Titular
```csharp
class Titular
{
    public string Nombre { get; set; }
    public string Apellido { get; set; }
    public string Direccion { get; set; }
    public string Telefono { get; set; }

    public Titular(string nombre, string apellido, string direccion, string telefono)
    {
        Nombre = nombre;
        Apellido = apellido;
        Direccion = direccion;
        Telefono = telefono;
    }

    public void MostrarInfo()
    {
        Console.WriteLine($"Titular: {Nombre} {Apellido}");
        Console.WriteLine($"Dirección: {Direccion}");
        Console.WriteLine($"Teléfono: {Telefono}");
    }
}
