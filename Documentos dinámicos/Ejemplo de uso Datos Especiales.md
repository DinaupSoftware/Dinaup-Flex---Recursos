
# Ejemplo de uso datos Especiales

Este ejemplo demuestra cómo utilizar los datos especiales en DinaScript dentro de un documento dinámico. El código muestra cómo acceder y mostrar diversas variables del sistema, datos de la sesión actual y información de la empresa.

## Código
```
<!doctype html>
<html>
   <head>
      <link rel="stylesheet" href="https://cdn.dinaup.com/dinaup/link/bootstrap.min.css">
      <meta charset="utf-8">
      <title>Ejemplo de Uso de Datos Especiales en DinaScript</title>
   </head>
   <body>
      <div class="container">
         <h1>Ejemplo de Uso de Datos Especiales en DinaScript</h1>
         <p>Este documento muestra cómo acceder a diferentes datos especiales proporcionados por DinaScript.</p>
         
         <h2>Información de la Sesión Actual</h2>
         <p>Nombre del Usuario: <b><!--: F.WriteText(D.SesionActual.TextoPrincipal) :--></b></p>
         <p>Cargo en la Empresa: <b><!--: F.WriteText(D.SesionActual.ReferenciaCargoEnEmpresa.TextoPrincipal) :--></b></p>
         <p>Correo Electrónico: <b><!--: F.WriteText(D.SesionActual.CorreoElectronico) :--></b></p>

         <h2>Información de la Empresa Actual</h2>
         <p>Nombre de la Empresa: <b><!--: F.WriteText(D.EmpresaActual.TextoPrincipal) :--></b></p>
         <p>Ejercicio Actual: <b><!--: F.WriteText(D.EmpresaActual.ReferenciaEjercicio.TextoPrincipal) :--></b></p>
         <p>Registro Mercantil: <b><!--: F.WriteText(D.EmpresaActual.RegistroMercantilDe) :--></b></p>
         <p>Razón Social: <b><!--: F.WriteText(D.EmpresaActual.ReferenciaDatosFiscales.ApellidosYNombreORazonSocial) :--></b></p>

         <h2>Datos Especiales del Sistema</h2>
         <p>Fecha Actual: <b><!--: F.WriteText(D.DatosEspeciales.FechaActual) :--></b></p>
         <p>Inicio del Trimestre: <b><!--: F.WriteText(D.DatosEspeciales.FechasAvanzadas.Inicios.InicioDeTrimestre) :--></b></p>
         <p>Fin del Trimestre: <b><!--: F.WriteText(D.DatosEspeciales.FechasAvanzadas.Finales.FinDeTrimestre) :--></b></p>

         <h2>Información del Sistema</h2>
         <p>Versión del Sistema: <b><!--: F.WriteText(D.DatosEspeciales.Sistema.Version) :--></b></p>
         <p>Año Actual: <b><!--: F.WriteText(D.DatosEspeciales.AñoActual) :--></b></p>
         <p>Día Actual: <b><!--: F.WriteText(D.DatosEspeciales.DiaActual) :--></b></p>
         <p>Día de la Semana: <b><!--: F.WriteText(D.DatosEspeciales.DiaDeLaSemanaActual) :--></b></p>
         <p>Hora Actual: <b><!--: F.WriteText(D.DatosEspeciales.HoraActual) :--></b></p>
         <p>Mes Actual (Número): <b><!--: F.WriteText(D.DatosEspeciales.MesActual) :--></b></p>
         <p>Fecha y Hora Actual: <b><!--: F.WriteText(D.DatosEspeciales.FechaYHoraActual) :--></b></p>
         <p>Mes Actual (Nombre): <b><!--: F.WriteText(D.DatosEspeciales.MesActualNombre) :--></b></p>
      </div>
   </body>
</html>

```