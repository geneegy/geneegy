import javax. swing.*; import java. awt.*;
import java. awt. event.*;
public class SwingComponents extends Frame implements Actionlistener
FlowLayout fl = new FlowLayout () ;
Font bFont = new Font ("Arial", Font.BOLD, 16);
JLabel 1b1 = new JLabel ("Enter your name: ");
TextField tf = new TextField (10) ;
Button bt = new Button ("Click me");
JLabel 1b2 = new JLabel ("");
public SwingComponents ()
bt. addActionlistener (this) ;
super ("Sample Event");

setSize (275, 225);

setLayout （£1）；

1b1. setFont (bFont) ;

1b2. setFont (bFont) ;

add (1b1) ;

add (tf) ;

add (bt);

add (1b2) ;


setDefaultcloseperation (Frame. EXIT _ON CIOSE) ;
public void actionPerformed (ActionEvent e)
String name = tf.getText () ;
String greet = "Hi, "+ name + "!";
1b2. setText (greet) ;
