# JavaSE-Lists

See the Udemy course: https://www.udemy.com/course/curso-certificacion-profesional-desarrollador-java-se-11

![image](https://github.com/luiscoco/JavaSE-30.Lists/assets/32194879/f1a1c53e-c616-4da8-b508-121108487d0f)

Let's talk about ArrayList, Vector, and LinkedList in Java.

## 1. ArrayList:

ArrayList is a part of the Java Collections Framework and is implemented in the java.util package.

It's a resizable array that can dynamically grow or shrink in size.

It provides fast random access to elements, making it efficient for retrieving elements by index.

```java
import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        // Creating an ArrayList
        ArrayList<String> arrayList = new ArrayList<>();

        // Adding elements
        arrayList.add("Apple");
        arrayList.add("Banana");
        arrayList.add("Orange");

        // Accessing elements
        System.out.println(arrayList.get(1)); // Output: Banana
    }
}
```

## 2. Vector:

Vector is also a part of the Java Collections Framework and is similar to ArrayList.

It's synchronized, which means it's thread-safe. This can be an advantage in multithreaded environments, but it might introduce some performance overhead.

```java
import java.util.Vector;

public class VectorExample {
    public static void main(String[] args) {
        // Creating a Vector
        Vector<String> vector = new Vector<>();

        // Adding elements
        vector.add("Red");
        vector.add("Green");
        vector.add("Blue");

        // Accessing elements
        System.out.println(vector.get(2)); // Output: Blue
    }
}
```

## 3. LinkedList

LinkedList is another implementation of the List interface, and it's based on a doubly-linked list data structure.

It provides efficient insertion and deletion of elements, especially in the middle of the list, but it may not be as efficient for random access.

```java
import java.util.LinkedList;

public class LinkedListExample {
    public static void main(String[] args) {
        // Creating a LinkedList
        LinkedList<String> linkedList = new LinkedList<>();

        // Adding elements
        linkedList.add("Cat");
        linkedList.add("Dog");
        linkedList.add("Fish");

        // Accessing elements
        System.out.println(linkedList.get(1)); // Output: Dog
    }
}
```

Each of these data structures has its use cases, and the choice between them depends on the specific requirements of your program. 

If you need fast random access, ArrayList is a good choice. If you need synchronization, Vector might be suitable. 

If you require efficient insertion and deletion, especially in the middle of the list, LinkedList is worth considering.
