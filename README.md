#Stack program using C++

Stack is a data structure, in which insertion take place at the one and deletion from another end.
In stack data structure first delete the element that is poped at last LIFO (Last In First Out).

First of all you have to include the libraries:
  <iostream> for input and output
  <cstdlib>  we will use this library for clearing the screen.

Then we have to make a structure for our program:
  struct { 
    int arr[10];       // our array lenght is 10.
    int top = -1;      // at first we have to assign the top to -1 because we don't have element in the array, and array starts
                          from 0.
    } stock1;         // From stock1 we can access the body of struct through this we can make changes in the body of struct.

After that we declare push function to insert element to our array:

  void pop(){

    if(stock1.top <0 || stock1.top > 9 ){     // if top is less than 0, then stack is empty, so it will display a message for the
                                                 user
        cout << "Under Flow...!\n";
    }
    else{
        stock1.arr[stock1.top] = NULL;      // if the top is greater than -1 means stack is not empty so the element of the array
                                               will be asssigned to NULL and then the top will decreased by one.
        stock1.top--;
    }
 }
