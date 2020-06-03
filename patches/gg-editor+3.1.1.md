1. dragAddEdge.ts

- support G6 3.5.0 addItem
- add `animateAnchorCfg` to support animate anchor
  usage:

```
<Flow
  className={styles.graph}
  ...
  customModes={(mode, behaviors) => {
    if (mode === 'default') {
      merge(behaviors, {
        'drag-add-edge': {
          type: 'drag-add-edge',
          animateAnchorCfg: {
            type: 'animate-circle',
            r: 3,
            size: [5, 5],
            lineWidth: 2,
            fill: '#FFFFFF',
            stroke: '#5AAAFF',
          },
        },
     });
   }
   return behaviors;
  }}
  ...
/>
```

2. use father-build & webpack to replace build.js

3. add some `//ts-ignore` to ignore some compiler error
4. add resize support, now graph can be resized when window size changed