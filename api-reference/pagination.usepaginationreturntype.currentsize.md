<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@vue-composition-ui/pagination](./pagination.md) &gt; [UsePaginationReturnType](./pagination.usepaginationreturntype.md) &gt; [currentSize](./pagination.usepaginationreturntype.currentsize.md)

## UsePaginationReturnType.currentSize property

Size of current page

<b>Signature:</b>

```typescript
readonly currentSize: number;
```

## Example 1

If perPageSize is 10, currentPage is 5, and totalSize is 52

```
console.log(currentSize) // 10 (41~50)

```

## Example 2

If perPageSize is 10, currentPage is 6, and totalSize is 52

```
console.log(currentSize) // 2 (51~52)

```

