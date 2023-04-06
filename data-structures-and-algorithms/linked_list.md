# Linked List Cheatsheet

## Overview

- A linked list is a linear data structure in which elements are stored in nodes
- Each node contains a value and a pointer to the next node in the list
- The first node is called the head and the last node is called the tail
- Linked lists can be singly or doubly linked

## Operations

### Insertion

#### Insertion at the Head

```python
# create a new node
new_node = Node(value)

# point new node to the current head
new_node.next = head

# make new node the new head
head = new_node
```

#### Insertion at the Tail

```python
# create a new node
new_node = Node(value)

# point the current tail to the new node
tail.next = new_node

# make the new node the new tail
tail = new_node
```

### Deletion

#### Deletion at the Head

```python
# point the head to the next node
head = head.next
```

#### Deletion at the Tail

```python
# traverse the list until the node before the tail
current_node = head
while current_node.next != tail:
  current_node = current_node.next

# point the current tail to None
current_node.next = None

# make the node before the current tail the new tail
tail = current_node
```

### Traversal

```python
current_node = head
while current_node is not None:
  # do something with current_node.value
  current_node = current_node.next
```

## Time Complexity

- Insertion and deletion at the head: O(1)
- Insertion and deletion at the tail: O(n)
- Traversal: O(n)

## Resources

- [GeeksforGeeks: Linked List](https://www.geeksforgeeks.org/data-structures/linked-list/)
- [Linked List Wikipedia](https://en.wikipedia.org/wiki/Linked_list)