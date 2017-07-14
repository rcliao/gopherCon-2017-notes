# Forward Compatible Go code

Breaks due to the programmer:

* Relying on output stability
* Relying on value comparability
    * time.Time
    * errors
    * reflect
* Relying on Go runtime details


How do you write the forward compatible Go code:

* Read the documentation
* Be careful of what you hardcode
* Use the right comparison
* Use the race detector
* Be willing to update unsafe code

