# Progress

### Install

```js
import Vue from 'vue';
import { Progress } from 'vant';

Vue.use(Progress);
```

## Usage

### Basic Usage

Use 'percentage' prop to set current progress

```html
<van-progress :percentage="50" />
```

### Stroke Width

```html
<van-progress :percentage="50" stroke-width="8" />
```

### Inactive

```html
<van-progress inactive :percentage="50" />
```

### Custom Style

Use `pivot-text` to custom text，use `color` to custom bar color

```html
<van-progress pivot-text="Orange" color="#f2826a" :percentage="25" />
<van-progress pivot-text="Red" color="#ee0a24" :percentage="50" />
<van-progress
  :percentage="75"
  pivot-text="Purple"
  pivot-color="#7232dd"
  color="linear-gradient(to right, #be99ff, #7232dd)"
/>
```

## API

### Props

| Attribute | Description | Type | Default |
| --- | --- | --- | --- |
| percentage | Percentage | _number \| string_ | `0` |
| stroke-width `v2.2.1` | Stroke width | _number \| string_ | `4px` |
| color | Color | _string_ | `#1989fa` |
| track-color `v2.2.9` | Track color | _string_ | `#e5e5e5` |
| pivot-text | Pivot text | _string_ | percentage |
| pivot-color | Pivot text background color | _string_ | inherit progress color |
| text-color | Pivot text color | _string_ | `white` |
| inactive | Whether to be gray | _boolean_ | `false` |
| show-pivot | Whether to show text | _boolean_ | `true` |
