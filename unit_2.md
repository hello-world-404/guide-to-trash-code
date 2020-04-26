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
Look out for this line:
```
password += Integer.toString((int)(Math.random() * ((9 - 0)) + 1) + 0);
```
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
Look out for this line:
```
password += (int)(Math.random() * ((9 - 0)) + 1) + 0;
```
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


### Writing the Code
After you have done the things done above, you are ready to write Trash Code!

**Remember, the first thing writing trash code is to be complicated.**

Let's say that you are writing a program that receives the input as the radius and outputs the perimeter and area.

**ALL CODE SEGMENTS ARE WRITTEN IN JAVA, USE YOUR CLEVER BRAIN TO CHANGE IT TO THE LANGUAGE YOU WRITE, THAT MAKES IT EVEN TRASH. **

1. First thing you have to do is to declare the base class and method of your code.
```
public class Area{
    public static void main(String[] args){

    }
}
```

2. Declare the variables you need with meaningless variable names, or write meaningful variable names and assign them with the wrong values.
```
public class Area{
    public static void main(String[] args){
          Double i =  888.0;
          Double e = 666.0;

          Double radius = 2 * 3.14 *
    }
}
```

3. Write equations for computing the area and perimeter and put set them to other variables.
```
public class Area{
    public static void main(String[] args){
          Double i =  888.0;
          Double e = 666.0;

          Double radius = 2 * 3.14 * i;
          Double perimeter = 3.14 * i * i;
    }
}
```
4. Print random stuff out!
```
public class Area{
    public static void main(String[] args){
          Double i =  888.0;
          Double e = 666.0;

          Double radius = 2 * 3.14 * i;
          Double perimeter = 3.14 * i * i;

          System.out.println(i);
          System.out.println(e);
          System.out.println(i);
          System.out.println(perimeter);
    }
}
```
5. Oh Yeah! What messy code!
