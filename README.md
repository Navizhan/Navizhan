import java.awt.*;
import java .awt.event.*;

public class Calculator extends Frame{

Button b0,b1,b2,b3,b4,b5,b6,b7,b8,b9,badd,bsub,bmul,bdiv,beq,bclr;
TextField textField = new TextField();


public Calculator(){
setTitle("CALCULATOR");
setSize(400, 300);
setLayout(new GridLayout(7, 2));
setResizable(false);

Panel p= new Panel(new FlowLayout(FlowLayout.CENTER));
add(p);

b0= new Button("0");
b0.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "0");
}
});
add(b0);


b1 = new Button("1");
b1.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "1");
}
});
add(b1);

b2= new Button("2");
b2.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "2");
}
});
add(b2);

b3 = new Button("3");
b3.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "3");
}
});
add(b3);

b4 = new Button("4");
b4.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "4");
}
});
add(b4);


b5 = new Button("5");
b5.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "5");
}
});
add(b5);


b6 = new Button("6");
b6.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "6");
}
});
add(b6);


b7 = new Button("7");
b7.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "7");
}
});
add(b7);


b8 = new Button("8");
b8.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "8");
}
});
add(b8);

b9 = new Button("9");
b9.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "9");
}
});
add(b9);

badd = new Button("+");
badd.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "+");
}
});
add(badd);

bsub = new Button("-");
bsub.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "-");
}
});
add(bsub);

bmul = new Button("*");
bmul.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "*");
}
});
add(bmul);

bdiv = new Button("/");
bdiv.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText(textField.getText() + "/");
}
});
add(bdiv);

beq = new Button("=");
beq.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
String expression = textField.getText();
double result = calculateResult(expression);
textField.setText(String.valueOf(result));
    }
});
add(beq);

bclr = new Button("clr");
bclr.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
textField.setText("");
}
});
add(bclr);
}


public double calculateResult(String expression) {
double result = 0.0;
return result;
}

public static void main(String[] args) {
Calculator calculator = new Calculator();
calculator.setVisible(true);
}

} rectify and modify this program


