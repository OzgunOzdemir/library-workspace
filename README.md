## Numeric Value

Numeric Value Directive for Angular Projects

## Installation

```
npm i numeric-value
```

## Usage

Import `NumericValueModule` in `AppModule`
```typescript
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { NumericValueModule } from 'numeric-value';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule,
    NumericValueModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```

After that you can use numeric value  `numericValue` directive in template

```html
<div class="container">
  <input type="text" placeholder="Numeric value directive does not use" />
  <input type="text" placeholder="Numeric value directive is using" numericValue />
</div>

```
