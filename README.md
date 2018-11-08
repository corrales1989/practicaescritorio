# practicaescritorio
proyecto ABC en c# con MVC

codigo reutilizable en capas

modo de uso:
Paso 1: crear un objeto de la clase "AdaptadorDatos "
Paso 2: validar si lleva o no lleva datos si no lleva se debera usar "Seleccionar_SP" de lo contrario "Seleccionar_SP_parametrizado"
Paso 3: mandar el nombre de SP en string, Arraylist Campos, Arraylist Valores

EJEMPLO:

private AdaptadorDatos _AdaptadorDatos;
        public void guardar(string Nombre_SP, ArrayList Campos_SP, ArrayList Valores_SP)
        {
            _AdaptadorDatos = new AdaptadorDatos();
            _AdaptadorDatos.Seleccionar_SP_parametrizado(Nombre_SP, Campos_SP, Valores_SP);

            /*foreach (string value in list)
            {
                MessageBox.Show(value.ToString());
            }*/

        }
