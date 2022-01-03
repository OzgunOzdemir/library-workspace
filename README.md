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
import { FormsModule } from '@angular/forms';
import { NumericValueModule } from 'numeric-value';


@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule,
    FormsModule,
    NumericValueModule,
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.scss']
})
export class AppComponent {
  public formData = {
    firstInput: '',
    secondInput: ''
  }
}

```

After that you can use numeric value  `numericValue` directive in template

```html
<div class="container">
  <input
    [(ngModel)]="formData.firstInput"
    type="text"
    placeholder="Numeric value directive does not use"
    name="fFirstNumber"
    #firstNumber="ngModel"
    autocomplete="off"
  />
  <input
    [(ngModel)]="formData.secondInput"
    type="text"
    placeholder="Numeric value directive is using"
    name="fSecondNumber"
    #secondNumber="ngModel"
    autocomplete="off"
    numericValue
  />
</div>

```
