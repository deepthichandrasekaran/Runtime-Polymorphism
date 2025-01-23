# Runtime-Polymorphism
package runtime;
class Shape {
    void draw() { 
        System.out.println("Drawing Shape");
    }
}

// Derived class
class Circle extends Shape {
    @Override
    void draw() { 
        System.out.println("Drawing Circle");
    }
}

// Derived class
class Rectangle extends Shape {
    @Override
    void draw() { 
        System.out.println("Drawing Rectangle");
    }
}
/**
 *
 * @author 1BSCCSA19
 */
public class Runtime {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        // TODO code application logic here
         Shape shape; 
        shape = new Circle();
        shape.draw(); 

        shape = new Rectangle();
        shape.draw(); }
}
        
    
Output
Drawing Circle
Drawing Rectangle
