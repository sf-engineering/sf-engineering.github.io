---
title: Salesforce Engineering
layout: default
description: Explore Apex design patterns and best practices.
---

<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
  }
  .container {
    max-width: 800px;
    margin: auto;
    background: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  h1, h2 {
    color: #0070d2;
  }
  pre {
    background: #eee;
    padding: 10px;
    border-radius: 5px;
    overflow-x: auto;
  }
  .comment-section {
    margin-top: 20px;
    padding: 10px;
    background: #f9f9f9;
    border-left: 5px solid #0070d2;
  }
</style>

<div class="container">

# 🚀 Salesforce Engineering

Welcome to the **Salesforce Engineering Hub**! This page is dedicated to sharing **Apex design patterns** and best practices for Salesforce developers. Whether you're a beginner or an expert, these patterns will help you build scalable and maintainable applications.

## 🔥 Apex Design Patterns

Click on any pattern to explore:

- [Singleton Pattern](#singleton-pattern) 🏆
- [Factory Pattern](#factory-pattern) 🏭
- [Strategy Pattern](#strategy-pattern) 🎯
- [Observer Pattern](#observer-pattern) 👀
- [Unit of Work Pattern](#unit-of-work-pattern) 📦

## 🏆 Singleton Pattern

Ensures that a class has only **one instance** and provides a **global access point** to it.

```apex
public class SingletonExample {
    private static SingletonExample instance;
    private SingletonExample() {}
    public static SingletonExample getInstance() {
        if (instance == null) {
            instance = new SingletonExample();
        }
        return instance;
    }
}
```

👉 [Learn more](singleton.md)

## 🏭 Factory Pattern

Encapsulates **object creation logic** to create different instances dynamically.

```apex
public class ShapeFactory {
    public static Shape getShape(String type) {
        if (type == 'Circle') return new Circle();
        if (type == 'Square') return new Square();
        return null;
    }
}
```

👉 [Learn more](factory.md)

## 🚀 Contribute

Want to add more patterns? **Fork this repo** and submit a PR! Contributions are always welcome. 🎉

---

💡 _Follow for more Salesforce engineering content!_

</div>
