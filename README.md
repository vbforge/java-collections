# Java Collections Framework (JCF) Playground

Welcome to the **Java Collections Framework (JCF) Playground** — a curated repository of learning projects, code examples, and reference implementations for mastering the Java Collections Framework. Whether you're preparing for interviews, brushing up on core Java, or building efficient applications, this repo provides a solid foundation.

---

## Projects of this repository:
 - [Custom-Implementation](Custom-Implementations/README.md)
 - [Learning-Collections-Framework](Learning-Collections-Framework/README.md)



---

## 📚 What is the Java Collections Framework?

The **Java Collections Framework** is a unified architecture for storing and manipulating groups of objects. It provides **interfaces**, **implementations**, and **algorithms** to handle data structures efficiently.

JCF is a **core part of the Java Standard Library** (`java.util`) and was introduced in Java 2 (JDK 1.2).

---

## 🧠 Core Concepts

### 🔹 Interfaces

JCF defines a set of core interfaces, which are the **foundation of collections**:

- `Collection<E>` – The root interface for all collections. 
- `List<E>` – An ordered collection (e.g., `ArrayList`, `LinkedList`).
- `Set<E>` – A collection that does not allow duplicate elements (e.g., `HashSet`, `TreeSet`).
- `SortedSet<E>` / `NavigableSet<E>` – Sorted set variants (e.g., `TreeSet`).
- `Queue<E>` / `Deque<E>` – Used for holding elements prior to processing (e.g., `LinkedList`, `ArrayDeque`).
- `Map<K, V>` – A mapping between keys and values (e.g., `HashMap`, `TreeMap`, `LinkedHashMap`).
- `SortedMap<K, V>` / `NavigableMap<K, V>` – Sorted key-value pairs (e.g., `TreeMap`).

### 🔹 Implementations

Each interface has multiple **concrete classes** optimized for specific needs:

| Interface | Implementation Examples     |
|-----------|-----------------------------|
| List      | `ArrayList`, `LinkedList`   |
| Set       | `HashSet`, `LinkedHashSet`, `TreeSet` |
| Queue     | `PriorityQueue`, `ArrayDeque` |
| Map       | `HashMap`, `TreeMap`, `LinkedHashMap`, `Hashtable` |

### 🔹 Utility Classes

- `Collections` – A utility class with static methods for sorting, searching, synchronization, etc.
- `Arrays` – Similar utilities for arrays.

---

## ⚙️ Why Use the Java Collections Framework?

- ✅ **Standardization** – One consistent API across implementations.
- ✅ **Efficiency** – Built-in algorithms like sorting, searching, shuffling.
- ✅ **Flexibility** – Replace one implementation with another easily.
- ✅ **Thread Safety** – Utilities for synchronized collections.
- ✅ **Rich API** – Offers powerful iteration patterns and functional programming support (e.g., with `Stream` API in Java 8+).

---

## 🌳 Collections Hierarchy

Below is a high-level view of the Java Collections Framework hierarchy, showing the relationships between interfaces and their key implementations:

```
java.util.Collection (Interface)
├── List (Interface)
│   ├── ArrayList
│   ├── LinkedList
│   └── Vector
│       └── Stack
│
├── Set (Interface)
│   ├── HashSet
│   │   └── LinkedHashSet
│   └── TreeSet (implements NavigableSet)
│
├── Queue (Interface)
│   ├── PriorityQueue
│   └── LinkedList
│
└── Deque (Interface)
    ├── ArrayDeque
    └── LinkedList

java.util.Map (Interface)
├── HashMap
│   └── LinkedHashMap
├── TreeMap (implements NavigableMap)
└── Hashtable
    └── Properties
```

### 📝 Notes:
- `Collection` is the root interface for all major collections except maps.
- `Map` is a separate hierarchy and does not extend `Collection`.
- Legacy classes like `Vector`, `Stack`, and `Hashtable` are synchronized but generally superseded by modern alternatives.
- `NavigableSet` and `NavigableMap` offer useful navigation methods (`lower()`, `higher()`, etc.).

---





