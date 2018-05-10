---
description: OS review
---

# Process Synchronization

恐龍書第五章

* preemptive kernel
* nonpreemptive kernel



*  critical section
  * Mutual Exclsive
  * Progress
  * Boundary

{% code-tabs %}
{% code-tabs-item title="critical section" %}
```c
do{
    // entry section
    // critical section
    // remainder section
} while(true)
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## synchronization with preemptive kernel

{% code-tabs %}
{% code-tabs-item title="peterson\'s solution" %}
```c
do{
    flag[i] = true;
    turn = j;/ 禮讓
    while(flag[j]&&trun==j);
        
```
{% endcode-tabs-item %}
{% endcode-tabs %}

