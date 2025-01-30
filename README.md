# TAREA12_SXE 🌐
---
Comienzo con los apartados tras haber realizado la instalación de la base de datos con la opción de “Demo
data”, y tras haber instalado las aplicaciones de facturación y contactos.
<details>
<summary> <b> Apartado 1 </b> </summary>

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

<details>
<summary> <b> Apartado 2 </b></summary>

```sql
INSERT INTO public.EmpresasFCT (nombre, quiereAlumnos, numAlumnos, fechaContacto)
VALUES
    ('Empresa1', TRUE, 2, '2025-03-15'),
    ('Empresa2', FALSE, 0, '2025-04-23'),
    ('Empresa3', TRUE, 1, '2025-02-04'),
    ('Empresa4', TRUE, 4, '2025-05-10'),
    ('Empresa5', FALSE, 0, '2025-03-12');
);
```
![imagen](https://github.com/user-attachments/assets/fc8b1e9f-30ac-4e7d-ba0c-520d0c53eb21)

Y este es el resultado:

![imagen](https://github.com/user-attachments/assets/e8854ec0-572a-4dfe-9523-cf02b6d8aa3c)

</details>

<details>
<summary> <b> Apartado 3 </b></summary>

```sql
select * from EmpresasFCT order by fechaContacto
```
![imagen](https://github.com/user-attachments/assets/efa226e7-30b7-45c2-b944-f7bb5b5d58db)

Y este es el resultado:

![imagen](https://github.com/user-attachments/assets/a428af17-32f6-429c-aaa3-eae5ab5040eb)

</details>

<details>
<summary> <b> Apartado 4 </b></summary>

```sql
select name, commercial_company_name from res_partner where city='Tracy' and is_company=False order by commercial_company_name
```
![imagen](https://github.com/user-attachments/assets/262bc9d3-adb3-40d7-bfab-ed01db14604a)

Y este es el resultado:

![imagen](https://github.com/user-attachments/assets/e0e9df50-dba5-4b45-b146-bb2a1f057f8c)

</details>

