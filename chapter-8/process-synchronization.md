---
description: OS review
---

# Process Synchronization

66恐龍書第五章

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

* software-based

{% code-tabs %}
{% code-tabs-item title="peterson\'s solution" %}
```c
do{
    flag[i] = true;
    turn = j;/ 禮讓
    while(flag[j]&&trun==j);
    
    // critical section
    flag[i] = false;
    
    // remainder section
} while(true)        
```
{% endcode-tabs-item %}
{% endcode-tabs %}

* single-processor
  * test-and-set

{% code-tabs %}
{% code-tabs-item title="test and set" %}
```c
boolean test_and_set(boolean *target){
    boolean rv = *target;
    *target = true;
    
    return rv;
}
do{
    while(test_and_set(&lock));
    // critical section
    
    lock = flase;
    // remainder section
} while(true);
```
{% endcode-tabs-item %}
{% endcode-tabs %}

