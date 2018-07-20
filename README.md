# @gurinder/vue-tabs

Inspired by https://github.com/spatie/vue-tabs-component

### Usage

HTML
```html
<vue-tabs>
    <vue-tab title="Title 1" :active="true">
        content of tab one
    </vue-tab>
    <vue-tab title="Title 2">
        content of tab 2
    </vue-tab>
    <vue-tab title="Title 3">
        content of tab 3
    </vue-tab>
</vue-tabs>
```

JS
```JS
import {Tabs, Tab} from '@gurinder/vue-tabs';
Vue.components('vueTabs', Tabs);
Vue.components('vueTab', Tab);
```

SCSS
```scss
.tab-links {

  > li {
    padding: 10px;
    border: 1px solid transparent;

    &.active {
      background: white;
      color: $primary;
      margin-bottom: -3px;
      @extend .bd;
      border-bottom-color: transparent;
      border-top-right-radius: $border-radius;
      border-top-left-radius: $border-radius;
    }

  }

}
```