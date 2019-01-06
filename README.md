# @nowzoo/ngx-crumbs

Breadcrumbs and window title for Angular apps.

[Demo](https://nowzoo.github.io/ngx-crumbs/)
|
[Demo Source Code](https://github.com/nowzoo/ngx-crumbs/tree/master/projects/ngx-crumbs-demo/src/app)

[Documentation](https://nowzoo.github.io/ngx-crumbs/docs/)


## Quick start

```bash
npm i @nowzoo/ngx-crumbs --save
```

Import the module...
```typescript
import { NgxCrumbsModule } from '@nowzoo/ngx-crumbs';
@NgModule({
  imports: [
    NgxCrumbsModule.forRoot()
  ],
})
export class AppModule { }
```

Add breadcrumbs to your route components using `ng-template` and the `ngxCrumb` directive. The content of the crumb can be dynamic...
```html
<ng-template ngxCrumb>Dynamic: {{counter}}</ng-template>
```

To have the crumbs automatically update the window title, add the `NgxCrumbsWindowTitleComponent` to your app component...

```html
<ngx-crumbs-window-title></ngx-crumbs-window-title>
```

To display Bootstrap breadcrumbs, use `NgxCrumbsComponent`...

```html
<ngx-crumbs></ngx-crumbs>
```

## Contributing

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.1.4.

`git clone https://github.com/nowzoo/ngx-crumbs.git`

The library code is in `projects/ngx-crumbs`.

The demo is in `projects/ngx-crumbs-demo`

Build the library: `ng build ngx-crumbs`

Serve the demo locally:  `ng serve ngx-crumbs-demo`



### Unit tests

Run `ng test ngx-crumbs` to execute the unit tests via [Karma](https://karma-runner.github.io).

The library tests can also be run with Wallaby. Select the `wallaby.js` file in `projects/ngx-crumbs`.
