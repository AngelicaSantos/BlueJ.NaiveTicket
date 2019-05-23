# NaiveTicket

The second Objects lab, from the BlueJ book's second chapter.

Look for the [Chapter 2 file](./doc/BlueJ-objects-first-ch2.pdf) you need in the [doc](./doc) folder.
There is 35 pages of reading and exercises in the chapter.

Work through all these exercises. You edit this file with your answers for these exercises.

### Exercise 2.1
* Create a TicketMachine object on the object bench.
* Upon viewing its methods, `getBalance`, `getPrice`, `insertMoney`, `printTicket`.
* Use `getPrice` method to view the value of the price of the tickets that was set when this object was created.
* Use `insertMoney` method to simulate inserting an amount of money into the machine.
* Use `getBalance` to check that the machine has a record of the amount inserted.
	* You can insert several separate amounts of money into the machine, just like you might insert multiple coins or notes into a real machine. Try inserting the exact amount required for a ticket. As this is a simple machine, a ticket will not be issued automatically, so once you have inserted enough money, call the `printTicket` method. A facsimile ticket should be printed in the BlueJ terminal window.

### Exercise 2.2
* What value is returned if you check the machine’s balance after it has printed a ticket? 0

### Exercise 2.3
* Experiment with inserting different amounts of money before printing tickets.
	* Do you notice anything strange about the machine’s behavior? The machine does not make any changes.
	* What happens if you insert too much money into the machine – do you receive any refund? No. 
	* What happens if you do not insert enough and then try to print a ticket? It still does not change anything.

### Exercise 2.4
* Try to obtain a good understanding of a ticket machine’s behavior by interacting with it on the object bench before we start looking at how the `TicketMachine` class is implemented in the next section.

### Exercise 2.5
* Create another ticket machine for tickets of a different price.
	* Buy a ticket from that machine.
	* Does the printed ticket look different? Yes. 

### Exercise 2.6
* Write out what you think the outer wrappers of the `Student` and `LabClass` classes might look like – do not worry about the inner part. 

public class Student 
{
Inner part 
}

public class LabClass
{
Inner part 
}

### Exercise 2.7
Does it matter whether we write<br>
`public class TicketMachine`<br>
or<br>
`class public TicketMachine`<br>
in the outer wrapper of a class? Yes it matters.  

* Edit the source of the `TicketMachine` class to make the change and then close the editor window.
	* Do you notice a change in the class diagram? yes. 
	* What error message do you get when you now press the compile button? <indentifier> expected

	* Do you think this message clearly explains what is wrong? Yes. Public would be the identifier.

### Exercise 2.8
* Check whether or not it is possible to leave out the word `public` from the outer wrapper of the `TicketMachine` class. Yes. 

### Exercise 2.9
* From your earlier experimentation with the ticket machine objects within BlueJ you can probably remember the names of some of the methods – `printTicket`, for instance.
	* Look at the class definition in Code 2.1 and use this knowledge, along with the additional information about ordering we have given you, to try to make a list of the names of the fields, constructors, and methods in the `TicketMachine` class.
	* Hint: There is only one constructor in the class.

Fields: price, balance, and total 
Constructor: ticketCost 
Methods: getPrice(), getBalance(), insertMoney(), printTicket()

### Exercise 2.10
* Do you notice any features of the constructor that make it significantly different from the other methods of the class? A constructor does not have a return type. 

### Exercise 2.11
* What do you think is the type of each of the following fields?


```java
private int count; this is a type of integer.
private Student representative; this is a type of String. 
private Server host; this is also a type of String.
```

### Exercise 2.12
* What are the names of the following fields?

```java
private boolean alive; named alive 
private Person tutor; named tutor 
private Game game; named game 
```
### Exercise 2.13

In the following field declaration from the TicketMachine class<br>

```java
private int price;
```
does it matter which order the three words appear in? Yes, the order matters. 
* Edit the `TicketMachine` class to try different orderings. After each change, close the editor.
	* Does the appearance of the class diagram after each change give you a clue as to whether or not other orderings are
possible? An error occurs which lets me know the order does matter. 
	* Check by pressing the compile button to see if there is an error message.
	* Make sure that you reinstantiate the original version after your experiments!

### Exercise 2.14
* Is it always necessary to have a semicolon at the end of a field declaration? Yes it is necessary to have a semicolon to let the program know it is the end of a declaration. 

* Once again, experiment via the editor.
* The rule you will learn here is an important one, so be sure to remember it.


### Exercise 2.15
* Write in full the declaration for a field of type `int` whose name is `status`.

 Private int status; 

### Exercise 2.16
* To what class does the following constructor belong? It belongs to the class "student" 
```
public Student(String name)
```

### Exercise 2.17
* How many parameters does the following constructor have and what are their types? 2 parameters. The first one is a type string and the second one is a type double. 
```
public Book(String title, double price)
```

### Exercise 2.18
* Can you guess what types some of the `Book` class’s fields might be?  
* Can you assume anything about the names of its fields? The author and the title could be string types. Year published is a int type.

Work all Exercises from 2.19 to 2.58 that are **NOT** marked *Challenge exercise*.
READ upto and INCLUDING section 2.15 of this chapter.

2.19- public Pet(String petsName)
{

name=petsName; 

}

2.21- getPrice() will return the price of a ticket. getBalance() will return the total amount of money in the machine.

2.22- I would characterize a getBalance as 'What is the current balance in the ticket machine?'

2.23- no it does not to be changed. 

2.24- Done

2.25- missing return statement 

2.26- getPrice is an integer type. printTicket is a void type meaning it does not return a value instead it prints out a ticket. 

2.27- no. the insertMoney and printTicket methods do not have return statements because they do not require a value to be returned. Insert money message is stating to receive money from a customer. Print ticket method is asking for the ticket to be printed. 

2.28- done 

2.29- setPrice is a method because it has a return type and therefore is not a constructor. 

2.30- done

2.31-done

2.32-done 

2.33-done

2.34-done

2.35-no because each one has different set amounts. 

2.36- if you put quotation marks around price, it would not be a parameter anymore. Instead it would become a string. 

2.37- a single parameter would not be constructed. Price is still in the quotation marks which makes it a string. 

2.38-no because in both examples, print was turned to a string and no longer a variable. 

2.39- it is now set at 1000 cents

2.40- no this value takes no parameters. 

2.41- Yes it is a mutator because it sets the price. 

2.42- done

2.43-

2.44- the balance won't change.

2.45- ....

2.46- in the naive ticket machine, the end of the printTicket() method, the total was added with the balance, which was then cleared.

2.47- no, after a ticket has been printed the value in the balance field could not be set to negative. 

2.49- 
Saving = price * discount;  


2.50- 
Mean = total/count;


2.51- 
if (price>budget)
{
System.out.println("Too expensive")
}
Else 
{
System.out.println("Just Right")
}

2.52- 


2.53- the refund balance clears the method. 

2.54- 

2.55- done 

2.56- It is a mutator because it changes the state of the object. 

2.57-