## 07_40 CSS Variables

CSS variables make it easier to maintain consistency across a website.

CSS variables may be declared with any CSS selector.  However, often we want the variable to apply
to all scopes.  Therefore the scope is often defined as ```:root``` so that it has global scope.

## Declaring Variables

```css
   :root {--primaryColor: #26408B;
          --secondaryColor: #81B1D5;
          --accentColor:  #ff4500;
          --borderFormat: 1px solid var(--secondaryColor);
          --defaultImgWidth: 250px;
          --defaultImgHeight: 250px;
   }

## Using Variables

   .productSidebar {color: var(--primaryColor);
                    background-color: var(--accentColor);
                    border: var(--borderFormat);
   }

   h2 {color:var(--primaryColor);
       color:var(--secondaryColor;)
   }
```

## Variables and the Cascade

The CSS Cascade rules still apply to variables.

Often a file containing variables needs to be applied across other stylesheets.  Therefore a file containing the variable declarations often is placed first.
