---
description: OS review
---

# Process Synchronization

66恐龍書第五章

* preemptive kernel
* nonpreemptive kernel



*  critical section
  * Mutual Exclusive
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

* hardware-based
  * test\_and\_set\(\)
  * compare\_and\_swap\(\)

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

{% code-tabs %}
{% code-tabs-item title="compare and swap" %}
```c
int compare_and_swap(int *value, int expected, int new_value){
    int temp = *value;
    if(*value == expected)
        *value = new_value;
    
    return temp;
}

do{
    while(compare_and_swap(&lock, 0, 1) != 0)
        ; /* do nothing */
        
        /* critical section*/
    
    lock = 0;
        /*remainder section*/
} while(true);
```
{% endcode-tabs-item %}
{% endcode-tabs %}



