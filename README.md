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



# Lists

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

### ArrayList vs LinkedList


### ArrayList

aaa.....bbb....ccc....ddd

0...........1...........2..........3

• When we try to insert a new object, the existing objects change their location. So the second object will be moved to the third place. Third object will be moved into the fourth location.

•If we delete an object, the third object will be placed into the second location. It will be shifted backwards. ArrayList isnt a recommanded choice.

ArrayList is not good when we are searching for an object(searching operation). ArrayList is not good when we are deleting or inserting an object.

► ArrayList implements randomAccess interface which provides Data Access.

ArrayList --> randomAccess --> provides Data Access

ArrayList is index based. 

index based: get(6) get(66) : searching

It will find the index within a short amount of time.


LinkedList is not based on index based


LinkedList: get(6) : searching

It will find the index, but it will take more time. It will go for every elemnt, which is sequential search. LinkedList is not good for index based.


### LinkedList

LinkedList will e arranged in double linked format.

insertion deletion ---> adjust one link


If we delete the second element, one will connect to three in LinkedList. If we delete the second and third element, one will connect to the fourth element. For the fifth, sixth and seventh elemnt, no changes will be required.


►In LinkedList format, if we insert and delete an object/element, there will be only a few changes. In ArratList, if we insert and delete an object/element, there will be many changes. Therefore, insertion and deletion is not recommanded in ArrayList. Also, it will take more time.




 

