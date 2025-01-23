# run-time-polymorphism
package run.time.polymorphism;
class Vehicle {
    void start() {
        System.out.println("Vehicle is starting...");
    }
}

class Car extends Vehicle {
    @Override
    void start() {
        System.out.println("Car is starting...");
    }
}

class Bike extends Vehicle {
    @Override
    void start() {
        System.out.println("Bike is starting...");
    }
}


/**
 *
 * @author 1BSCCSA43
 */
public class RunTimePolymorphism {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
    Vehicle myVehicle;
     
    myVehicle = new Car();
        myVehicle.start(); 

        myVehicle = new Bike();
        myVehicle.start(); 
    }
}

    
output 

Car is starting...
Bike is starting...
BUILD SUCCESSFUL (total time: 0 seconds)


