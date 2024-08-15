# Some-topic-related-to-DSA-

DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DSA Essentials</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Orbitron:wght@700&display=swap" rel="stylesheet">
</head>
<body>
    <div id="lunaglow-lightning"></div>
    <div class="lunaglow-container">
        <h1>DSA Essentials</h1>
        
        <div class="lunaglow-intro">
            <p>Ready to <span class="lunaglow-highlight">supercharge your coding skills</span>? Dive into these 7 game-changing DSA concepts! They're the secret sauce behind <span class="lunaglow-highlight">efficient algorithms</span> and will <span class="lunaglow-highlight">skyrocket your problem-solving abilities</span>. Let's unlock the power of DSA together!</p>
        </div>

        <div class="lunaglow-topic">
            <h2>1. Arrays</h2>
            <p>Arrays are the <span class="lunaglow-highlight">backbone of data storage</span>. They offer lightning-fast access to elements but can be tricky for insertions and deletions. Master arrays, and you'll have a solid foundation for more complex data structures.</p>
            <div class="lunaglow-code">
let fruits = ["apple", "banana", "orange"];
console.log(fruits[1]); // Output: banana
            </div>
            <div class="lunaglow-problem">Problem: Find the largest number in an array.</div>
            <button class="lunaglow-btn" onclick="lunaglowToggleAnswer(this)">Reveal Solution</button>
            <div class="lunaglow-answer">
let numbers = [5, 2, 8, 1, 9];
let largest = Math.max(...numbers);
console.log(largest); // Output: 9
            </div>
        </div>

        <div class="lunaglow-topic">
            <h2>2. Linked Lists</h2>
            <p>Linked lists are the <span class="lunaglow-highlight">flexible cousins of arrays</span>. They excel at insertions and deletions but require some effort for access. Understanding linked lists opens doors to more advanced data structures.</p>
            <div class="lunaglow-code">
class Node {
    constructor(data) {
        this.data = data;
        this.next = null;
    }
}
            </div>
            <div class="lunaglow-problem">Problem: Create a simple linked list with 3 nodes.</div>
            <button class="lunaglow-btn" onclick="lunaglowToggleAnswer(this)">Reveal Solution</button>
            <div class="lunaglow-answer">
let head = new Node(1);
head.next = new Node(2);
head.next.next = new Node(3);
            </div>
        </div>

        <div class="lunaglow-topic">
            <h2>3. Stacks</h2>
            <p>Stacks follow the <span class="lunaglow-highlight">Last-In-First-Out (LIFO) principle</span>. They're crucial for function calls, undo mechanisms, and parsing expressions. Master stacks to tackle recursive problems with ease.</p>
            <div class="lunaglow-code">
let stack = [];
stack.push(1);
stack.push(2);
console.log(stack.pop()); // Output: 2
            </div>
            <div class="lunaglow-problem">Problem: Check if brackets are balanced.</div>
            <button class="lunaglow-btn" onclick="lunaglowToggleAnswer(this)">Reveal Solution</button>
            <div class="lunaglow-answer">
function isBalanced(str) {
    let stack = [];
    for (let char of str) {
        if (char === '(') stack.push(char);
        else if (char === ')') {
            if (stack.length === 0) return false;
            stack.pop();
        }
    }
    return stack.length === 0;
}
console.log(isBalanced("(())")); // Output: true
            </div>
        </div>

        <div class="lunaglow-topic">
            <h2>4. Queues</h2>
            <p>Queues operate on the <span class="lunaglow-highlight">First-In-First-Out (FIFO) principle</span>. They're perfect for managing tasks, handling requests, and implementing breadth-first search algorithms. Queue up your skills for real-world applications!</p>
            <div class="lunaglow-code">
let queue = [];
queue.push(1);
queue.push(2);
console.log(queue.shift()); // Output: 1
            </div>
            <div class="lunaglow-problem">Problem: Print first 5 numbers in order.</div>
            <button class="lunaglow-btn" onclick="lunaglowToggleAnswer(this)">Reveal Solution</button>
            <div class="lunaglow-answer">
let queue = [1, 2, 3, 4, 5];
while (queue.length > 0) {
    console.log(queue.shift());
}
            </div>
        </div>

        <div class="lunaglow-topic">
            <h2>5. Trees</h2>
            <p>Trees are <span class="lunaglow-highlight">hierarchical structures</span> that branch out from a root. They're essential for representing relationships, optimizing searches, and solving complex problems. Plant this knowledge for a flourishing coding career!</p>
            <div class="lunaglow-code">
class TreeNode {
    constructor(value) {
        this.value = value;
        this.left = null;
        this.right = null;
    }
}
            </div>
            <div class="lunaglow-problem">Problem: Create a simple binary tree.</div>
            <button class="lunaglow-btn" onclick="lunaglowToggleAnswer(this)">Reveal Solution</button>
            <div class="lunaglow-answer">
let root = new TreeNode(1);
root.left = new TreeNode(2);
root.right = new TreeNode(3);
            </div>
        </div>

        <div class="lunaglow-topic">
            <h2>6. Sorting</h2>
            <p>Sorting algorithms bring <span class="lunaglow-highlight">order to chaos</span>. From simple bubble sort to lightning-fast quicksort, these techniques are crucial for efficient data manipulation. Sort out your understanding to optimize your code!</p>
            <div class="lunaglow-code">
let numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5];
numbers.sort((a, b) => a - b);
console.log(numbers);
            </div>
            <div class="lunaglow-problem">Problem: Implement bubble sort.</div>
            <button class="lunaglow-btn" onclick="lunaglowToggleAnswer(this)">Reveal Solution</button>
            <div class="lunaglow-answer">
function bubbleSort(arr) {
    for (let i = 0; i < arr.length; i++) {
        for (let j = 0; j < arr.length - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]];
            }
        }
    }
    return arr;
}
            </div>
        </div>

        <div class="lunaglow-topic">
            <h2>7. Searching</h2>
            <p>Searching algorithms are your <span class="lunaglow-highlight">data detectives</span>. From simple linear search to the efficient binary search, these techniques are key to finding information quickly. Sharpen your searching skills to tackle complex problems!</p>
            <div class="lunaglow-code">
let numbers = [1, 3, 5, 7, 9];
console.log(numbers.indexOf(5)); // Output: 2
            </div>
            <div class="lunaglow-problem">Problem: Implement binary search.</div>
            <button class="lunaglow-btn" onclick="lunaglowToggleAnswer(this)">Reveal Solution</button>
            <div class="lunaglow-answer">
function binarySearch(arr, target) {
    let left = 0, right = arr.length - 1;
    while (left <= right) {
        let mid = Math.floor((left + right) / 2);
        if (arr[mid] === target) return mid;
        if (arr[mid] < target) left = mid + 1;
        else right = mid - 1;
    }
    return -1;
}
            </div>
        </div>

        <div class="lunaglow-topic">
            <h2>Check Your First Job Salary</h2>
            <p>Want to see what your first job might pay? Click the button to find out!</p>
            <button class="lunaglow-btn" onclick="lunaglowCheckSalary()">Check Salary</button>
            <div id="lunaglow-salary-result" class="lunaglow-answer" style="display: none;"></div>
        </div>
    </div>

    <footer class="lunaglow-footer">
        <p>&copy; 2024 DSA Essentials. All rights reserved.</p>
    </footer>

  
</body>
</html>
