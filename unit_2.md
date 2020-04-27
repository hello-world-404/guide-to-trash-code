[Go back to home page](README.md)
## Unit 2
The basics of trash code: long and unwinded code that does nothing.

### Long and unwinded code
In order for you to write beautiful trash code, you must write long and unwinded code that does nothing. You might ask, what is meant by
long and unwinded code? The answer for is clear and easy: long code that usually can be replaced by other the call of a method or a class, and by
writing duplicate segments of them makes your code harder to understand and more trash!

### Writing long and unwinding code.
Here are some tips to help you write long and unwinded and unnecessary code that can be replaced by more efficient solutions.

1. Try to not use the call of any methods or classes or any shortcuts, as they can destroy trash code.  
2. If you must need a call of a method or any class, try writing the method in the code, that will make your code even longer and does the same thing
as the method. Then after you write your unwinded code, **do not use it** and call the method that can be replaced by that long code.
3. If you are writing an if statement, write to check one condition in all of the branches. For example:

**DO THIS**
```
/* The below example is a part of a password generation program.
* The pwGen method generates a password like this: chs.0293
* The chs part is the prefix. . is the . 0293 is the randomly generated
* 4 digit number.
* @ author: One-Kingyo
*/
public String pwGen(){
        password = prefix + ".";
        password += Integer.toString((int)(Math.random() * ((9 - 0)) + 1) + 0);

        for(int i = 0; i < length; i++){
            password += Integer.toString((int)(Math.random() * ((9 - 0)) + 1) + 0);
        }
        count++;
        return password;
}
```
**DON'T DO THIS**
```
/* The below example is a part of a password generation program.
* The pwGen method generates a password like this: chs.0293
* The chs part is the prefix. . is the . 0293 is the randomly generated
* 4 digit number.
* @ author: One-Kingyo
*/
public String pwGen(){
        password = prefix + ".";
        password += (int)(Math.random() * ((9 - 0)) + 1) + 0;

        for(int i = 0; i < length; i++){
            password += Integer.toString((int)(Math.random() * ((9 - 0)) + 1) + 0);
        }
        count++;
        return password;
}
```

In the above example, the long code is written to be:
```
password += Integer.toString((int)(Math.random() * ((9 - 0)) + 1) + 0);
```
while the short code is written to be:
```
password += (int)(Math.random() * ((9 - 0)) + 1) + 0;
```
The two solutions basically does the same thing, generating a number between 0 - 9
and adding them to the variable password. But notice that the first code segment is
slightly longer, but it does the same thing. That's long and unwinded code.

Here's another example:
```
/* The below code segment is part from a cruise price calculation program.
* The code segment calculates the total revenue made from the cruise trip.
* The variable signup represents the total number of people who signed up
* for the cruise. If the number of signups is smaller than 200, then the price
* is the same. If the number of signups is bigger than 200 and smaller than 300,
* then everybody gets a discount of 350. If the number of signups is bigger than 300
* then everybody gets a discount of 500
* @author: One-Kingyo
*/

```

**DO THIS**
```

public int calculateRevenue(){
        if(signup < 200){
            return signup * price;
        }
        else if(signup >= 200 & signup < 300){
            return (signup * price) - (signup * 350);
        }
        else{
            return (signup * price) - (signup * 500);
        }
}
```

**DON'T DO THIS**
```
public int calculateRevenue(){
       if(signup < 200){
           return signup * price;
       }
       else if(signup < 300){
           return signup * (price - 350);
       }
       else{
           return signup * (price - 500);
       }
   }
```

In the above example, there are two parts of long and unwinded code. We
will introduce the first part first.

The long if statement is written to be:
```
if(signup < 200){

}
else if(signup >= 200 & signup < 300){

}
else{

}
```
while the short code is written to be:
```
if(signup < 200){

}
else if(signup < 300){

}
else{

}
```
Notice the if statement header of the else-if branch. The long code checks
the first condition again, while the short code does not. This is a excellent
example of long and unwinded code that can be replaced by something else.

Another example in the above code is these two lines.

The long way to write the total price of signups is:
```
  return (signup * price) - (signup * 350);
  return (signup * price) - (signup * 500);

```

The short way to write the total price of signups is:
```
 return signup * (price - 350);
 return signup * (price - 500);
```

Again, like the above example, both code segments do the same thing, but the first method is longer and more complicated than the shorter method. Which is trash code. 
