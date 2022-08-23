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
        background-color:blue;


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

***

### #unique-id (ID selector) selects element having the same id attribute 
```css
    #A{
        background-color:blue;


    }
```
```mermaid
    graph TD
    #A
    #B
    #C
    #D
    style #A fill:#1919a6;
```

***

# Combinations

#### CSS selectors can be used in various combination to select desired element/s

### div p (Descendant slector) slelects all descendant(p) element of the parent(div)

```css
    div p{
        background-color:blue;


    }
```
```mermaid
    graph TD
    A(div)-->B(p):::select
    A --> C(div) -->F(p):::select
    A --> D(btn)
    B --> E(p):::select

    classDef select fill:#1919a6;
```

***

### div > p (Direct child selector) selects the 1st generation descendants

```css
    div > p{
        background-color:blue;


    }
```
```mermaid
    graph TD
    A(div)-->B(p):::select
    A --> C(div) -->F(p)
    A --> D(btn)
    B --> E(p)

    classDef select fill:#1919a6;

```

***

### div ~ p (General sibling slector) slects elements (p) next to (div) of same generation

```css
    div ~ p{
        background-color:blue;
        
        
    }
```
```mermaid
   graph TD
    A(p) 
    B(div)
    C(p):::select
    D(a)
    E(p):::select


    classDef select fill:#1919a6;
```

***

### div + p (adjacent sibling selector) selects element (p) immediate next to (div) element

```css
    div + p{
        background-color:blue;


    }
```
```mermaid
    graph TD
    A(p) 
    B(div)
    C(p):::select
    D(a)
    E(p)


    classDef select fill:#1919a6;
```

***

### a, div (Or slector) selects all elements in the list

```css
    a, div{
        background-color:blue;


    }
```
```mermaid
    graph TD
    A(a):::select
    B(div):::select
    D(a):::select
    E(p)


    classDef select fill:#1919a6;
```

***

### a.class-name (And selctor) selects the matching combination
```html
<html>
    <style>
        a.a-color{
            color:red;
        }
        

    </style>

    <!-- Display in red -->
    <a class="a-color" href="">I'm Gokul</a> 
    <!-- No change -->
    <p class="p-color">I'm Gokul
</html>
```
```mermaid
    graph TD
    A(a.class-name):::select
    B(p.class-name)


    classDef select fill:#1919a6;

```

***

# Pseudo Class 

### p:first-child (First child selector) selects the element if it's the first child

```css
    p:first-child{
        background-color:blue;


    }
```
```mermaid
    graph TD
    A(div)-->B(p):::select
    A(div)-->C(p)
    A(div)-->D(p)
    A(div)-->E(p)

    E(div)--->F(a)
    E(div)--->G(p)
    E(div)--->I(p)
    classDef select fill:#1919a6;
```

***

### p:last-child (Last child selector) selects the element if it's the last child

```css
    p:last-child{
        background-color:blue;


    }
```
```mermaid
    graph TD
   A(div)-->B(a)
   A(div)-->C(a)
   A(div)-->D(p):::select

   E(div)--->F(p)
   E(div)--->G(p)
   E(div)--->I(a)

   classDef select fill:#1919a6;

```










