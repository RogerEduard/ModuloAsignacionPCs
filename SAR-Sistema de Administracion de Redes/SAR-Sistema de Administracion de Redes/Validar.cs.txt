using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Windows.Forms;

namespace SAR_Sistema_de_Administracion_de_Redes
{
    class Validar
    {
        public static void SoloNumero(KeyPressEventArgs V)
        {
            if (char.IsDigit(V.KeyChar))
            { V.Handled = false; }
            else if (Char.IsSeparator(V.KeyChar))
            { V.Handled = false; }
            else if (Char.IsControl(V.KeyChar))
            { V.Handled = false; }
            else { V.Handled = true;
            MessageBox.Show("Debe ingresar DNI, solo numero");
            }
            


        }
    }
}
