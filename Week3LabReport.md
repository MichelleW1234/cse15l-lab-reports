# Part 1:
## Code:

![code1](https://user-images.githubusercontent.com/122498397/215352492-ebf3ec93-878b-4fb9-b039-fde7fcf3302e.jpg)
![code2](https://user-images.githubusercontent.com/122498397/215352594-d8fe2be7-2425-4ae5-9284-ff76c5a15de6.jpg)

![code3](https://user-images.githubusercontent.com/122498397/215352600-42485359-22dd-43b9-98ba-3142bb9cd379.jpg)
![code4](https://user-images.githubusercontent.com/122498397/215352604-3c9ad3e0-33db-40d4-ad22-315bb0d60a1c.jpg)

## Results from using `/add-message`:

### `Hello`:

![image1](https://user-images.githubusercontent.com/122498397/215352624-de3e78cb-3705-413b-a60a-0696d54dd5d0.jpg)

To come up with the result above, all of the methods from both `StringServer.java`, the file that contains both main() and handleRequest() (the method that ultimately figures out what to do with the `/add-message` request in the path), and `theServer.java`, the black box file, are called, as they all call eachother in order to print out the resulting link to the page in the terminal. There are also methods from Java's built in classes, such as the `HttpServer` class, that are called in `theServer.java`. 

In `StringServer.java`, there are two classes, `StringServer` and `Handler`, which both contain methods with relevant arguments. There are two relevant arguments in `main()` from the `StringServer` class. One is `4000` (the port number) that is strung at the end of the command to run the file, which becomes the `main` method's `args[0]` and also the value that is referenced by `int port` that becomes an argument when `main()` calls `start()` from `theServer.java`. The second relevant argument in `main()` is a new object `new Handler()` from the `Handler` class in `theServer.java` that is the second argument for `start()` when it is called. In `handleRequest()` in the `Handler` class, there are six relevant arguments. The first one is 'url', an object from the 'URI' class that contains the URL to the resulting page in the photo and is what the body of the method will be processing. The second one is the `String "/add-message"`, the argument of `contains()` in the outer if-statement condition `url.getPath().contains()`, which checks for whether or not the path in `url` contains that `String`. This specific `String` is very important, as it is the request that determines whether or not there is a specified message in the query of `url` that will be printed. The third argument is the `String "="` in the `split()` method in `url.getQuery().split()`, which determines where the query of `url` will be split and becomes two elements in the 'String' array, `parameters`. The fourth and fifth arguments are in `parameters[0].equals("s")`, a condition in the nested if-statement. The index `0` in `parameters[0]` references the first element of `parameters`, while the `String "s"` is what that element will be checked for. The final relevant arguemnt is the index `1` in `parameters[1]`, which is what is returned from `handleRequest()`, and is also what should be printed in the page that the resulting link that is outputted in the terminal leads to if everything that `handleRequest()` checks for (`/add-message?s=`) is added to the end of the link. 

To get the desired result (having the message after the `=` link to be printed), every condition must be met in `handleRequest()`, which is why every field and argument of `handleRequest()` from the `Handler` class is relevant. Without them, although a link will still be outputted in the terminal that leads to a page, the computer will not know to print the message after `/add-message?s=`, which is what we want it to do, therefore, for this type of request, nothing should be changed. However, for this *specific* request (having `hello` be printed on the page), the relevant argument with the value that should be changed is `url`--- specifically the part after the `"="` in `url`, as that is what becomes the second element of `parameter` and is returned to let the computer know that that is what should be printed.

### `How are you`:

![image2](https://user-images.githubusercontent.com/122498397/215352628-da07622d-18df-4b3c-8876-9bb3c8bef221.jpg)

To come up with the result above, all of the methods from both `StringServer.java`, the file that contains both main() and handleRequest() (the method that ultimately figures out what to do with the `/add-message` request in the path), and `theServer.java`, the black box file, are called, as they all call eachother in order to print out the resulting link to the page in the terminal. There are also methods from Java's built in classes, such as the `HttpServer` class, that are called in `theServer.java`. 

In `StringServer.java`, there are two classes, `StringServer` and `Handler`, which both contain methods with relevant arguments. There are two relevant arguments in `main()` from the `StringServer` class. One is `4000` (the port number) that is strung at the end of the command to run the file, which becomes the `main` method's `args[0]` and also the value that is referenced by `int port` that becomes an argument when `main()` calls `start()` from `theServer.java`. The second relevant argument in `main()` is a new object `new Handler()` from the `Handler` class in `theServer.java` that is the second argument for `start()` when it is called. In `handleRequest()` in the `Handler` class, there are six relevant arguments. The first one is 'url', an object from the 'URI' class that contains the URL to the resulting page in the photo and is what the body of the method will be processing. The second one is the `String "/add-message"`, the argument of `contains()` in the outer if-statement condition `url.getPath().contains()`, which checks for whether or not the path in `url` contains that `String`. This specific `String` is very important, as it is the request that determines whether or not there is a specified message in the query of `url` that will be printed. The third argument is the `String "="` in the `split()` method in `url.getQuery().split()`, which determines where the query of `url` will be split and becomes two elements in the 'String' array, `parameters`. The fourth and fifth arguments are in `parameters[0].equals("s")`, a condition in the nested if-statement. The index `0` in `parameters[0]` references the first element of `parameters`, while the `String "s"` is what that element will be checked for. The final relevant arguemnt is the index `1` in `parameters[1]`, which is what is returned from `handleRequest()`, and is also what should be printed in the page that the resulting link that is outputted in the terminal leads to if everything that `handleRequest()` checks for (`/add-message?s=`) is added to the end of the link. 

To get the desired result (having the message after the `=` link to be printed), every condition must be met in `handleRequest()`, which is why every field and argument of `handleRequest()` from the `Handler` class is relevant. Without them, although a link will still be outputted in the terminal that leads to a page, the computer will not know to print the message after `/add-message?s=`, which is what we want it to do, therefore, for this type of request, nothing should be changed. However, for this *specific* request (having `How are you` be printed on the page), the relevant argument with the value that should be changed is `url`--- specifically the part after the `"="` in `url`, as that is what becomes the second element of `parameter` and is returned to let the computer know that that is what should be printed.

# Part 2:

/**
-A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)
-An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)
-The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)
-The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)
-Briefly describe why the fix addresses the issue.
**/

## A buggy program in ArrayExamples.java:

![Image 1-29-23 at 2 06 PM](https://user-images.githubusercontent.com/122498397/215358237-a0961448-64cd-4df9-9030-5e7c51e43a2f.jpg)

## A failure-inducing input:

# code block
int[] input2 = {3, 5, 10, 15, 20};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{20, 15, 10, 5, 3}, input2);

## An input that doesn’t induce a failure:

# code block
int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);

## The symptom:

??????

## The bug:

### Before:

# code block
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
}

### After:

# code block
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int originalElement = arr[i];
      arr[i] = arr[arr.length - i - 1];
      arr[arr.length - i - 1] = originalElement;
    }
}

After finding out that the method was trying to go through the array and switching the elements from both ends of the array until it got to the center, I realized that, while the first element was being changed to the last element, the last element wasn’t being changed to the first element. Therefore, I had to write the code inside of the for loop that would save the  element at i (the first element), and then, after the first element was changed, would change the last element to the first element as well. I also had to divide arr.length by 2, since, if the switching is supposed to stop when it reaches the middle of the array, this means that the number of iterations would only be half of the length of the list rather than the entire length. 

# Part 3:

In this past week, I learned a lot about debugging. Although I've obviously had to start learning to debug ever since I started coding, I never knew about the tests that I could myself to check different methods in a file. 

































