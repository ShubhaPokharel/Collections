# Collections

Collections are group of objects.

#### Two types of Collection-

1. Lists
   
2. Sets


► Lists are used to store the duplicates and it is ordered

ex: abcde ---> abcde

In lists,we have ArrayList and LinkedList

► Sets are used to store the unique values and it is un-ordered.

ex: abcde ---> dbace

In Sets,we have HasSet,LinkedHashSet, and TreeSet.

- In Collection data, the index starts from zero

 
 Example 1-

 package com.pnc.bank;

import java.util.ArrayList;

public class ArrayListEx1 {

	public static void main(String[] args) {
 
		ArrayList objects = new ArrayList();
  
		objects.add(10); //0
  
		objects.add(10.3);//1
  
		objects.add("ratan");//2
  
		objects.add('A');//3
  
		objects.add(10);//4
  
		System.out.println(objects);
  
		System.out.println("The size of the objects- " + objects.size());
  
		
		Integer first = (Integer) objects.get(0);
  
		System.out.println("The first element "+first);
  
		
		Double second = (Double) objects.get(1);
  
		System.out.println("The second element "+second);
  
		
		Integer last = (Integer) objects.get(objects.size()-1);
  
		System.out.println("The last element "+last);
  
		
		// TODO Auto-generated method stub

	}

}

Right now,we have 5 objects but in general we can have to one thousand objects. Type Casting is only good for when we have a few objects. To overcome that issue we can use generics. <>

Generics mean "what type of data we can hold". Generics is what represents what type of data collection can hold. It only holds one type of data type, so type casting is not required.

Example 2 Generics-

public class ArrayListEx2{

   public static void main(Staring[] args){

      ArrayList<String> names = New ArrayList<String>();

      names.add("ratan");
      
      names.add("shubha");
      
      names.add("srayva");
      
      names.add("anu");
      
      names.add("john");

      String first = names.get(0);
      
      System.out.println("This is the first element:" + first);

      String third = names.get(2);
      
      System.out.println("This is the third element:" + third);

      String last = names.get(names.get() -1);

      //printing the data in COllection format

      System.out.println(names);

      //iterating all elements and printing

      for(String name: names){

         System.out.println("your name" + name);
         
      }

      //iterating the data using loop

      for(int i = 0; i<names.size(); i++){

         Syste.out.println("your name "+ names.get(i));
      }
      
     
   }
   
}

_____


aaa              bbb               ccc             ddd


