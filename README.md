## Node / Express Import Aggregation Examples

### About the Project

Distinct and separate exports from the same file, or even multiple files,
can be aggregated and exported in one file. Here's a useful code example below:

```
// In parentModule.js
export { myFunc, myVar } from 'child1.js';
export { myClasses } from 'child2.js';

// In top-level module
import { myVar, myFunc, myClasses } from 'parent.js'
```