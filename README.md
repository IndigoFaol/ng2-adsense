# ng2-adsense
[![NPM version][npm-image]][npm-url]

[npm-image]: https://img.shields.io/npm/v/koa2-raven.svg
[npm-url]: https://npmjs.org/package/koa2-raven

### Use
#### 1. Install
```bash
npm install ng2-adsense --save
```

#### 2. Place Code
Use the standard adsense code somewhere on your index.html
```html
<script async src=//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js></script>
```
#### 3. Add to NgModule
Add AdsenseModule to the imports of your NgModule
```javascript
import { AdsenseModule } from 'ng2-adsense';
@NgModule({
  declarations: [
    AppComponent,
    PageComponent,
    OtherPageComponent,
  ],
  imports: [
    BrowserModule,
    RouterModule.forRoot(AppRoutes, {useHash: true}),
    AdsenseModule, // <--- Add to imports
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```
#### 4. Use
```html
<ng2-adsense [adClient]="'ca-pub-7640562161899788'" [adSlot]="7259870550"><ng2-adsense>
```
