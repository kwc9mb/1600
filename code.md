# Sample Code
## C# Code Block
<pre><code>using System;
using System.Collections.Generic;
namespace MenuOrder
{
    class Program
    {
        static void Main(string[] args)
        {
            bool moreItems = true;
            float orderTotal = 0;
            Dictionary<string,float> Menu = new Dictionary<string, float>(){
                {"Baja Taco",(float)4},{"Burrito",(float)7.5},{"Bowl",(float)8.5},
                {"Nachos",(float)11},{"Quesadilla",(float)8.5},{"Super Burrito",(float)8
                {"Super Quesadilla",(float)9.5},{"Taco",(float)3},{"Tortilla Salad",(flo
            };
            
            while(moreItems){
                Console.WriteLine("\nItem:");
                string menuEntry = Console.ReadLine();
                if(Menu.ContainsKey(menuEntry)){
                    orderTotal += Menu[menuEntry];
                    Console.WriteLine($"Total: ${orderTotal:0.00}");
                }else if(menuEntry.Equals("end", StringComparison.InvariantCultureIgnore
                    moreItems = false;
                }
            }
        }
    }
}
</code></pre>

### __Navigation__
- __[Home](/README.md)__ - README.md
- __[Courses](/courses.md)__ - Current and Past 
- __[About Me](/aboutme.md)__ - Information
- __[Contact](/contact.md)__ - Contact Information


