# DSA-Big-O

This will be exercises to determine the Big-O complexity of algorithms.

## Even or odd

```
 function isEven(value) {
    if (value % 2 === 0) {
        return true;
    }
    else
        return false;
    }
}
```

This is an O(1) complexity algorithm because any size 'value' input will only trigger one
operation of the function.

## Are you here?

```
function areYouHere(arr1, arr2) {
    for (let i = 0; i < arr1.length; i++) {
        const el1 = arr1[i];
        for (let j = 0; j < arr2.length; j++) {
            const el2 = arr2[j];
            if (el1 === el2) return true;
        }
    }
    return false;
}
```

This is an O(n^2) algorithm because it runs two loops using the inputs, so with even a slightly
larger input, the amount of operations required would increase greatly.

## Doubler

```
function doubleArrayValues(array) {
    for (let i = 0; i < array.length; i++) {
        array[i] *= 2;
    }
    return array;
}
```

This is an O(n) algorithm, because as you increase the size of the array, you directly increase
the amount of operations the loop must perform.

## Naive search

```
function naiveSearch(array, item) {
    for (let i = 0; i < array.length; i++) {
        if (array[i] === item) {
            return i;
        }
    }
}
```

This is an O(n) algorithm, in the same way as the previous algorithm, depending on the array
size, the amount of operations the loop performs will be directly increased.
