# CSS Selectors Explained

### * (Universal Selector) selects all the elements 
```css
    *{
        background-color:blue;


    }
```
```mermaid
    graph TD
        A:::select
        B:::select
        C:::select
        D:::select
        classDef select fill:#1919a6

```

***

### div (Type selector) selects all elements of the same type
```css
    div{
        background-color:blue;

    }
```
```mermaid
    graph TD
    A(div):::select;
    B(span );
    C(div):::select;
    D(span);

    classDef select fill:#1919a6;

```

***

### .class-name (class selector) selects all elements having the same class attribute
```css
    .box{

    }

```
```mermaid
    graph TD
    A(.box):::select;
    B(.box):::select;
    C(.circle)
    D(.triangle);

    classDef select fill:#1919a6;
```


