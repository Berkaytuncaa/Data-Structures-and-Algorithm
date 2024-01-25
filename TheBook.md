## Stacks

![](stack.png)

- stack is a LIFO data structure. Last-in First-out.
- stores objects into a sort of "vertical tower"
- `push()`
    - to add to the top
- `pop()`
    - to remove from the top
- `peek()`
    - to look at the object on top
- `search(obj)`
    - to look at the index of the object (index starts at 1, top obj is 1)
- can out of memory

``` java
Stack<String> stack = new Stack<>();
        stack.push("Rdr2");
        stack.push("Skyrim");
        stack.push("Witcher 3");
        stack.push("Gta 6");

        stack.pop(); // this will pop Gta 6

        // Searching for an element
        int position = stack.search("Skyrim");
        
        if(position == -1)
            System.out.println("Element not found");
        else
            System.out.println("Element is found at position: " + position);

        System.out.println("Top element is: " + stack.peek());
```

## Queues

![](QUeue-Data-Structures.png)

- queue is a FIFO data structure. First-in First-out.
- a collection designed for holding elements prior to processing
- linear data structure
- `offer()`
    - to add, enqueue
- `poll()`
    - to remove, dequeue
- `peek()`
    - to look at the head object

``` java
Queue<String> queue = new LinkedList<>();

        // Using offer() to add elements to the queue
        queue.offer("Rdr2");
        queue.offer("Skyrim");
        queue.offer("Witcher 3");
        queue.offer("Gta 6");

        // Using peek() to look at the head of the queue
        System.out.println("Head element is: " + queue.peek());

        // Using poll() to remove the head of the queue
        System.out.println("Removed element is: " + queue.poll());

        // Using peek() to look at the head of the queue after removal
        System.out.println("Head element after removal is: " + queue.peek());
```

## Priority Queues

- a FIFO data structure that serves elements with the heighest priorities first, before elements with lower priorities
- If the parameter of the priority queue is number, by default sorts it in ascending order
- If it is a String, by default sorts it in alphabetical order

``` java
 PriorityQueue<String> queue = new PriorityQueue<>();

        // Using add() to add elements to the queue
        queue.add("Rdr2");
        queue.add("Skyrim");
        queue.add("Witcher 3");
        queue.add("Gta 6");

        // Using peek() to look at the head of the queue
        System.out.println("Head element is: " + queue.peek());

        // Using poll() to remove the head of the queue
        System.out.println("Removed element is: " + queue.poll());

        // Using peek() to look at the head of the queue after removal
        System.out.println("Head element after removal is: " + queue.peek());
```

## LinkedLists

