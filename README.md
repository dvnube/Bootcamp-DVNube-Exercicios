# Bootcamp-DVNube-Exercicios

'Levantar do sofá', 
Se 'controle estive em suas mãos' então
'coloque no sofá' 
SeNão
'vá ao banheiro'
FimSe 

'Pegar a escova e a pasta de dente', 
'coloca a pasta na escova' e 'escova os dentes',
Se 'passou de 3 minutos escovando' Então 
'Abri a torneira' e 'leve a agua até a boca' e 'enxacha a boca',
Senão 
'Escove os dentes por 3 minutos' e 'abri a torneira' e 'leve a água até a boca' e 'enxacha a boca',
Fim se 

'Fecha a torneira' e 'Voltar para sala' 
Se 'Lugar no sofá esta ocupado' então 
'sentar no sofá em outro lugar',
Senão 
'Senta no sofá'
 FimSe
 
 
 public class Pseudocodigo {
	
    public  integer xubileu;
    private List<string> imprimir;
    
    private List<String> grupoA = new List<String>{'Levar do sofá, vá até ao banheiro', 'Pegar a escova e a pasta de dente', 'colocar a pasta na escova e escova os dentes','Ao abri a torneira, leva a agua até a boca e enxacha a boca','Cuspa a agua e leva a escova de dente', 'Volta para sala', 'Senta no sofá'};
    private List<String> grupoB = new List<String>{'Pegar a escova e a pasta de dente','Levar do sofá, vá até ao banheiro', 'Senta no sofá','Volta para sala','Ao abri a torneira'};
    private List<String> grupoC = new List<String>{'Cuspa a agua e leva a escova de dente','Senta no sofá','Pegar a escova e a pasta de dente', 'Volta para sala'};
    private List<String> grupoD = new List<String>{'Colocar a pasta na escova e escova os dentes','Senta no sofá'};
     
    public void ImprimirListaCorreta() {
        if (xubileu >= 90) {
            imprimir = grupoA;
        } else if (xubileu >= 80 && xubileu < 90) {
            imprimir = grupoB;
        } else if (xubileu >= 65 && xubileu < 80) {
            imprimir = grupoC;
        } else {
            imprimir = grupoD;
        }
        System.debug(imprimir);
    }    
}
