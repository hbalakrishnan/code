# code

The musical_group.tsv has following entries like list of musical items
```
Yearbook Committee	/m/0dykyh3
Scratch Me Scratch	/m/0f403mn
Broadfield Marchers	/m/0dm6vr9
Choo Choo	/m/0dnzqf0
The Bitter Ind	/m/0dykw2b
Indigo	/m/01wj3vq
Indigo Girls & Ani DiFranco	/m/01v5dc3
```

so load this file and try to build an index. It should have search query and upon searching it should return the id associated with that.
The delimiter here is /m/

```
Name of the item: Scratch Me Scratch
id: 0f403mn
```

```
public interface SearchService {
  /**
     if the input here is Indigo, then it should return list of [01wj3vq,01v5dc3]
  */
  public List<String> search(String query);
}
```



