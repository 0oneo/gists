CRUD
===

## Create

```objective-c
#include <stdio.h>
#include <CoreFoudation/CoreFoundation.h>


const int NUMBER_OF_CUSTOMERS = 3;

CFStringRef customers[NUMBER_OF_CUSTOMERS] = {
	CFSTR("Hello"),
	CFSTR("Bar"),
	CFSTR("Foo")
};

CFArrayRef cfCustomers = CFArrayCreate(
	kCFAllocatorDefault, (const void **)customers, NUMBER_OF_CUSTOMERS, &kCFTypeArrayCallBacks
);

CFShow(cfCustomers);

CFRelease(cfCustomers);


````
