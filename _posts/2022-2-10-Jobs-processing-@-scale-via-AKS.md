---
layout: post
title:  Jobs processing @ scale via AKS
categories: [AKS,K8S, Azure]
---

![This is an image](https://rafay.co/wp-content/uploads/2019/11/k8saks1-1.jpg)

A Job creates one or more Pods and will continue to retry execution of the Pods until a specified number of them successfully terminate. As pods successfully complete, the Job tracks the successful completions. When a specified number of successful completions is reached, the task (ie, Job) is complete. Deleting a Job will clean up the Pods it created. Suspending a Job will delete its active Pods until the Job is resumed again.

A simple case is to create one Job object in order to reliably run one Pod to completion. The Job object will start a new Pod if the first Pod fails or is deleted (for example due to a node hardware failure or a node reboot).

You can also use a Job to run multiple Pods in parallel.

This is a raw snippet:

```
hello world
123
This is a text snippet
```

This is a PHP snippet:

```php
<?php
    echo 'Hello, World!';
?>
```

This is a JavaScript snippet:

```js
const add = (a, b) => a + b
const minus = (a, b) => a - b

console.log(add(100,200))  // 300
console.log(minus(100,200))  // -100
```

This is a Python snippet:

```python
def say_hello():
    print("hello world!")

say_hello()   // "hello world!"
```
