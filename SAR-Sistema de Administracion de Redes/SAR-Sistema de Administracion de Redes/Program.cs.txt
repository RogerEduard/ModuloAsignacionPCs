using System;
using System.Collections.Generic;
using System.Linq;
using System.Windows.Forms;

namespace SAR_Sistema_de_Administracion_de_Redes
{
    static class Program
    {
        /// <summary>
        /// Punto de entrada principal para la aplicación.
        /// </summary>
        [STAThread]
        static void Main()
        {
            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            Application.Run(new Form1());
        }
    }
}
