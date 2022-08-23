# CSS Cheat Sheet

### * (Universal Selector) selects all the element 
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

### div (Type selector) selects elements of the same type
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