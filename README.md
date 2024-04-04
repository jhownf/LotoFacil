# LotoFacil
LotoFacil primeira entrega
import javax.swing.*;
import java.awt.event.*;

public class LotoFacilGUI {
    private JFrame frame;
    private JPanel panel;
    private JButton btnAposta0a100, btnApostaAaZ, btnApostaParImpar, btnSair;

    public LotoFacilGUI() {
        frame = new JFrame("LOTOFÁCIL");
        panel = new JPanel();
        btnAposta0a100 = new JButton("Apostar de 0 a 100");
        btnApostaAaZ = new JButton("Apostar de A à Z");
        btnApostaParImpar = new JButton("Apostar em par ou ímpar");
        btnSair = new JButton("Sair");

        btnAposta0a100.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                JOptionPane.showMessageDialog(null, "Implemente a lógica para apostar de 0 a 100 aqui.");
            }
        });

        btnApostaAaZ.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                JOptionPane.showMessageDialog(null, "Implemente a lógica para apostar de A à Z aqui.");
            }
        });

        btnApostaParImpar.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                JOptionPane.showMessageDialog(null, "Implemente a lógica para apostar em par ou ímpar aqui.");
            }
        });

        btnSair.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                frame.dispose();
            }
        });

        panel.add(btnAposta0a100);
        panel.add(btnApostaAaZ);
        panel.add(btnApostaParImpar);
        panel.add(btnSair);

        frame.add(panel);
        frame.setSize(300, 200);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setVisible(true);
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(new Runnable() {
            public void run() {
                new LotoFacilGUI();
            }
        });
    }
}
