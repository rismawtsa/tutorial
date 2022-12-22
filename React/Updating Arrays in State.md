# Updating Arrays in State

In React, keep the arrays in state as read-only. This means that we shouldn't

- reassign the itemn is an array like `a[0] = 'test'`.
- use methods that mutate the array, such as `push()`, `slice()`, `pop()`, etc.

## Sorting or Reverse

The [sort()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort) and [reverse()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse) methods mutate the array. If we want to sort/reverse the array in the state, make a copy of the array first, and then make changes to it.

```
const [list, setList] = useState([
    {
        title: "Javascript",
        votes: 4
    },
    {
        title: "Java",
        votes: 2
    }
])

function handleClick() {
    const nextList = [...list];
    nextList.sort(());
    setList(nextList);
}
```
