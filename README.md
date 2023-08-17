# Give a List<List<Integer>> list that has only 2 columns. Write a sort which first sorts on first column then on second column
```
Collections.sort(list, (x,y)->{
    if(x.get(0) == y.get(0)){
      return Integer.compareTo(x.get(1), y.get(1));
    }
    return Integer.compareTo(x.get(0), y.get(0));
  }
)
```
