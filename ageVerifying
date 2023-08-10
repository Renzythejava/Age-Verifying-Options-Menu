import javax.swing.*;
import java.awt.*;
import java.net.MalformedURLException;
import java.net.URL;

public class ageVerifying {
    public static void main(String[] args) {
        ageVerifying ageVerifier = new ageVerifying();
        ageVerifier.verifyAge();
    }

    public void verifyAge() {
        int choice = JOptionPane.showConfirmDialog(null,
                "18 yaşından büyük müsünüz?", "Yaş Doğrulama",
                JOptionPane.YES_NO_OPTION, JOptionPane.QUESTION_MESSAGE, createIcon());

        if (choice == JOptionPane.YES_OPTION) {
            JOptionPane.showMessageDialog(null, "Hoşgeldiniz!");
        } else {
            System.exit(0);
        }
    }

    private Icon createIcon() {
        ImageIcon icon = null;
        try {
            URL imageUrl = new URL("https://www.pngplay.com/wp-content/uploads/2/Question-Mark-Background-PNG.png"); // Resim URL'sini buraya girin
            Image image = new ImageIcon(imageUrl).getImage().getScaledInstance(100, 100, Image.SCALE_SMOOTH);
            icon = new ImageIcon(image);
        } catch (MalformedURLException e) {
            e.printStackTrace();
        }
        return icon;
    }
}
