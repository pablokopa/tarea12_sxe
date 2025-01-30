# TAREA12_SXE 🌐
---
Comienzo con los apartados tras haber realizado la instalación de la base de datos con la opción de “Demo
data”, y tras haber instalado las aplicaciones de facturación y contactos.
<details>
<summary> <h2><b> Apartado 1 </b> </h2></summary>

Para crear la tabla de 'EmpresasFCT' he escrito lo siguiente:
```sql
CREATE TABLE IF NOT EXISTS public.EmpresasFCT(
	idEmpresa SERIAL PRIMARY KEY,
	nombre VARCHAR(40),
	quiereAlumnos BOOLEAN,
	numAlumnos INTEGER,
	fechaContacto DATE
);
```
![imagen](https://github.com/user-attachments/assets/7745f670-2eb7-4de2-aa06-9e1ba84d2cab)

Y este es el resultado:

![imagen](https://github.com/user-attachments/assets/7bb2d4d9-c4b8-4841-a4dc-da3c75803831)

</details>

