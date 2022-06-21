# Stacks and Queues

Defention of stack: it's a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

## Common terminology for a stack is

1. Push 
2. Pop 
3. Top 
4. Peek 
5. IsEmpty 

Stacks follow these concepts:


## First In Last Out (FILO):


the first item added in the stack will be the last item popped out of the stack.

## Last In First Out (LIFO):

he last item added to the stack will be the first item popped out of the stack.

# Visualization

The topmost item is denoted as the top. When you push something to the stack, it becomes the new top. When you pop something from the stack, you pop the current top and set the next top as top.next

## Push O(1)

Pushing a Node onto a stack will always be an O(1) operation.

## Pop O(1)

When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.


## Peek O(1)

When conducting a peek, you will only be inspecting the top Node of the stack.

Typically, you would check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.


## IsEmpty O(1)



# Queue


## Common terminology for a stack is

1. Enqueue  
2. Dequeue  
3. Front  
4. Rear  
5. Peek 
6. IsEmpty  

## First In First Out (FIFO)

This means that the first item in the queue will be the first item out of the queue.

## Last In Last Out (LILO)

This means that the last item in the queue will be the last item out of the queue.



