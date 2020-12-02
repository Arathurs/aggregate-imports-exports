## Node / Express Import Aggregation Examples

### About the Project

Distinct and separate exports from the same file, or even multiple files, can be aggregated and exported in one file. This is useful when we need a bunch of related modules imported in one place. We can export the individual models from each containing file, and import then with one line. The first method we can use to achieve this is to individually export all needed exports in each file. Then import them all in the needed parent file. Here's a useful code example below:

```
// In parentModule.js
export { myFunc, myVar } from 'child1.js';
export { myClasses } from 'child2.js';

// In top-level module
import { myVar, myFunc, myClasses } from 'parent.js'
```