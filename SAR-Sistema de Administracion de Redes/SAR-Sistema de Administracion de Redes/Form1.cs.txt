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
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void button1_Click(object sender, EventArgs e)
        {
            /*Form1.ActiveForm.Visible = false
            Form2.ActiveForm.Visible = true*/
            Form2 form2 = new Form2();
 
            form2.ShowDialog(); 


        }

        private void button2_Click(object sender, EventArgs e)
        {
            Form3 form3 = new Form3();

            form3.ShowDialog(); 

        }

        private void archivoToolStripMenuItem_Click(object sender, EventArgs e)
        {

        }

        private void salirToolStripMenuItem_Click(object sender, EventArgs e)
        {
            System.Environment.Exit(0);
        }

        private void equiposToolStripMenuItem1_Click(object sender, EventArgs e)
        {
            Form3 equipo = new Form3();
            equipo.MdiParent = this;
            equipo.Show();
        }

        private void usuariosToolStripMenuItem_Click(object sender, EventArgs e)
        {
            Form2 usuario = new Form2();
            usuario.MdiParent = this;
            usuario.Show();
        }
    }
}
