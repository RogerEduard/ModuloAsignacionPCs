using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Windows.Forms;

namespace SAR_Sistema_de_Administracion_de_Redes
{
    public partial class Form2 : Form
    {
        public Form2()
        {
            InitializeComponent();
        }

        private void Form2_Load(object sender, EventArgs e)
        {
           

        }

        

        private void textBox2_KeyPress(object sender, KeyPressEventArgs f)
        {
            Validar.SoloNumero(f);
        }

        private void textBox2_TextChanged(object sender, EventArgs e)
        {
            double parsedValue;

            if (!double.TryParse(textBox2.Text, out parsedValue))
            {
                textBox2.Text = "";
            }
        }

        private void button2_Click(object sender, EventArgs e)
        {
            Form2.ActiveForm.Visible = false;
        }

        

       

       

        

       

        
    }
}
