# Applet in Java

* Applets are small Java applications that can be accessed on an Internet server, transported over Internet, and can be automatically installed and run as apart of a web document.
After a user receives an applet, the applet can produce a graphical user interface. 
* It has limited access to resources so that it can run complex computations without introducing the risk of viruses or breaching data integrity.
* Any applet in Java is a class that extends the java.applet.Applet class.
* An Applet class does not have any main() method. It is viewed using JVM. The JVM can use either a plug-in of the Web browser or a separate runtime environment to run an applet application.
* JVM creates an instance of the applet class and invokes init() method to initialize an Applet.

## Lifecycle of Java Applet

### Following are the stages in Applet
1.Applet is initialized.
2.Applet is started
3.Applet is painted.
4.Applet is stopped.
5.Applet is destroyed.

## java.applet.Applet class
For creating any applet java.applet.Applet class must be inherited. It provides 4 life cycle methods of applet.

* public void init(): is used to initialized the Applet. It is invoked only once.
* public void start(): is invoked after the init() method or browser is maximized. It is used to start the Applet.
* public void stop(): is used to stop the Applet. It is invoked when Applet is stop or browser is minimized.
* public void destroy(): is used to destroy the Applet. It is invoked only once.

## Example
```javascript
import java.awt.*;
import java.applet.*;
public class Simple extends Applet
{
 public void paint(Graphics g)
 {
  g.drawString("A simple Applet", 20, 20);
 }
}
```
## Advantages of Applet
* It works at client side so less response time.
 * It can be executed by browsers running under many plateforms, including Linux, Windows, Mac Os etc.

