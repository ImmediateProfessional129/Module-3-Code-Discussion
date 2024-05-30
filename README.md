# Module-3-Code-Discussion
This is my modified code for Module 3 Discussion

using System;

class Program
{
  static void Main()
  {
    Foo f = new Foo();
    Console.WriteLine("The x value of Foo class default constructor is {0}", f.X);
    f.X = 12;
    Console.WriteLine("The x value of Foo class is {0}", f.X);
  }
}

public class Foo
{
  private decimal x;
  //Default Constructor
  public Foo ()
  {
    x = 0;
  }
  //Properties
  public decimal X
  {
    get         { return x;  }
    set { x = value; }
    //private set { x = Math.Round (value, 2); }
  }

  public int Auto { get; private set; }  // Automatic property
}
