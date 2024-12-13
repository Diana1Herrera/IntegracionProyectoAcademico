Integración de proyecto academico

Descripción del proyecto
Este proyecto es una aplicación de escritorio desarrollada en C# utilizando Windows Forms, diseñada para gestionar la información de estudiantes que toman clases de música. La aplicación permite ingresar datos del estudiante, calcular costos y generar informes.

Funcionalidades principales
Ingreso de Datos: Permite al usuario ingresar información como ID, nombre, instrumento, género, número de clases y costo por clase.
Cálculo de Costos: Calcula el costo total del curso basado en el número de clases y el costo por clase.
Interfaz Gráfica: Utiliza un diseño intuitivo para facilitar la interacción del usuario.
Visualización : Permite visualizar un árbol binario en una interfaz gráfica.
Recorridos : Implementa métodos para recorrer el árbol (preorden, inorden, postorden).

Tecnologías utilizadas
Lenguaje de programación: C#
Marco de trabajo: .NET Framework
Interfaz Gráfica: Windows Forms

Estructura del proyecto
El proyecto está organizado en varias clases que representan diferentes componentes de la aplicación:
Form1: Pantalla principal que maneja el inicio de sesión.
fmrMenu: Menú principal donde se pueden seleccionar diferentes opciones.
GestionEstudiantes: Clase que gestiona la información del estudiante.
IngresoDeDatos: Formulario para ingresar los datos del estudiante.

Código relevante
Ingreso de datos y validación de la contraseña:
csharp
Copy code
private void button1_Click(object sender, EventArgs e) {  
    string laClave = this.txtContrasena.Text.Trim();  
    if (laClave.Equals("")) {  
        this.txtContrasena.Focus();  
    }  
    if (!laClave.Equals(clave)) {  
        this.error.SetError(this.txtContrasena, "Contraseña inválida.");  
        this.txtContrasena.Focus();  
    } else {  
        fmrMenu menuOpciones = new fmrMenu();  
        menuOpciones.Show();  
        this.Hide();  
    }  
}  
Instrucciones para Ejecutar el Proyecto
Clona el repositorio desde GitHub:
bash
Copy code
git clone https://github.com/Diana1Herrera/IntegracionProyectoAcademico.git
