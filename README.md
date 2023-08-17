## Given a List<List<Integer>> list that has only 2 columns. Write a sort which first sorts on first column then on second column
```
Collections.sort(list, (x,y)->{
    if(x.get(0) == y.get(0)){
      return Integer.compare(x.get(1), y.get(1));
    }
    return Integer.compare(x.get(0), y.get(0));
  }
)
```
The trick is use `Integer.compare`, `Long.compare` or `String.compare` to compare instead of using manual 1, -1, and 0.

## Can we declare Array of ArrayList in java?
Yes. But there will be a warning of unchecked conversion for below piece of code.
`ArrayList<Integer>[] arr = new ArrayList[];`
Therefore it is recommended to have ArrayList of ArrayList.
