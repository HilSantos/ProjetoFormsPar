# ProjetoFormsPar
CRIE UM PROJETO DE FORMA QUE RECEBA UM VALOR INTEIRO E AO CLICAR NO BOTÃO E INFORME NUMA LABEL SE O NÚMERO É PAR OU ÍMPAR.

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace ProjetoFormsPar
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

  private void btnVerificar_Click(object sender, EventArgs e)
        {
            int numero = Convert.ToInt32(txtNumero.Text);

if (numero % 2 == 0)
            {
                lblResultado.Text = "O número é par.";
            }
            else 
            {
                lblResultado.Text = "O número é ímpar.";
            }
        }
    }
}
