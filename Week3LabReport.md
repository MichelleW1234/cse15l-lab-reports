# Part 1:
## Code:

![code1](https://user-images.githubusercontent.com/122498397/215352492-ebf3ec93-878b-4fb9-b039-fde7fcf3302e.jpg)

![code2](https://user-images.githubusercontent.com/122498397/215352594-d8fe2be7-2425-4ae5-9284-ff76c5a15de6.jpg)

![code3](https://user-images.githubusercontent.com/122498397/215352600-42485359-22dd-43b9-98ba-3142bb9cd379.jpg)

![code4](https://user-images.githubusercontent.com/122498397/215352604-3c9ad3e0-33db-40d4-ad22-315bb0d60a1c.jpg)

## Results from using `/add-message`:

![image1](https://user-images.githubusercontent.com/122498397/215352624-de3e78cb-3705-413b-a60a-0696d54dd5d0.jpg)

To come up with this result, all of the methods from both `StringServer.java`, the file that contains both main() and handleRequest() (the method that ultimately figures out what to do with the `/add-message` request in the path), and `theServer.java`, the black box file, are called, as they all call eachother in order to print out the resulting link to the page in the terminal. There are also methods from Java's built in classes, such as the `HttpServer` class, that are called in `theServer.java`. 

In `StringServer.java`, there are two relevant arguments in `main()`. One is the `4000` (the port number) that is strung at the end of the command to run the file, which becomes the `main` method's `args[0]` and also the value that is referenced by `int port` that becomes an argument when `main()` calls `start()` from `theServer.java`. The second relevant argument in `main` is a new object `new Handler()` from the `Handler` class in `theServer.java` that is the second argument for `start()` when it is called. In `handleRequest()` in `StringServer.java`, there are six relevant arguments.  

Which methods in your code are called?
What are the relevant arguments to those methods, and the values of any relevant fields of the class?
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

![image2](https://user-images.githubusercontent.com/122498397/215352628-da07622d-18df-4b3c-8876-9bb3c8bef221.jpg)
