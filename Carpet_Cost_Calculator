import java.util.*;
import java.lang.*;
class Floor

{
    double length;
    double width;
    Floor(double length, double width)
    {
        if(length < 0)
        {
            this.length = 0;
        }
        else {
            this.length = length;
        }
        if(width < 0)
        {
            this.width = 0;
        }
        else{
        this.width = width;
    }

    }
    public double getArea()
    {
        return length * width;
    }
}
class Carpet
{
    double cost;
    Carpet(double cost)
    {
        if(cost < 0)
        {
            this.cost = 0;
        }
        else
        {
            this.cost = cost;
        }
    }
    public double getCost()
    {
        return cost;
    }
}
class Calculator
{
    Floor floor;
    Carpet carpet;
    Calculator(Floor floor, Carpet carpet)
    {
        this.floor = floor;
        this.carpet = carpet;
    }
    public double getTotalCost()
    {
        return floor.getArea() * carpet.getCost();
    }
}
public class CarpetCostCalculator {
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the length and width of carpet : ");
        double len = sc.nextDouble();
        double wid = sc.nextDouble();
        Floor floor = new Floor(len, wid);
        System.out.println("The total area of carpet is " + floor.getArea());
        System.out.println("Enter the cost per square meter : ");
        double cos = sc.nextDouble();
        Carpet carpet = new Carpet(cos);
        Calculator calculator = new Calculator(floor, carpet);
        System.out.println("The total cost of the carpet is " + calculator.getTotalCost() + " rupees");
    }
}
